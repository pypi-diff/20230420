# Comparing `tmp/trigger_count-0.1.6.tar.gz` & `tmp/trigger_count-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trigger_count-0.1.6.tar", max compression
+gzip compressed data, was "trigger_count-0.1.7.tar", max compression
```

## Comparing `trigger_count-0.1.6.tar` & `trigger_count-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0        0 2023-03-13 15:40:57.895086 trigger_count-0.1.6/README.md
--rw-r--r--   0        0        0      395 2023-03-15 12:53:16.400191 trigger_count-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-13 15:40:57.895086 trigger_count-0.1.6/trigger_count/__init__.py
--rw-r--r--   0        0        0        0 2023-03-13 15:40:57.895086 trigger_count-0.1.6/trigger_count/daq/__init__.py
--rw-r--r--   0        0        0     2515 2023-03-13 15:40:57.895086 trigger_count-0.1.6/trigger_count/daq/labjack.py
--rw-r--r--   0        0        0        0 2023-03-13 15:40:57.895086 trigger_count-0.1.6/trigger_count/workaround/__init__.py
--rw-r--r--   0        0        0     6268 2023-03-15 12:53:16.388191 trigger_count-0.1.6/trigger_count/workaround/align.py
--rw-r--r--   0        0        0     3489 2023-03-13 15:40:57.895086 trigger_count-0.1.6/trigger_count/workaround/arduino.py
--rw-r--r--   0        0        0     1488 2023-03-14 16:58:13.192464 trigger_count-0.1.6/trigger_count/workaround/start_gui.py
--rw-r--r--   0        0        0     3034 2023-03-15 09:08:13.632010 trigger_count-0.1.6/trigger_count/workaround/xml.py
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 trigger_count-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-20 09:07:10.209580 trigger_count-0.1.7/README.md
+-rw-r--r--   0        0        0      395 2023-04-20 09:56:01.121807 trigger_count-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 09:07:10.209580 trigger_count-0.1.7/trigger_count/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 09:07:10.209580 trigger_count-0.1.7/trigger_count/daq/__init__.py
+-rw-r--r--   0        0        0     3162 2023-04-20 09:16:50.245417 trigger_count-0.1.7/trigger_count/daq/labjack.py
+-rw-r--r--   0        0        0        0 2023-04-20 09:32:07.572241 trigger_count-0.1.7/trigger_count/kengo/__init__.py
+-rw-r--r--   0        0        0      963 2023-04-20 09:40:17.310325 trigger_count-0.1.7/trigger_count/kengo/arduino.py
+-rw-r--r--   0        0        0        0 2023-04-20 09:07:10.209580 trigger_count-0.1.7/trigger_count/workaround/__init__.py
+-rw-r--r--   0        0        0     6268 2023-04-20 09:55:13.764831 trigger_count-0.1.7/trigger_count/workaround/align.py
+-rw-r--r--   0        0        0     3489 2023-04-20 09:07:10.209580 trigger_count-0.1.7/trigger_count/workaround/arduino.py
+-rw-r--r--   0        0        0     1488 2023-04-20 09:07:10.209580 trigger_count-0.1.7/trigger_count/workaround/start_gui.py
+-rw-r--r--   0        0        0     3034 2023-04-20 09:07:10.209580 trigger_count-0.1.7/trigger_count/workaround/xml.py
+-rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 trigger_count-0.1.7/PKG-INFO
```

### Comparing `trigger_count-0.1.6/trigger_count/daq/labjack.py` & `trigger_count-0.1.7/trigger_count/daq/labjack.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 class DaqLabjack:
     """Basic class to use labjack as a data acquisition system (daq)."""
 
     def __init__(self) -> None:
         """Open connection to labjack."""
         self.handle = ljm.openS("T7", "ANY", "ANY")
         self.counters: dict[str, str] = {}
+        self._main_counter: str | None = None
 
     def read_port(self, port_name: str) -> float:
         """Read value from labjack port."""
         value = ljm.eReadName(self.handle, port_name)
         return value
 
     def add_counter(self, counter_name: str, port_name: str) -> None:
@@ -47,22 +48,38 @@
     def read_all_counters(self) -> dict:
         """Read all currently configured counters."""
         values = {}
         for counter_name, port_name in self.counters.items():
             values[counter_name] = self.read_counter_by_port(port_name)
         return values
 
+    def set_main_counter(self, counter_name: str) -> None:
+        """Set name of main counter."""
+        if counter_name in self.counters.keys():
+            self._main_counter = counter_name
+        else:
+            raise KeyError(f"Counter {counter_name} not added!")
+
     def block_until_new_count(self, counter_name: str) -> None:
         """Block script advancement until a new count has been registered."""
         last_count = self.read_counter_by_name(counter_name)
         while True:
             new_count = self.read_counter_by_name(counter_name)
             if new_count != last_count:
                 break
 
+    def read_main_counter(self) -> int:
+        """Read value of main counter."""
+        count = self.read_counter_by_name(self._main_counter)
+        return count
+
+    def wait_for_main_counter(self) -> None:
+        """Hold script until main counter has increased."""
+        self.block_until_new_count(self._main_counter)
+
 
 if __name__ == "__main__":
     daq = DaqLabjack()
     daq.add_counter("eye_camera", "DIO2")
     while True:
         print(datetime.datetime.now(), daq.read_all_counters())
         time.sleep(1)
```

### Comparing `trigger_count-0.1.6/trigger_count/workaround/align.py` & `trigger_count-0.1.7/trigger_count/workaround/align.py`

 * *Files identical despite different names*

### Comparing `trigger_count-0.1.6/trigger_count/workaround/arduino.py` & `trigger_count-0.1.7/trigger_count/workaround/arduino.py`

 * *Files identical despite different names*

### Comparing `trigger_count-0.1.6/trigger_count/workaround/start_gui.py` & `trigger_count-0.1.7/trigger_count/workaround/start_gui.py`

 * *Files identical despite different names*

### Comparing `trigger_count-0.1.6/trigger_count/workaround/xml.py` & `trigger_count-0.1.7/trigger_count/workaround/xml.py`

 * *Files identical despite different names*

