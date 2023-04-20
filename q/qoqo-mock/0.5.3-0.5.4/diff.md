# Comparing `tmp/qoqo_mock-0.5.3.tar.gz` & `tmp/qoqo_mock-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoqo_mock-0.5.3.tar", last modified: Fri Feb  3 13:13:10 2023, max compression
+gzip compressed data, was "qoqo_mock-0.5.4.tar", last modified: Thu Apr 20 14:12:30 2023, max compression
```

## Comparing `qoqo_mock-0.5.3.tar` & `qoqo_mock-0.5.4.tar`

### file list

```diff
@@ -1,22 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:13:10.311825 qoqo_mock-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-03 13:12:56.000000 qoqo_mock-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-02-03 13:13:10.311825 qoqo_mock-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-02-03 13:12:56.000000 qoqo_mock-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-03 13:12:56.000000 qoqo_mock-0.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:13:10.311825 qoqo_mock-0.5.3/qoqo_mock/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-02-03 13:12:56.000000 qoqo_mock-0.5.3/qoqo_mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-02-03 13:12:56.000000 qoqo_mock-0.5.3/qoqo_mock/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:13:10.311825 qoqo_mock-0.5.3/qoqo_mock/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-02-03 13:12:56.000000 qoqo_mock-0.5.3/qoqo_mock/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-02-03 13:12:56.000000 qoqo_mock-0.5.3/qoqo_mock/backend/mocked_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:13:10.311825 qoqo_mock-0.5.3/qoqo_mock/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-02-03 13:12:56.000000 qoqo_mock-0.5.3/qoqo_mock/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-02-03 13:12:56.000000 qoqo_mock-0.5.3/qoqo_mock/interface/mocked_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 13:13:10.311825 qoqo_mock-0.5.3/qoqo_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-02-03 13:13:10.000000 qoqo_mock-0.5.3/qoqo_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-03 13:13:10.000000 qoqo_mock-0.5.3/qoqo_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 13:13:10.000000 qoqo_mock-0.5.3/qoqo_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-03 13:13:10.000000 qoqo_mock-0.5.3/qoqo_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-03 13:13:10.000000 qoqo_mock-0.5.3/qoqo_mock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 13:13:10.311825 qoqo_mock-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-02-03 13:12:56.000000 qoqo_mock-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:12:30.918056 qoqo_mock-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 14:12:07.000000 qoqo_mock-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-20 14:12:30.918056 qoqo_mock-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-20 14:12:07.000000 qoqo_mock-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:12:30.914056 qoqo_mock-0.5.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-20 14:12:07.000000 qoqo_mock-0.5.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-04-20 14:12:07.000000 qoqo_mock-0.5.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-20 14:12:07.000000 qoqo_mock-0.5.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-20 14:12:07.000000 qoqo_mock-0.5.4/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-20 14:12:07.000000 qoqo_mock-0.5.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-20 14:12:07.000000 qoqo_mock-0.5.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:12:30.914056 qoqo_mock-0.5.4/qoqo_mock/
+-rw-r--r--   0 runner    (1001) docker     (123)   493771 2023-04-20 14:12:07.000000 qoqo_mock-0.5.4/qoqo_mock/DEPENDENCIES
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-20 14:12:07.000000 qoqo_mock-0.5.4/qoqo_mock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:12:30.914056 qoqo_mock-0.5.4/qoqo_mock/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-20 14:12:07.000000 qoqo_mock-0.5.4/qoqo_mock/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-04-20 14:12:07.000000 qoqo_mock-0.5.4/qoqo_mock/backend/mocked_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:12:30.918056 qoqo_mock-0.5.4/qoqo_mock/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-20 14:12:07.000000 qoqo_mock-0.5.4/qoqo_mock/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-20 14:12:07.000000 qoqo_mock-0.5.4/qoqo_mock/interface/mocked_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:12:30.914056 qoqo_mock-0.5.4/qoqo_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-20 14:12:30.000000 qoqo_mock-0.5.4/qoqo_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-20 14:12:30.000000 qoqo_mock-0.5.4/qoqo_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:12:30.000000 qoqo_mock-0.5.4/qoqo_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-20 14:12:30.000000 qoqo_mock-0.5.4/qoqo_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 14:12:30.000000 qoqo_mock-0.5.4/qoqo_mock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:12:30.918056 qoqo_mock-0.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:12:30.910056 qoqo_mock-0.5.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:12:30.918056 qoqo_mock-0.5.4/tests/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-20 14:12:07.000000 qoqo_mock-0.5.4/tests/backend/test_mocked_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:12:30.918056 qoqo_mock-0.5.4/tests/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-04-20 14:12:07.000000 qoqo_mock-0.5.4/tests/interface/test_mocked_interface.py
```

### Comparing `qoqo_mock-0.5.3/LICENSE` & `qoqo_mock-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_mock-0.5.3/PKG-INFO` & `qoqo_mock-0.5.4/qoqo_mock.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
-Name: qoqo_mock
-Version: 0.5.3
-Summary: Quantum Computing Base Package
-Home-page: https://quantumsimulations.de
-Author: HQS Quantum Simulations
-Author-email: info@quantumsimulations.de
+Name: qoqo-mock
+Version: 0.5.4
+Author-email: HQS Quantum Simulation GmbH <info@quantumsimulations.de>
 License: Apache-2.0
-Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: dev
 License-File: LICENSE
 
 <img src="qoqo_Logo_vertical_color.png" alt="qoqo logo" width="300" />
 
 # qoqo-mock
 
 Mocking backend for the qoqo/roqoqo quantum toolkit by [HQS Quantum Simulations](https://quantumsimulations.de).
@@ -49,12 +48,10 @@
 roqoqo circuits can be sent to the mock backend and all steps of a full hardware backend are applied, except calling actual quantum hardware. Measurements return random results.  
 This backend is designed purely for benchmarking purposes.
 
 ## General Notes
 
 This software is still in the beta stage. Functions and documentation are not yet complete and breaking changes can occur.
 
-This project is partly supported by [PlanQK](https://planqk.de).
-
 ## Contributing
 
 We welcome contributions to the project. If you want to contribute code, please have a look at CONTRIBUTE.md for our code contribution guidelines.
```

### Comparing `qoqo_mock-0.5.3/README.md` & `qoqo_mock-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `qoqo_mock-0.5.3/qoqo_mock/__init__.py` & `qoqo_mock-0.5.4/qoqo_mock/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,13 +18,9 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
-from qoqo_mock.__version__ import __version__
-from qoqo_mock.interface import (
-    mocked_call_operation,
-    mocked_call_circuit
-)
+from qoqo_mock.interface import mocked_call_operation, mocked_call_circuit
 from qoqo_mock.backend import MockedBackend
```

### Comparing `qoqo_mock-0.5.3/qoqo_mock/__version__.py` & `qoqo_mock-0.5.4/qoqo_mock/backend/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,22 @@
-"""qoqo_mock version information"""
+"""Qoqo backend for mocking.
+
+.. autosummary::
+    :toctree: generated/
+
+    MockedBackend
+
+"""
 # Copyright © 2019-2023 HQS Quantum Simulations GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except
 # in compliance with the License. You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
-__version__ = 'v0.5.3'
+from qoqo_mock.backend.mocked_backend import (
+    MockedBackend,
+)
```

### Comparing `qoqo_mock-0.5.3/qoqo_mock/backend/__init__.py` & `qoqo_mock-0.5.4/qoqo_mock/interface/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-"""Qoqo backend for mocking.
-
-.. autosummary::
-    :toctree: generated/
-
-    MockedBackend
-
-"""
+"""Mocked interface for qoqo operations and circuits."""
 # Copyright © 2019-2023 HQS Quantum Simulations GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except
 # in compliance with the License. You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
-from qoqo_mock.backend.mocked_backend import (
-    MockedBackend,
+
+from qoqo_mock.interface.mocked_interface import (
+    mocked_call_operation,
+    mocked_call_circuit,
 )
```

### Comparing `qoqo_mock-0.5.3/qoqo_mock/backend/mocked_backend.py` & `qoqo_mock-0.5.4/qoqo_mock/backend/mocked_backend.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,51 @@
-"""Mocked Backend"""
+"""Mocked Backend."""
 # Copyright © 2019-2023 HQS Quantum Simulations GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except
 # in compliance with the License. You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 from qoqo import Circuit
-from typing import (
-    Tuple,
-    List,
-    Dict,
-    Any,
-    Optional,
-    cast
-)
+from typing import Tuple, List, Dict, Any, Optional, cast
 from qoqo_mock import mocked_call_circuit
 
 
 class MockedBackend(object):
-    r"""Mocked backend to qoqo
+    r"""Mocked backend to qoqo.
 
     The mocked backend mock-simulates a quantum circuit on a given device by translating the qoqo
     circuit using the qoqo_mocked interface. This interface produces random measurements coherent
     with the measured quantity. These results are then output from the run function in this backend
     and are accessible through the classical registers dictionary.
     """
 
-    def __init__(self,
-                 number_qubits: int = 1) -> None:
-        """Initialize backend
+    def __init__(self, number_qubits: int = 1) -> None:
+        """Initialize backend.
 
         Args:
             number_qubits: The number of qubits to use
 
         """
         self.name = "mocked"
         self.number_qubits = number_qubits
 
-    def run_circuit(self, circuit: Circuit
-                    ) -> Tuple[Dict[str, List[List[bool]]],
-                               Dict[str, List[List[float]]],
-                               Dict[str, List[List[complex]]]]:
-        """Run a circuit with the Mocked backend
+    def run_circuit(
+        self, circuit: Circuit
+    ) -> Tuple[
+        Dict[str, List[List[bool]]],
+        Dict[str, List[List[float]]],
+        Dict[str, List[List[complex]]],
+    ]:
+        """Run a circuit with the Mocked backend.
 
         Args:
             circuit: The circuit that is run
 
         Returns:
             Union[None, Dict[str, 'RegisterOutput']]
 
@@ -61,62 +56,80 @@
         internal_complex_register_dict: Dict[str, List[complex]] = dict()
 
         output_bit_register_dict: Dict[str, List[List[bool]]] = dict()
         output_float_register_dict: Dict[str, List[List[float]]] = dict()
         output_complex_register_dict: Dict[str, List[List[complex]]] = dict()
 
         for bit_def in circuit.filter_by_tag("DefinitionBit"):
-            internal_bit_register_dict[bit_def.name()] = [False for _ in range(bit_def.length())]
+            internal_bit_register_dict[bit_def.name()] = [
+                False for _ in range(bit_def.length())
+            ]
             if bit_def.is_output():
                 output_bit_register_dict[bit_def.name()] = list()
 
         for float_def in circuit.filter_by_tag("DefinitionFloat"):
             internal_float_register_dict[float_def.name()] = [
-                0.0 for _ in range(float_def.length())]
+                0.0 for _ in range(float_def.length())
+            ]
             if float_def.is_output():
-                output_float_register_dict[float_def.name()] = cast(List[List[float]], list())
+                output_float_register_dict[float_def.name()] = cast(
+                    List[List[float]], list()
+                )
 
         for complex_def in circuit.filter_by_tag("DefinitionComplex"):
             internal_complex_register_dict[complex_def.name()] = [
-                complex(0.0) for _ in range(complex_def.length())]
+                complex(0.0) for _ in range(complex_def.length())
+            ]
             if complex_def.is_output():
-                output_complex_register_dict[complex_def.name()] = cast(List[List[complex]], list())
-
-        (internal_bit_register_dict,
-         internal_float_register_dict,
-         internal_complex_register_dict,
-         output_bit_register_dict,
-         output_complex_register_dict) = mocked_call_circuit(
+                output_complex_register_dict[complex_def.name()] = cast(
+                    List[List[complex]], list()
+                )
+
+        (
+            internal_bit_register_dict,
+            internal_float_register_dict,
+            internal_complex_register_dict,
+            output_bit_register_dict,
+            output_complex_register_dict,
+        ) = mocked_call_circuit(
             circuit=circuit,
             classical_bit_registers=internal_bit_register_dict,
             classical_float_registers=internal_float_register_dict,
             classical_complex_registers=internal_complex_register_dict,
             output_bit_register_dict=output_bit_register_dict,
             output_complex_register_dict=output_complex_register_dict,
-            number_qubits=self.number_qubits)
+            number_qubits=self.number_qubits,
+        )
 
         for name, reg in output_bit_register_dict.items():
             if name in internal_bit_register_dict.keys():
                 reg.append(internal_bit_register_dict[name])
 
         for name, reg in output_float_register_dict.items():  # type: ignore
             if name in internal_float_register_dict.keys():
                 reg.append(internal_float_register_dict[name])  # type: ignore
 
         for name, reg in output_complex_register_dict.items():  # type: ignore
             if name in internal_complex_register_dict.keys():
-                reg.append(internal_complex_register_dict[name])    # type: ignore
+                reg.append(internal_complex_register_dict[name])  # type: ignore
 
-        return (output_bit_register_dict, output_float_register_dict, output_complex_register_dict)
+        return (
+            output_bit_register_dict,
+            output_float_register_dict,
+            output_complex_register_dict,
+        )
 
-    def run_measurement_registers(self, measurement: Any
-                                  ) -> Tuple[Dict[str, List[List[bool]]],
-                                             Dict[str, List[List[float]]],
-                                             Dict[str, List[List[complex]]]]:
-        """Run all circuits of a measurement with the Mocked backend
+    def run_measurement_registers(
+        self, measurement: Any
+    ) -> Tuple[
+        Dict[str, List[List[bool]]],
+        Dict[str, List[List[float]]],
+        Dict[str, List[List[complex]]],
+    ]:
+        """Run all circuits of a measurement with the Mocked backend.
 
         Args:
             measurement: The measurement that is run
 
         Returns:
             Union[None, Dict[str, 'RegisterOutput']]
 
@@ -129,42 +142,43 @@
         output_complex_register_dict: Dict[str, List[List[complex]]] = dict()
         for circuit in measurement.circuits():
             if constant_circuit is None:
                 run_circuit = circuit
             else:
                 run_circuit = constant_circuit + circuit
 
-            (tmp_bit_register_dict,
-             tmp_float_register_dict,
-             tmp_complex_register_dict) = self.run_circuit(
-                run_circuit
-            )
+            (
+                tmp_bit_register_dict,
+                tmp_float_register_dict,
+                tmp_complex_register_dict,
+            ) = self.run_circuit(run_circuit)
             output_bit_register_dict.update(tmp_bit_register_dict)
             output_float_register_dict.update(tmp_float_register_dict)
             output_complex_register_dict.update(tmp_complex_register_dict)
         return (
             output_bit_register_dict,
             output_float_register_dict,
-            output_complex_register_dict
+            output_complex_register_dict,
         )
 
-    def run_measurement(self, measurement: Any
-                        ) -> Optional[Dict[str, float]]:
-        """Run a circuit with the Mocked backend
+    def run_measurement(self, measurement: Any) -> Optional[Dict[str, float]]:
+        """Run a circuit with the Mocked backend.
 
         Args:
             measurement: The measurement that is run
 
         Returns:
             Union[None, Dict[str, 'RegisterOutput']]
 
         """
         # Initializing the classical registers for calculation and output
 
-        (output_bit_register_dict,
+        (
+            output_bit_register_dict,
             output_float_register_dict,
-            output_complex_register_dict) = self.run_measurement_registers(measurement)
+            output_complex_register_dict,
+        ) = self.run_measurement_registers(measurement)
         return measurement.evaluate(
             output_bit_register_dict,
             output_float_register_dict,
-            output_complex_register_dict
+            output_complex_register_dict,
         )
```

### Comparing `qoqo_mock-0.5.3/qoqo_mock/interface/mocked_interface.py` & `qoqo_mock-0.5.4/qoqo_mock/interface/mocked_interface.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,59 +9,57 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
 from qoqo import operations as ops
 from qoqo import Circuit
-from typing import (
-    cast,
-    Dict,
-    List,
-    Any,
-    Tuple
-)
+from typing import cast, Dict, List, Any, Tuple
 import numpy as np
 
-_ALLOWED_PRAGMAS = ['PragmaSetNumberOfMeasurements',
-                    'PragmaSetStateVector',
-                    'PragmaSetDensityMatrix',
-                    'PragmaNoise',
-                    'PragmaDamping',
-                    'PragmaDepolarising',
-                    'PragmaDephasing',
-                    'PragmaRandomNoise',
-                    'PragmaGeneralNoise',
-                    'PragmaRepeatGate',
-                    'PragmaBoostNoise',
-                    'PragmaStopParallelBlock',
-                    'PragmaSleep',
-                    'PragmaGlobalPhase',
-                    'PragmaActiveReset',
-                    'InputSymbolic',
-                    'PragmaStartDecompositionBlock',
-                    'PragmaStopDecompositionBlock',
-                    'PragmaConditional']
+_ALLOWED_PRAGMAS = [
+    "PragmaSetNumberOfMeasurements",
+    "PragmaSetStateVector",
+    "PragmaSetDensityMatrix",
+    "PragmaNoise",
+    "PragmaDamping",
+    "PragmaDepolarising",
+    "PragmaDephasing",
+    "PragmaRandomNoise",
+    "PragmaGeneralNoise",
+    "PragmaRepeatGate",
+    "PragmaBoostNoise",
+    "PragmaStopParallelBlock",
+    "PragmaSleep",
+    "PragmaGlobalPhase",
+    "PragmaActiveReset",
+    "InputSymbolic",
+    "PragmaStartDecompositionBlock",
+    "PragmaStopDecompositionBlock",
+    "PragmaConditional",
+]
 
 
 def mocked_call_circuit(
-        circuit: Circuit,
-        classical_bit_registers: Dict[str, List[bool]],
-        classical_float_registers: Dict[str, List[float]],
-        classical_complex_registers: Dict[str, List[complex]],
-        output_bit_register_dict: Dict[str, List[List[bool]]],
-        output_complex_register_dict: Dict[str, List[List[complex]]],
-        number_qubits: int = 1,
-        **kwargs) -> Tuple[
-            Dict[str, List[bool]],
-            Dict[str, List[float]],
-            Dict[str, List[complex]],
-            Dict[str, List[List[bool]]],
-            Dict[str, List[List[complex]]]]:
-    """Execute mocked qoqo circuit
+    circuit: Circuit,
+    classical_bit_registers: Dict[str, List[bool]],
+    classical_float_registers: Dict[str, List[float]],
+    classical_complex_registers: Dict[str, List[complex]],
+    output_bit_register_dict: Dict[str, List[List[bool]]],
+    output_complex_register_dict: Dict[str, List[List[complex]]],
+    number_qubits: int = 1,
+    **kwargs
+) -> Tuple[
+    Dict[str, List[bool]],
+    Dict[str, List[float]],
+    Dict[str, List[complex]],
+    Dict[str, List[List[bool]]],
+    Dict[str, List[List[complex]]],
+]:
+    """Execute mocked qoqo circuit.
 
     The Mocked interface is an interface which mock-simulates a quantum circuit. The quantum
     gates are not applied and the measurements produce random results coherent with the
     measured quantity.
 
     Args:
         circuit: The qoqo circuit that is executed
@@ -83,50 +81,57 @@
             Dict[str, List[float]],
             Dict[str, List[complex]],
             Dict[str, List[List[bool]]],
             Dict[str, List[List[complex]]]]: modified registers
 
     """
     for op in circuit:
