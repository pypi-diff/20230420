# Comparing `tmp/logging_exceptions-0.1.8.tar.gz` & `tmp/logging_exceptions-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/logging_exceptions-0.1.8.tar", last modified: Mon Apr 30 09:04:56 2018, max compression
+gzip compressed data, was "logging_exceptions-0.1.9.tar", last modified: Thu Apr 20 20:54:24 2023, max compression
```

## Comparing `logging_exceptions-0.1.8.tar` & `logging_exceptions-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 thiel     (5095) tbi       (1000)        0 2018-04-30 09:04:56.000000 logging_exceptions-0.1.8/
-drwxr-xr-x   0 thiel     (5095) tbi       (1000)        0 2018-04-30 09:04:56.000000 logging_exceptions-0.1.8/logging_exceptions.egg-info/
--rw-r--r--   0 thiel     (5095) tbi       (1000)     7795 2018-04-30 09:04:56.000000 logging_exceptions-0.1.8/logging_exceptions.egg-info/PKG-INFO
--rw-r--r--   0 thiel     (5095) tbi       (1000)      239 2018-04-30 09:04:56.000000 logging_exceptions-0.1.8/logging_exceptions.egg-info/SOURCES.txt
--rw-r--r--   0 thiel     (5095) tbi       (1000)        1 2018-04-30 09:04:56.000000 logging_exceptions-0.1.8/logging_exceptions.egg-info/dependency_links.txt
--rw-r--r--   0 thiel     (5095) tbi       (1000)       19 2018-04-30 09:04:56.000000 logging_exceptions-0.1.8/logging_exceptions.egg-info/top_level.txt
--rw-r--r--   0 thiel     (5095) tbi       (1000)     1057 2018-04-09 13:37:36.000000 logging_exceptions-0.1.8/LICENSE
--rw-r--r--   0 thiel     (5095) tbi       (1000)       21 2018-04-09 13:37:36.000000 logging_exceptions-0.1.8/MANIFEST.in
--rw-r--r--   0 thiel     (5095) tbi       (1000)     5704 2017-07-28 13:14:59.000000 logging_exceptions-0.1.8/README.rst
--rw-r--r--   0 thiel     (5095) tbi       (1000)    11991 2018-04-30 09:03:14.000000 logging_exceptions-0.1.8/logging_exceptions.py
--rw-r--r--   0 thiel     (5095) tbi       (1000)       79 2018-04-30 09:04:56.000000 logging_exceptions-0.1.8/setup.cfg
--rw-r--r--   0 thiel     (5095) tbi       (1000)      930 2018-04-30 09:03:28.000000 logging_exceptions-0.1.8/setup.py
--rw-r--r--   0 thiel     (5095) tbi       (1000)     7795 2018-04-30 09:04:56.000000 logging_exceptions-0.1.8/PKG-INFO
+drwxr-xr-x   0 thiel     (1000) thiel     (1000)        0 2023-04-20 20:54:24.365803 logging_exceptions-0.1.9/
+-rw-r--r--   0 thiel     (1000) thiel     (1000)     1057 2021-07-21 08:49:27.000000 logging_exceptions-0.1.9/LICENSE
+-rw-r--r--   0 thiel     (1000) thiel     (1000)       21 2021-07-21 08:49:27.000000 logging_exceptions-0.1.9/MANIFEST.in
+-rw-r--r--   0 thiel     (1000) thiel     (1000)     6336 2023-04-20 20:54:24.365803 logging_exceptions-0.1.9/PKG-INFO
+-rw-r--r--   0 thiel     (1000) thiel     (1000)     5704 2021-07-21 08:49:27.000000 logging_exceptions-0.1.9/README.rst
+drwxr-xr-x   0 thiel     (1000) thiel     (1000)        0 2023-04-20 20:54:24.365803 logging_exceptions-0.1.9/logging_exceptions.egg-info/
+-rw-r--r--   0 thiel     (1000) thiel     (1000)     6336 2023-04-20 20:54:24.000000 logging_exceptions-0.1.9/logging_exceptions.egg-info/PKG-INFO
+-rw-r--r--   0 thiel     (1000) thiel     (1000)      239 2023-04-20 20:54:24.000000 logging_exceptions-0.1.9/logging_exceptions.egg-info/SOURCES.txt
+-rw-r--r--   0 thiel     (1000) thiel     (1000)        1 2023-04-20 20:54:24.000000 logging_exceptions-0.1.9/logging_exceptions.egg-info/dependency_links.txt
+-rw-r--r--   0 thiel     (1000) thiel     (1000)       19 2023-04-20 20:54:24.000000 logging_exceptions-0.1.9/logging_exceptions.egg-info/top_level.txt
+-rw-r--r--   0 thiel     (1000) thiel     (1000)    12005 2021-07-21 08:49:42.000000 logging_exceptions-0.1.9/logging_exceptions.py
+-rw-r--r--   0 thiel     (1000) thiel     (1000)       79 2023-04-20 20:54:24.365803 logging_exceptions-0.1.9/setup.cfg
+-rw-r--r--   0 thiel     (1000) thiel     (1000)      930 2023-04-20 20:53:16.000000 logging_exceptions-0.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `logging_exceptions-0.1.8/logging_exceptions.egg-info/PKG-INFO` & `logging_exceptions-0.1.9/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,195 +1,177 @@
-Metadata-Version: 1.1
-Name: logging-exceptions
-Version: 0.1.8
-Summary: Self-logging exceptions: Attach log messages to exceptions and output them conditionally.
-Home-page: https://github.com/Bernhard10/logging_exceptions
-Author: Bernhard C. Thiel
-Author-email: thiel@tbi.univie.ac.at
-License: MIT
-Description-Content-Type: UNKNOWN
-Description: Self-logging exceptions
-        =======================
-        
-        * `Source on GitHub <https://github.com/bernhard10/logging_exceptions>`_
-        
-        Installation
-        ------------
-        
-        
-        Use setup.py :
-        
-        .. code-block:: bash
-        
-            python setup.py install
-        
-        Warning
-        -------
-        
-        This module modifies `sys.excepthook` when it is imported!
-        
-        Usage
-        -----
-        
-        Self-logging exceptions
-        ~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Attach a log message to an exception:
-        
-        .. code-block:: python
-        
-            import logging
-            import logging_exceptions as exlog
-        
-            e = ValueError("Wrong value")
-            logger = logging.getLogger(__name__)
-            with exlog.log_to_exception(logger, e):
-                logger.critical("This is a %s log mressage", "long")
-            raise e # The exception can also be raised inside the with statement
-        
-        
-        If the error is not caught, the log message will be displayed upon program
-        termination.
-        
-        Catch the error and display the log message at a costum log-level:
-        
-        .. code-block:: python
-        
-            import logging_exceptions as exlog
-            import logging
-            try:
-                e = ValueError("Wrong value")
-                logger = logging.getLogger(__name__)
-                with exlog.log_to_exception(logger, e):
-                    logger.critical("This is a %s log mressage", "long")
-                    raise e
-            except ValueError as err:
-                exlog.log(err, level=logging.DEBUG, with_stacktrace=False)
-        
-        Here, `exlog.log` is a synonym for `exlog.log_exception`
-        
-        Logging from a different function name and line number
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        The code in log_exception calls the `_log` function of a Logger object.
-        To avoid recording the function name and line number of `log_to_exception`,
-        `logging_exception` calls `logging.setLoggerClass(ExlogLogger)` to set the
-        class for all loggers created after import of `logging_exception` to `ExlogLogger`.
-        
-        `ExlogLogger` is a subclass of `logging.Logger` defined by this module. It
-        overrides `findCaller` to have more control over the recorded caller.
-        In addition to ignoring functions defined inside `logging_exceptions`,
-        `ExlogLogger` classes have the public attribute `ignored_functions`.
-        
-        By adding function names to `ignored_functions`, it is possible to record
-        matching function's parents instead of matching functions as the caller.
-        
-        In particular, the context manager `logging_exceptions.log_at_caller` can be used
-        in helper functions to temporarily update a logger's `ignored_functions` in order to record a function's caller instead of the function.
-        
-        The following code will emit a log message with the function name set to 
-        `foo`, not `helper_function`:
-        
-         .. code-block:: python
-        
-             import logging_exceptions as exlog
-             logger = logging.get_logger(__name__)
-             def helper_function():
-                with exlog.log_at_caller(logger):
-                  logger.log("This is a log message")
-             def foo():
-                helper_function()
-        
-        
-        
-        Commandline convenience functions
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        The following convenience functions are not directly related to exceptions,
-        but useful if you use argparse.
-        
-        Add the '--verbose', '--debug' and '--quiet' options to an
-        argparse.Argumentparser instance.
-        
-        .. code-block:: python
-        
-            import argparse
-            import logging_exceptions as exlog
-        
-            parser=argparse.ArgumentParser("Some help text")
-            exlog.update_parser(parser)
-            args = parser.parse_args()
-        
-            logging.basicConfig()
-            # The following call updates the log levels of the root logger
-            # and potential some other loggers.
-            exlog.config_from_args(args)
-        
-        Now the script can be used from the commandline like this:
-        
-        .. code-block:: bash
-        
-            # Set the log-level for the loggers with the names `path.to.module1`
-            # and `path.to.module2` to DEBUG.
-            python script.py --debug path.to.module1,path.to.module2
-        
-        Examples
-        --------
-        
-        See the file 'logging_exceptions_examples.py'
-        
-        Comparison to logging.handlers.MemoryHandler
-        --------------------------------------------
-        
-        The logging.handlers module contains a handler for a similar purpose: The MemoryHandler.
-        It buffers log messages and only emits them, if a log record of severity error or above is encountered.
-        I will quickly explain the differences between MemoryHandler and my module:
-        
-        MemoryHandler is great if you know that an event of severity ERROR may occur
-        in the future (typically in the same function) and you want to prepare for
-        this potential exception. Typically, you know the scope for which the exceptions
-        have to be buffered and you know when the buffered exceptions are no longer needed and can be discarded.
-        
-        While for MemoryHandler the error condition is rather unspecific, the scope in
-        which we have to decide between discarding and emitting the log messages is well
-        known.
-        
-        The `log_to_exception` decorator, on the other hand, is useful if the exception
-        is well specified (it is already created/ caught), but the the scope in which
-        the exception may or may not be caught is unspecified. Examples would be
-        library functions that raise an error.
-        
-        A typical example would be the following:
-        
-        .. code-block:: python
-        
-            import logging
-            from logging_exceptions import log_to_exception
-        
-            # Whoever calls public_function may want to catch the ValueError and hide
-            # the log messages or change their level to logging.DEBUG
-            def public_function():
-                logger = logging.getLogger(__name__)
-                a = some_complex_calculation(12)
-                try:
-                    some_function(a)
-                except ValueError as e:
-                    with log_to_exception(logger, e):
-                        log.error("While calling `some_function` with %s, "
-                                  "which is result of `some_complex_calculation`(%d),"
-                                  " an error occurred", a, 12)
-                    raise
-        
-        
-        Compatibility
-        -------------
-        
-        Compatible with python 2.7 and python 3
-        
-Keywords: logging exceptions
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
+Self-logging exceptions
+=======================
+
+* `Source on GitHub <https://github.com/bernhard10/logging_exceptions>`_
+
+Installation
+------------
+
+
+Use setup.py :
+
+.. code-block:: bash
+
+    python setup.py install
+
+Warning
+-------
+
+This module modifies `sys.excepthook` when it is imported!
+
+Usage
+-----
+
+Self-logging exceptions
+~~~~~~~~~~~~~~~~~~~~~~~
+
+Attach a log message to an exception:
+
+.. code-block:: python
+
+    import logging
+    import logging_exceptions as exlog
+
+    e = ValueError("Wrong value")
+    logger = logging.getLogger(__name__)
+    with exlog.log_to_exception(logger, e):
+        logger.critical("This is a %s log mressage", "long")
+    raise e # The exception can also be raised inside the with statement
+
+
+If the error is not caught, the log message will be displayed upon program
+termination.
+
+Catch the error and display the log message at a costum log-level:
+
+.. code-block:: python
+
+    import logging_exceptions as exlog
+    import logging
+    try:
+        e = ValueError("Wrong value")
+        logger = logging.getLogger(__name__)
+        with exlog.log_to_exception(logger, e):
+            logger.critical("This is a %s log mressage", "long")
+            raise e
+    except ValueError as err:
+        exlog.log(err, level=logging.DEBUG, with_stacktrace=False)
+
+Here, `exlog.log` is a synonym for `exlog.log_exception`
+
+Logging from a different function name and line number
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The code in log_exception calls the `_log` function of a Logger object.
+To avoid recording the function name and line number of `log_to_exception`,
+`logging_exception` calls `logging.setLoggerClass(ExlogLogger)` to set the
+class for all loggers created after import of `logging_exception` to `ExlogLogger`.
+
+`ExlogLogger` is a subclass of `logging.Logger` defined by this module. It
+overrides `findCaller` to have more control over the recorded caller.
+In addition to ignoring functions defined inside `logging_exceptions`,
+`ExlogLogger` classes have the public attribute `ignored_functions`.
+
+By adding function names to `ignored_functions`, it is possible to record
+matching function's parents instead of matching functions as the caller.
+
+In particular, the context manager `logging_exceptions.log_at_caller` can be used
+in helper functions to temporarily update a logger's `ignored_functions` in order to record a function's caller instead of the function.
+
+The following code will emit a log message with the function name set to 
+`foo`, not `helper_function`:
+
+ .. code-block:: python
+
+     import logging_exceptions as exlog
+     logger = logging.get_logger(__name__)
+     def helper_function():
+        with exlog.log_at_caller(logger):
+          logger.log("This is a log message")
+     def foo():
+        helper_function()
+
+
+
+Commandline convenience functions
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The following convenience functions are not directly related to exceptions,
+but useful if you use argparse.
+
+Add the '--verbose', '--debug' and '--quiet' options to an
+argparse.Argumentparser instance.
+
+.. code-block:: python
+
+    import argparse
+    import logging_exceptions as exlog
+
+    parser=argparse.ArgumentParser("Some help text")
+    exlog.update_parser(parser)
+    args = parser.parse_args()
+
+    logging.basicConfig()
+    # The following call updates the log levels of the root logger
+    # and potential some other loggers.
+    exlog.config_from_args(args)
+
+Now the script can be used from the commandline like this:
+
+.. code-block:: bash
+
+    # Set the log-level for the loggers with the names `path.to.module1`
+    # and `path.to.module2` to DEBUG.
+    python script.py --debug path.to.module1,path.to.module2
+
+Examples
+--------
+
+See the file 'logging_exceptions_examples.py'
+
+Comparison to logging.handlers.MemoryHandler
+--------------------------------------------
+
+The logging.handlers module contains a handler for a similar purpose: The MemoryHandler.
+It buffers log messages and only emits them, if a log record of severity error or above is encountered.
+I will quickly explain the differences between MemoryHandler and my module:
+
+MemoryHandler is great if you know that an event of severity ERROR may occur
+in the future (typically in the same function) and you want to prepare for
+this potential exception. Typically, you know the scope for which the exceptions
+have to be buffered and you know when the buffered exceptions are no longer needed and can be discarded.
+
+While for MemoryHandler the error condition is rather unspecific, the scope in
+which we have to decide between discarding and emitting the log messages is well
+known.
+
+The `log_to_exception` decorator, on the other hand, is useful if the exception
+is well specified (it is already created/ caught), but the the scope in which
+the exception may or may not be caught is unspecified. Examples would be
+library functions that raise an error.
+
+A typical example would be the following:
+
+.. code-block:: python
+
+    import logging
+    from logging_exceptions import log_to_exception
+
+    # Whoever calls public_function may want to catch the ValueError and hide
+    # the log messages or change their level to logging.DEBUG
+    def public_function():
+        logger = logging.getLogger(__name__)
+        a = some_complex_calculation(12)
+        try:
+            some_function(a)
+        except ValueError as e:
+            with log_to_exception(logger, e):
+                log.error("While calling `some_function` with %s, "
+                          "which is result of `some_complex_calculation`(%d),"
+                          " an error occurred", a, 12)
+            raise
+
+
+Compatibility
+-------------
+
+Compatible with python 2.7 and python 3
```

### Comparing `logging_exceptions-0.1.8/LICENSE` & `logging_exceptions-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `logging_exceptions-0.1.8/README.rst` & `logging_exceptions-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: logging_exceptions
+Version: 0.1.9
+Summary: Self-logging exceptions: Attach log messages to exceptions and output them conditionally.
+Home-page: https://github.com/Bernhard10/logging_exceptions
+Author: Bernhard C. Thiel
+Author-email: thiel@tbi.univie.ac.at
+License: MIT
+Keywords: logging exceptions
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+License-File: LICENSE
+
 Self-logging exceptions
 =======================
 
 * `Source on GitHub <https://github.com/bernhard10/logging_exceptions>`_
 
 Installation
 ------------
