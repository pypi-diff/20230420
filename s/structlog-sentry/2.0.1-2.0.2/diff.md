# Comparing `tmp/structlog_sentry-2.0.1.tar.gz` & `tmp/structlog_sentry-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structlog_sentry-2.0.1.tar", max compression
+gzip compressed data, was "structlog_sentry-2.0.2.tar", max compression
```

## Comparing `structlog_sentry-2.0.1.tar` & `structlog_sentry-2.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       20 2023-04-18 12:56:42.797586 structlog_sentry-2.0.1/.coveragerc
--rw-r--r--   0        0        0      618 2023-04-18 12:56:42.797586 structlog_sentry-2.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1065 2023-04-18 12:56:42.797586 structlog_sentry-2.0.1/LICENSE
--rw-r--r--   0        0        0     5876 2023-04-18 12:56:42.801586 structlog_sentry-2.0.1/README.md
--rw-r--r--   0        0        0     1225 2023-04-18 12:56:42.801586 structlog_sentry-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     7312 2023-04-18 12:56:42.801586 structlog_sentry-2.0.1/structlog_sentry/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 12:56:42.801586 structlog_sentry-2.0.1/structlog_sentry/py.typed
--rw-r--r--   0        0        0      581 2023-04-18 12:56:42.801586 structlog_sentry-2.0.1/tox.ini
--rw-r--r--   0        0        0     7178 1970-01-01 00:00:00.000000 structlog_sentry-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-04-20 07:33:19.813394 structlog_sentry-2.0.2/.coveragerc
+-rw-r--r--   0        0        0      618 2023-04-20 07:33:19.813394 structlog_sentry-2.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1065 2023-04-20 07:33:19.813394 structlog_sentry-2.0.2/LICENSE
+-rw-r--r--   0        0        0     5876 2023-04-20 07:33:19.813394 structlog_sentry-2.0.2/README.md
+-rw-r--r--   0        0        0     1225 2023-04-20 07:33:19.813394 structlog_sentry-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7884 2023-04-20 07:33:19.813394 structlog_sentry-2.0.2/structlog_sentry/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:33:19.813394 structlog_sentry-2.0.2/structlog_sentry/py.typed
+-rw-r--r--   0        0        0      581 2023-04-20 07:33:19.813394 structlog_sentry-2.0.2/tox.ini
+-rw-r--r--   0        0        0     7178 1970-01-01 00:00:00.000000 structlog_sentry-2.0.2/PKG-INFO
```

### Comparing `structlog_sentry-2.0.1/.pre-commit-config.yaml` & `structlog_sentry-2.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `structlog_sentry-2.0.1/LICENSE` & `structlog_sentry-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `structlog_sentry-2.0.1/README.md` & `structlog_sentry-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `structlog_sentry-2.0.1/pyproject.toml` & `structlog_sentry-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "structlog-sentry"
-version = "2.0.1"
+version = "2.0.2"
 description = "Sentry integration for structlog"
 authors = ["Kiwi.com platform <platform@kiwi.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/kiwicom/structlog-sentry"
 homepage = "https://github.com/kiwicom/structlog-sentry"
```

### Comparing `structlog_sentry-2.0.1/structlog_sentry/__init__.py` & `structlog_sentry-2.0.2/structlog_sentry/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -173,23 +173,38 @@
                 event_dict["sentry"] = "sent"
 
     def _handle_breadcrumb(self, event_dict: EventDict) -> None:
         with capture_internal_exceptions():
             event, hint = self._get_breadcrumb_and_hint(event_dict)
             self._get_hub().add_breadcrumb(event, hint=hint)
 
+    @staticmethod
+    def _get_level_value(level_name: str) -> int:
+        """Get numeric value for the log level name given."""
+        try:
+            # Try to get one of predefined log levels
+            return getattr(logging, level_name)
+        except AttributeError as e:
+            # May be it is a custom log level?
+            level = logging.getLevelName(level_name)
+            if isinstance(level, int):
+                return level
+
+            # Re-raise original error
+            raise ValueError(f"{level_name} is not a valid log level") from e
+
     def __call__(
         self, logger: WrappedLogger, name: str, event_dict: EventDict
     ) -> EventDict:
         """A middleware to process structlog `event_dict` and send it to Sentry."""
         self._original_event_dict = event_dict.copy()
         sentry_skip = event_dict.pop("sentry_skip", False)
 
         if self.active and not sentry_skip and self._can_record(logger, event_dict):
-            level = getattr(logging, event_dict["level"].upper())
+            level = self._get_level_value(event_dict["level"].upper())
 
             if level >= self.event_level:
                 self._handle_event(event_dict)
 
             if level >= self.level:
                 self._handle_breadcrumb(event_dict)
```

### Comparing `structlog_sentry-2.0.1/tox.ini` & `structlog_sentry-2.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `structlog_sentry-2.0.1/PKG-INFO` & `structlog_sentry-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structlog-sentry
-Version: 2.0.1
+Version: 2.0.2
 Summary: Sentry integration for structlog
 Home-page: https://github.com/kiwicom/structlog-sentry
 License: MIT
 Author: Kiwi.com platform
 Author-email: platform@kiwi.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