-        (classical_bit_registers,
-         classical_float_registers,
-         classical_complex_registers,
-         output_bit_register_dict,
-         output_complex_register_dict) = mocked_call_operation(
-            op,
+        (
             classical_bit_registers,
             classical_float_registers,
             classical_complex_registers,
             output_bit_register_dict,
             output_complex_register_dict,
-            number_qubits,
-            **kwargs)
-
-    return (classical_bit_registers,
+        ) = mocked_call_operation(
+            op,
+            classical_bit_registers,
             classical_float_registers,
             classical_complex_registers,
             output_bit_register_dict,
-            output_complex_register_dict)
+            output_complex_register_dict,
+            number_qubits,
+            **kwargs
+        )
+
+    return (
+        classical_bit_registers,
+        classical_float_registers,
+        classical_complex_registers,
+        output_bit_register_dict,
+        output_complex_register_dict,
+    )
 
 
 def mocked_call_operation(
-        operation: Any,
-        classical_bit_registers: Dict[str, List[bool]],
-        classical_float_registers: Dict[str, List[float]],
-        classical_complex_registers: Dict[str, List[complex]],
-        output_bit_register_dict: Dict[str, List[List[bool]]],
-        output_complex_register_dict: Dict[str, List[List[complex]]],
-        number_qubits: int = 1,
-        **kwargs) -> Tuple[
-            Dict[str, List[bool]],
-            Dict[str, List[float]],
-            Dict[str, List[complex]],
-            Dict[str, List[List[bool]]],
-            Dict[str, List[List[complex]]]]:
-    """Execute mocked qoqo operation
+    operation: Any,
+    classical_bit_registers: Dict[str, List[bool]],
+    classical_float_registers: Dict[str, List[float]],
+    classical_complex_registers: Dict[str, List[complex]],
+    output_bit_register_dict: Dict[str, List[List[bool]]],
+    output_complex_register_dict: Dict[str, List[List[complex]]],
+    number_qubits: int = 1,
+    **kwargs
+) -> Tuple[
+    Dict[str, List[bool]],
+    Dict[str, List[float]],
+    Dict[str, List[complex]],
+    Dict[str, List[List[bool]]],
+    Dict[str, List[List[complex]]],
+]:
+    """Execute mocked qoqo operation.
 
     Args:
         operation: The qoqo operation that is executed
         classical_bit_registers: Dictionary or registers (lists) containing bit readout values
         classical_float_registers: Dictionary or registers (lists)
                                    containing float readout values
         classical_complex_registers: Dictionary or registers (lists)