```

### Comparing `logging_exceptions-0.1.8/logging_exceptions.py` & `logging_exceptions-0.1.9/logging_exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 
 class ExlogLogger(logging.Logger):
     def __init__(self, name, level=logging.NOTSET):
         super(ExlogLogger, self).__init__(name, level)
         self.ignored_functions = []
 
-    def findCaller(self, stack_info=False):
+    def findCaller(self, stack_info=False, stacklevel=1):
         """
         Modified copy of the original logging.Logger.findCaller function.
 
         Instead of only ignoring the logging Module when searching for
         the function with the logging call, this also ignores logging_exceptions.
 
         This is implemented by replacing
```

### Comparing `logging_exceptions-0.1.8/setup.py` & `logging_exceptions-0.1.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Get the long description from the README file
 with open('README.rst') as f:
     long_description = f.read()
 
 
 setup(name='logging_exceptions',
-      version='0.1.8',
+      version='0.1.9',
       py_modules=['logging_exceptions'],
       author="Bernhard C. Thiel",
       author_email="thiel@tbi.univie.ac.at",
       description="Self-logging exceptions: Attach log messages to exceptions and output them conditionally.",
       long_description=long_description,
       url='https://github.com/Bernhard10/logging_exceptions',
       license='MIT',
```

### Comparing `logging_exceptions-0.1.8/PKG-INFO` & `logging_exceptions-0.1.9/logging_exceptions.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,195 +1,194 @@
-Metadata-Version: 1.1
-Name: logging_exceptions
-Version: 0.1.8
+Metadata-Version: 2.1
+Name: logging-exceptions
+Version: 0.1.9
 Summary: Self-logging exceptions: Attach log messages to exceptions and output them conditionally.
 Home-page: https://github.com/Bernhard10/logging_exceptions
 Author: Bernhard C. Thiel
 Author-email: thiel@tbi.univie.ac.at
 License: MIT
-Description-Content-Type: UNKNOWN
-Description: Self-logging exceptions
-        =======================
-        
-        * `Source on GitHub <https://github.com/bernhard10/logging_exceptions>`_
-        
-        Installation
-        ------------
-        
-        
-        Use setup.py :
-        
-        .. code-block:: bash
-        
-            python setup.py install
-        
-        Warning
-        -------
-        
-        This module modifies `sys.excepthook` when it is imported!
-        
-        Usage
-        -----
-        
-        Self-logging exceptions
-        ~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Attach a log message to an exception:
-        
-        .. code-block:: python
-        
-            import logging
-            import logging_exceptions as exlog
-        
-            e = ValueError("Wrong value")
-            logger = logging.getLogger(__name__)
-            with exlog.log_to_exception(logger, e):
-                logger.critical("This is a %s log mressage", "long")
-            raise e # The exception can also be raised inside the with statement
-        
-        
-        If the error is not caught, the log message will be displayed upon program
-        termination.
-        
-        Catch the error and display the log message at a costum log-level:
-        
-        .. code-block:: python
-        
-            import logging_exceptions as exlog
-            import logging
-            try:
-                e = ValueError("Wrong value")
-                logger = logging.getLogger(__name__)
-                with exlog.log_to_exception(logger, e):
-                    logger.critical("This is a %s log mressage", "long")
-                    raise e
-            except ValueError as err:
-                exlog.log(err, level=logging.DEBUG, with_stacktrace=False)
-        
-        Here, `exlog.log` is a synonym for `exlog.log_exception`
-        
-        Logging from a different function name and line number
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        The code in log_exception calls the `_log` function of a Logger object.
-        To avoid recording the function name and line number of `log_to_exception`,
-        `logging_exception` calls `logging.setLoggerClass(ExlogLogger)` to set the
-        class for all loggers created after import of `logging_exception` to `ExlogLogger`.
-        
-        `ExlogLogger` is a subclass of `logging.Logger` defined by this module. It
-        overrides `findCaller` to have more control over the recorded caller.
-        In addition to ignoring functions defined inside `logging_exceptions`,
-        `ExlogLogger` classes have the public attribute `ignored_functions`.
-        
-        By adding function names to `ignored_functions`, it is possible to record
-        matching function's parents instead of matching functions as the caller.
-        
-        In particular, the context manager `logging_exceptions.log_at_caller` can be used
-        in helper functions to temporarily update a logger's `ignored_functions` in order to record a function's caller instead of the function.
-        
-        The following code will emit a log message with the function name set to 
-        `foo`, not `helper_function`:
-        
-         .. code-block:: python
-        
-             import logging_exceptions as exlog
-             logger = logging.get_logger(__name__)
-             def helper_function():
-                with exlog.log_at_caller(logger):
-                  logger.log("This is a log message")
-             def foo():
-                helper_function()
-        
-        
-        
-        Commandline convenience functions
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        The following convenience functions are not directly related to exceptions,
-        but useful if you use argparse.
-        
-        Add the '--verbose', '--debug' and '--quiet' options to an
-        argparse.Argumentparser instance.
-        
-        .. code-block:: python
-        
-            import argparse
-            import logging_exceptions as exlog
-        
-            parser=argparse.ArgumentParser("Some help text")
-            exlog.update_parser(parser)
-            args = parser.parse_args()
-        
-            logging.basicConfig()
-            # The following call updates the log levels of the root logger
-            # and potential some other loggers.
-            exlog.config_from_args(args)
-        
-        Now the script can be used from the commandline like this:
-        
-        .. code-block:: bash
-        
-            # Set the log-level for the loggers with the names `path.to.module1`
-            # and `path.to.module2` to DEBUG.
-            python script.py --debug path.to.module1,path.to.module2
-        
-        Examples
-        --------
-        
-        See the file 'logging_exceptions_examples.py'
-        
-        Comparison to logging.handlers.MemoryHandler
-        --------------------------------------------
-        
-        The logging.handlers module contains a handler for a similar purpose: The MemoryHandler.
-        It buffers log messages and only emits them, if a log record of severity error or above is encountered.
-        I will quickly explain the differences between MemoryHandler and my module:
-        
-        MemoryHandler is great if you know that an event of severity ERROR may occur
-        in the future (typically in the same function) and you want to prepare for
-        this potential exception. Typically, you know the scope for which the exceptions
-        have to be buffered and you know when the buffered exceptions are no longer needed and can be discarded.
-        
-        While for MemoryHandler the error condition is rather unspecific, the scope in
-        which we have to decide between discarding and emitting the log messages is well
-        known.
-        
-        The `log_to_exception` decorator, on the other hand, is useful if the exception
-        is well specified (it is already created/ caught), but the the scope in which
-        the exception may or may not be caught is unspecified. Examples would be
-        library functions that raise an error.
-        
-        A typical example would be the following:
-        
-        .. code-block:: python
-        
-            import logging
-            from logging_exceptions import log_to_exception
-        
-            # Whoever calls public_function may want to catch the ValueError and hide
-            # the log messages or change their level to logging.DEBUG
-            def public_function():
-                logger = logging.getLogger(__name__)
-                a = some_complex_calculation(12)
-                try:
-                    some_function(a)
-                except ValueError as e:
-                    with log_to_exception(logger, e):
-                        log.error("While calling `some_function` with %s, "
-                                  "which is result of `some_complex_calculation`(%d),"
-                                  " an error occurred", a, 12)
-                    raise
-        
-        
-        Compatibility
-        -------------
-        
-        Compatible with python 2.7 and python 3
-        
 Keywords: logging exceptions
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
+License-File: LICENSE
+
+Self-logging exceptions
+=======================
+
+* `Source on GitHub <https://github.com/bernhard10/logging_exceptions>`_
+
+Installation
+------------
+
+
+Use setup.py :
+
+.. code-block:: bash
+
+    python setup.py install
+
+Warning
+-------
+
+This module modifies `sys.excepthook` when it is imported!
+
+Usage
+-----
+
+Self-logging exceptions
+~~~~~~~~~~~~~~~~~~~~~~~
+
+Attach a log message to an exception:
+
+.. code-block:: python
+
+    import logging
+    import logging_exceptions as exlog
+
+    e = ValueError("Wrong value")
+    logger = logging.getLogger(__name__)
+    with exlog.log_to_exception(logger, e):
+        logger.critical("This is a %s log mressage", "long")
+    raise e # The exception can also be raised inside the with statement
+
+
+If the error is not caught, the log message will be displayed upon program
+termination.
+
+Catch the error and display the log message at a costum log-level:
+
+.. code-block:: python
+
+    import logging_exceptions as exlog
+    import logging
+    try:
+        e = ValueError("Wrong value")
+        logger = logging.getLogger(__name__)
+        with exlog.log_to_exception(logger, e):
+            logger.critical("This is a %s log mressage", "long")
+            raise e
+    except ValueError as err:
+        exlog.log(err, level=logging.DEBUG, with_stacktrace=False)
+
+Here, `exlog.log` is a synonym for `exlog.log_exception`
+
+Logging from a different function name and line number
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The code in log_exception calls the `_log` function of a Logger object.
+To avoid recording the function name and line number of `log_to_exception`,
+`logging_exception` calls `logging.setLoggerClass(ExlogLogger)` to set the
+class for all loggers created after import of `logging_exception` to `ExlogLogger`.
+
+`ExlogLogger` is a subclass of `logging.Logger` defined by this module. It
+overrides `findCaller` to have more control over the recorded caller.
+In addition to ignoring functions defined inside `logging_exceptions`,
+`ExlogLogger` classes have the public attribute `ignored_functions`.
+
+By adding function names to `ignored_functions`, it is possible to record
+matching function's parents instead of matching functions as the caller.
+
+In particular, the context manager `logging_exceptions.log_at_caller` can be used
+in helper functions to temporarily update a logger's `ignored_functions` in order to record a function's caller instead of the function.
+
+The following code will emit a log message with the function name set to 
+`foo`, not `helper_function`:
+
+ .. code-block:: python
+
+     import logging_exceptions as exlog
+     logger = logging.get_logger(__name__)
+     def helper_function():
+        with exlog.log_at_caller(logger):
+          logger.log("This is a log message")
+     def foo():
+        helper_function()
+
+
+
+Commandline convenience functions
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The following convenience functions are not directly related to exceptions,
+but useful if you use argparse.
+
+Add the '--verbose', '--debug' and '--quiet' options to an
+argparse.Argumentparser instance.
+
+.. code-block:: python
+
+    import argparse
+    import logging_exceptions as exlog
+
+    parser=argparse.ArgumentParser("Some help text")
+    exlog.update_parser(parser)
+    args = parser.parse_args()
+
+    logging.basicConfig()
+    # The following call updates the log levels of the root logger
+    # and potential some other loggers.
+    exlog.config_from_args(args)
+
+Now the script can be used from the commandline like this:
+
+.. code-block:: bash
+
+    # Set the log-level for the loggers with the names `path.to.module1`
+    # and `path.to.module2` to DEBUG.
+    python script.py --debug path.to.module1,path.to.module2
+
+Examples
+--------
+
+See the file 'logging_exceptions_examples.py'
+
+Comparison to logging.handlers.MemoryHandler
+--------------------------------------------
+
+The logging.handlers module contains a handler for a similar purpose: The MemoryHandler.
+It buffers log messages and only emits them, if a log record of severity error or above is encountered.
+I will quickly explain the differences between MemoryHandler and my module:
+
+MemoryHandler is great if you know that an event of severity ERROR may occur
+in the future (typically in the same function) and you want to prepare for
+this potential exception. Typically, you know the scope for which the exceptions
+have to be buffered and you know when the buffered exceptions are no longer needed and can be discarded.
+
+While for MemoryHandler the error condition is rather unspecific, the scope in
+which we have to decide between discarding and emitting the log messages is well
+known.
+
+The `log_to_exception` decorator, on the other hand, is useful if the exception
+is well specified (it is already created/ caught), but the the scope in which
+the exception may or may not be caught is unspecified. Examples would be
+library functions that raise an error.
+
+A typical example would be the following:
+
+.. code-block:: python
+
+    import logging
+    from logging_exceptions import log_to_exception
+
+    # Whoever calls public_function may want to catch the ValueError and hide
+    # the log messages or change their level to logging.DEBUG
+    def public_function():
+        logger = logging.getLogger(__name__)
+        a = some_complex_calculation(12)
+        try:
+            some_function(a)
+        except ValueError as e:
+            with log_to_exception(logger, e):
+                log.error("While calling `some_function` with %s, "
+                          "which is result of `some_complex_calculation`(%d),"
+                          " an error occurred", a, 12)
+            raise
+
+
+Compatibility
+-------------
+
+Compatible with python 2.7 and python 3
```