@@ -142,67 +147,77 @@
         stuff
 
     Raises:
         RuntimeError: Operation cannot be mocked
 
     """
     tags = operation.tags()
-    if 'GateOperation' in tags:
+    if "GateOperation" in tags:
         pass
-    elif 'DefinitionFloat' in tags:
+    elif "DefinitionFloat" in tags:
         pass
-    elif 'DefinitionComplex' in tags:
+    elif "DefinitionComplex" in tags:
         pass
-    elif 'DefinitionBit' in tags:
+    elif "DefinitionBit" in tags:
         pass
-    elif 'DefinitionUsize' in tags:
+    elif "DefinitionUsize" in tags:
         pass
-    elif 'MeasureQubit' in tags:
+    elif "MeasureQubit" in tags:
         operation = cast(ops.MeasureQubit, operation)
         res = np.random.randint(0, 1)
         if operation.readout() not in classical_bit_registers.keys():
-            classical_bit_registers[operation.readout()] = [False for _ in range(number_qubits)]
+            classical_bit_registers[operation.readout()] = [
+                False for _ in range(number_qubits)
+            ]
         else:
             index = cast(int, operation.readout_index())
             classical_bit_registers[operation.readout()][index] = res  # type: ignore
-    elif 'PragmaRepeatedMeasurement' in tags:
+    elif "PragmaRepeatedMeasurement" in tags:
         operation = cast(ops.PragmaRepeatedMeasurement, operation)
         output_bit_register_dict[operation.readout()] = np.random.randint(
-            0, 2, size=(operation.number_measurements(), number_qubits)).tolist()
+            0, 2, size=(operation.number_measurements(), number_qubits)
+        ).tolist()
         if operation.readout() in classical_bit_registers.keys():
             del classical_bit_registers[operation.readout()]
-    elif 'PragmaGetPauliProduct' in tags:
+    elif "PragmaGetPauliProduct" in tags:
         operation = cast(ops.PragmaGetPauliProduct, operation)
-        classical_float_registers[operation.readout()] = [np.random.random(1).tolist(), ]
-    elif 'PragmaGetOccupationProbability' in tags:
+        classical_float_registers[operation.readout()] = [
+            np.random.random(1).tolist(),
+        ]
+    elif "PragmaGetOccupationProbability" in tags:
         operation = cast(ops.PragmaGetOccupationProbability, operation)
-        classical_float_registers[operation.readout()] = np.random.random(number_qubits).tolist()
-    elif 'PragmaGetStateVector' in tags:
+        classical_float_registers[operation.readout()] = np.random.random(
+            number_qubits
+        ).tolist()
+    elif "PragmaGetStateVector" in tags:
         operation = cast(ops.PragmaGetStateVector, operation)
         values = np.random.default_rng().uniform(0, 1, (2**number_qubits, 2))
         values_complex = values[..., 0] + 1j * values[..., 1]
         normalisation = 0
         for value in values_complex:
-            normalisation += abs(value)**2
+            normalisation += abs(value) ** 2
         values_normalised = values_complex / normalisation
         classical_complex_registers[operation.readout()] = values_normalised.tolist()
-    elif 'PragmaGetDensityMatrix' in tags:
+    elif "PragmaGetDensityMatrix" in tags:
         operation = cast(ops.PragmaGetDensityMatrix, operation)
         qubits = np.random.randint(0, 2, size=number_qubits)
         statevector = np.array([1])
         for qubit in qubits:
             if qubit == 0:
                 statevector = np.kron(np.array([1, 0]), statevector)
             else:
                 statevector = np.kron(np.array([0, 1]), statevector)
-        output_complex_register_dict[
-            operation.readout()] = np.kron(statevector[..., None], statevector).tolist()
+        output_complex_register_dict[operation.readout()] = np.kron(
+            statevector[..., None], statevector
+        ).tolist()
     elif any(pragma in tags for pragma in _ALLOWED_PRAGMAS):
         pass
     else:
         raise RuntimeError("Operation cannot be mocked")
 
-    return (classical_bit_registers,
-            classical_float_registers,
-            classical_complex_registers,
-            output_bit_register_dict,
-            output_complex_register_dict)
+    return (
+        classical_bit_registers,
+        classical_float_registers,
+        classical_complex_registers,
+        output_bit_register_dict,
+        output_complex_register_dict,
+    )
```

### Comparing `qoqo_mock-0.5.3/qoqo_mock.egg-info/PKG-INFO` & `qoqo_mock-0.5.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
-Name: qoqo-mock
-Version: 0.5.3
-Summary: Quantum Computing Base Package
-Home-page: https://quantumsimulations.de
-Author: HQS Quantum Simulations
-Author-email: info@quantumsimulations.de
+Name: qoqo_mock
+Version: 0.5.4
+Author-email: HQS Quantum Simulation GmbH <info@quantumsimulations.de>
 License: Apache-2.0
-Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: dev
 License-File: LICENSE
 
 <img src="qoqo_Logo_vertical_color.png" alt="qoqo logo" width="300" />
 
 # qoqo-mock
 
 Mocking backend for the qoqo/roqoqo quantum toolkit by [HQS Quantum Simulations](https://quantumsimulations.de).
@@ -49,12 +48,10 @@
 roqoqo circuits can be sent to the mock backend and all steps of a full hardware backend are applied, except calling actual quantum hardware. Measurements return random results.  
 This backend is designed purely for benchmarking purposes.
 
 ## General Notes
 
 This software is still in the beta stage. Functions and documentation are not yet complete and breaking changes can occur.
 
-This project is partly supported by [PlanQK](https://planqk.de).
-
 ## Contributing
 
 We welcome contributions to the project. If you want to contribute code, please have a look at CONTRIBUTE.md for our code contribution guidelines.
```

