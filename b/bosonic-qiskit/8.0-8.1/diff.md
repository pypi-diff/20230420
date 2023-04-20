# Comparing `tmp/bosonic-qiskit-8.0.tar.gz` & `tmp/bosonic-qiskit-8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bosonic-qiskit-8.0.tar", last modified: Wed Jan 18 19:53:00 2023, max compression
+gzip compressed data, was "bosonic-qiskit-8.1.tar", last modified: Thu Apr 20 20:03:55 2023, max compression
```

## Comparing `bosonic-qiskit-8.0.tar` & `bosonic-qiskit-8.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:53:00.471606 bosonic-qiskit-8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-01-18 19:53:00.471606 bosonic-qiskit-8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:53:00.467606 bosonic-qiskit-8.0/bosonic_qiskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-01-18 19:53:00.000000 bosonic-qiskit-8.0/bosonic_qiskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-01-18 19:53:00.000000 bosonic-qiskit-8.0/bosonic_qiskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 19:53:00.000000 bosonic-qiskit-8.0/bosonic_qiskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-18 19:53:00.000000 bosonic-qiskit-8.0/bosonic_qiskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-18 19:53:00.000000 bosonic-qiskit-8.0/bosonic_qiskit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:53:00.467606 bosonic-qiskit-8.0/c2qa/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/c2qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/c2qa/animate.py
--rw-r--r--   0 runner    (1001) docker     (123)    25567 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/c2qa/circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/c2qa/kraus.py
--rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/c2qa/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/c2qa/qumoderegister.py
--rw-r--r--   0 runner    (1001) docker     (123)    14897 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/c2qa/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/c2qa/wigner.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-18 19:53:00.471606 bosonic-qiskit-8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 19:53:00.471606 bosonic-qiskit-8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/tests/test_animate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/tests/test_inconsistent_statevectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    19881 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/tests/test_noise_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/tests/test_parameterized.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/tests/test_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/tests/test_qumoderegister.py
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-01-18 19:52:50.000000 bosonic-qiskit-8.0/tests/test_wigner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:03:55.482550 bosonic-qiskit-8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-20 20:03:55.482550 bosonic-qiskit-8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:03:55.478551 bosonic-qiskit-8.1/bosonic_qiskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-20 20:03:55.000000 bosonic-qiskit-8.1/bosonic_qiskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-20 20:03:55.000000 bosonic-qiskit-8.1/bosonic_qiskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:03:55.000000 bosonic-qiskit-8.1/bosonic_qiskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 20:03:55.000000 bosonic-qiskit-8.1/bosonic_qiskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 20:03:55.000000 bosonic-qiskit-8.1/bosonic_qiskit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:03:55.482550 bosonic-qiskit-8.1/c2qa/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/animate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27351 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/kraus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/parameterized_unitary_gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/qumoderegister.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/c2qa/wigner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 20:03:55.482550 bosonic-qiskit-8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:03:55.482550 bosonic-qiskit-8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_animate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_inconsistent_statevectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_noise_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_parameterized.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_qumoderegister.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-20 20:03:39.000000 bosonic-qiskit-8.1/tests/test_wigner.py
```

### Comparing `bosonic-qiskit-8.0/LICENSE` & `bosonic-qiskit-8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.0/README.md` & `bosonic-qiskit-8.1/README.md`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.0/bosonic_qiskit.egg-info/SOURCES.txt` & `bosonic-qiskit-8.1/bosonic_qiskit.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 bosonic_qiskit.egg-info/requires.txt
 bosonic_qiskit.egg-info/top_level.txt
 c2qa/__init__.py
 c2qa/animate.py
 c2qa/circuit.py
 c2qa/kraus.py
 c2qa/operators.py
+c2qa/parameterized_unitary_gate.py
 c2qa/qumoderegister.py
 c2qa/util.py
 c2qa/wigner.py
 tests/__init__.py
 tests/test_animate.py
 tests/test_circuit.py
 tests/test_gates.py
```

### Comparing `bosonic-qiskit-8.0/c2qa/animate.py` & `bosonic-qiskit-8.1/c2qa/animate.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import matplotlib.animation
 import matplotlib.pyplot as plt
 import numpy
 import qiskit
 
 
 from c2qa.circuit import CVCircuit
-from c2qa.operators import ParameterizedUnitaryGate
+from c2qa.parameterized_unitary_gate import ParameterizedUnitaryGate
 from c2qa.wigner import simulate_wigner
 
 
 def animate_wigner(
     circuit: CVCircuit,
     qubit: qiskit.circuit.quantumcircuit.QubitSpecifier = None,
     cbit: qiskit.circuit.quantumcircuit.ClbitSpecifier = None,
@@ -28,14 +28,15 @@
     axes_steps: int = 200,
     processes: int = None,
     keep_state: bool = True,
     noise_passes = None,
     sequential_subcircuit: bool = False,
     draw_grid: bool = False,
     trace: bool = True,
+    bitrate: int = -1
 ):
     """Animate the Wigner function at each step defined in the given CVCirctuit.
 
     This assumes the CVCircuit was simulated with an animation_segments > 0 to
     act as the frames of the generated movie.
 
     The ffmpeg binary must be on your system PATH in order to execute this
@@ -119,15 +120,15 @@
         fargs=(fig, ax, xvec, w_fock, file, draw_grid),
         interval=200,
         repeat=True,
     )
 
     # Save to file using ffmpeg, Pillow (GIF, APNG), or display
     if file:
-        save_animation(anim, file)
+        save_animation(anim, file, bitrate)
 
     return anim
 
 
 def __animate_circuit(circuit, animation_segments, keep_state, qubit, cbit, sequential_subcircuit):
     sim_circuits = []  # Each frame will have its own circuit to simulate
 
@@ -322,26 +323,26 @@
 
     for _ in range(animation_segments):
         frames.append(inst)
 
     return frames
 
 
-def save_animation(anim: matplotlib.animation.FuncAnimation, file: str):
+def save_animation(anim: matplotlib.animation.FuncAnimation, file: str, bitrate: int):
     file_path = pathlib.Path(file)
 
     if file_path.suffix == ".mp4":
-        writer = matplotlib.animation.FFMpegWriter(fps=24)
+        writer = matplotlib.animation.FFMpegWriter(fps=24, bitrate=bitrate)
     elif file_path.suffix == ".gif" or file_path.suffix == ".apng":
-        writer = matplotlib.animation.PillowWriter(fps=24)
+        writer = matplotlib.animation.PillowWriter(fps=24, bitrate=bitrate)
     else:
         print(
             f"Unknown animation file type {file_path.suffix}, defaulting to using PillowWriter"
         )
-        writer = matplotlib.animation.PillowWriter(fps=24)
+        writer = matplotlib.animation.PillowWriter(fps=24, bitrate=bitrate)
 
     anim.save(file, writer=writer)
 
 
 def _animate_init():
     pass  # Prevent rendering frame 0 twice (once for init, once for animate)
 
@@ -362,19 +363,19 @@
         abs_max = 5
     color_levels = numpy.linspace(-abs_max, abs_max, 100)
 
     xvec_int = [int(x) for x in xvec]
     xvec_int = sorted(set(xvec_int))
 
     ax.clear()
-    cont = ax.contourf(xvec, xvec, w_fock, color_levels, cmap="RdBu_r")
+    cont = ax.contourf(xvec, xvec, w_fock, color_levels, cmap="RdBu")
 
-    ax.set_xlabel("x")
+    ax.set_xlabel(r"$x$")
     ax.set_xticks(xvec_int)
-    ax.set_ylabel("p")
+    ax.set_ylabel(r"$p$")
     ax.set_yticks(xvec_int)
     if draw_grid:
         ax.grid()
 
     if frame == 0:
         fig.colorbar(cont, ax=ax)
```

### Comparing `bosonic-qiskit-8.0/c2qa/circuit.py` & `bosonic-qiskit-8.1/c2qa/circuit.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import warnings
 
 import numpy as np
 from qiskit import QuantumCircuit, QuantumRegister
 from qiskit.circuit.parametertable import ParameterTable
 import qiskit.providers.aer.library.save_instructions as save
 
-from c2qa.operators import CVOperators, ParameterizedUnitaryGate
+from c2qa.operators import CVOperators
+from c2qa.parameterized_unitary_gate import ParameterizedUnitaryGate
 from c2qa.qumoderegister import QumodeRegister
 
 
 class CVCircuit(QuantumCircuit):
     """Extension of QisKit QuantumCircuit to add continuous variable (bosonic) gate support to simulations."""
 
     def __init__(self, *regs, name: str = None, probe_measure: bool = False):
@@ -384,15 +385,15 @@
                 duration=duration,
                 unit=unit
             ),
             qargs=qumode_a + qumode_b,
         )
 
     def cv_c_r(self, theta, qumode, qubit, duration=100, unit="ns"):
-        """Qubit dependent phase-space rotation gate.
+        """Qubit dependent phase-space rotation gate (i.e., dispersive interaction).
 
         Args:
             theta (real): phase
             qumode_a (list): list of qubits representing qumode
             qubit_ancilla (qubit): QisKit control qubit
 
         Returns:
@@ -569,14 +570,39 @@
         else:
             self.append(
                 ParameterizedUnitaryGate(
                     self.ops.csnap, [theta, n], num_qubits=len(qumode) + 1, label="cSNAP", duration=duration, unit=unit
                 ),
                 qargs=qumode + [qubit],
             )
+            
+    def cv_multisnap(self, thetas, ns, qumode, duration=1, unit="us"):
+        params = thetas + ns
+        self.append(
+            ParameterizedUnitaryGate(
+                self.ops.multisnap, params, num_qubits=len(qumode), label="mSNAP", duration=duration, unit=unit
+            ),
+            qargs=qumode,
+        )
+            
+    def cv_c_multiboson_sampling(self, max, qumode, qubit=None, duration=1, unit="us"):
+        """SNAP (Selective Number-dependent Arbitrary Phase) gates for multiboson sampling.
+        Args:
+            max (int): the period of the mapping
+            qumode (list): list of qubits representing qumode
+            qubit (Qubit): control qubit.
+        Returns:
+            Instruction: QisKit instruction
+        """
+        self.append(
+            ParameterizedUnitaryGate(
+                self.ops.c_multiboson_sampling, [max], num_qubits=len(qumode) + 1, label="c_multiboson_sampling", duration=duration, unit=unit
+            ),
+            qargs=qumode + [qubit],
+        )
 
     def cv_eswap(self, theta, qumode_a, qumode_b, duration=100, unit="ns"):
         """Exponential SWAP gate.
 
         Args:
             theta (real): phase
             qumode_a (list): list of qubits representing qumode
@@ -715,7 +741,23 @@
         # If not, only use those needed (starting with least significant bit).
         # This piece is useful so that the user doesn't need to think about
         # how many bits are needed to read out a list of qumodes, qubits, etc.
         if len(flat_list) < len(cbit_list):
             self.measure(flat_list, cbit_list[0:len(flat_list)])
         else:
             self.measure(flat_list, cbit_list)
+
+    def cv_c_multiboson_sampling(self, max, qumode, qubit, duration=1, unit="us"):
+        """SNAP (Selective Number-dependent Arbitrary Phase) gates for multiboson sampling.
+        Args:
+            max (int): the period of the mapping
+            qumode (list): list of qubits representing qumode
+            qubit (Qubit): control qubit.
+        Returns:
+            Instruction: QisKit instruction
+        """
+        self.append(
+            ParameterizedUnitaryGate(
+                self.ops.c_multiboson_sampling, [max], num_qubits=len(qumode) + 1, label="c_multiboson_sampling", duration=duration, unit=unit
+            ),
+            qargs=qumode + [qubit],
+        )
```

### Comparing `bosonic-qiskit-8.0/c2qa/kraus.py` & `bosonic-qiskit-8.1/c2qa/kraus.py`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.0/c2qa/qumoderegister.py` & `bosonic-qiskit-8.1/c2qa/qumoderegister.py`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.0/c2qa/util.py` & `bosonic-qiskit-8.1/c2qa/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,72 @@
 import qiskit
 import qiskit.quantum_info
 from qiskit.quantum_info import Statevector
 
 
 from c2qa import CVCircuit
 
+def flatten(l):
+    return [item for sublist in l for item in sublist]
+
+def cv_multiboson_sampling(circuit,list_qumodes_to_sample:list, qmr_number:int=0):
+    # Count number of qubits in circuit so far
+    num_qubits = len(flatten(circuit._qubit_regs))
+    # Collect qumode register from circuit
+    qmr = circuit.qmregs[qmr_number]
+    # Add one ancilla qubits to the circuit per qumode to measure
+    qbr_extra = qiskit.QuantumRegister(size=len(list_qumodes_to_sample), name="qbr_sampling")
+    # Add classical bits to readout measurement results
+    cbr_extra = qiskit.ClassicalRegister(len(list_qumodes_to_sample)*circuit.num_qubits_per_qumode, name="cbr_sampling")
+    circuit.add_register(qbr_extra,cbr_extra)
+    # Iterate over the qumodes
+    qumode_counter=0
+    for j in list_qumodes_to_sample:
+        # Set the initial maximum Fock state
+        max = circuit.cutoff
+        # Iterate a number of time corresponding to the number of bits required to represent the maximum Fock state in binary (remove useless characters at the front)
+        for iteration in range(len(bin(circuit.cutoff))-3):
+            # Make sure the ancilla qubit is always reset to 0
+            circuit.initialize('0',qbr_extra[qumode_counter])
+            # Apply a circuit which flips the ancilla if the qumode occupation is odd etc. see (Curtis et al., PRA, 2021 and Wang et al.,  PRX, 2020)
+            circuit.cv_c_multiboson_sampling(max,qmr[list_qumodes_to_sample[j]],qbr_extra[qumode_counter])
+            # Measure the qubit onto the classical bits (from left to right)
+            classical_bit=circuit.num_qubits_per_qumode-1-iteration+(qumode_counter*circuit.num_qubits_per_qumode)
+            circuit.measure(qbr_extra[qumode_counter],classical_bit)
+            # Update the maximum value for the SNAP gate creation
+            max = int(max/2)
+        circuit.barrier()
+        qumode_counter+=1
+    # Simulate circuit with a single shot
+    _, result = simulate(circuit, shots=1)
+    # Return integer value of boson number occupation, converted from the bits which make up a binary number
+    print(result.get_counts())
+    full_set_of_binary = list(result.get_counts().keys())[0].encode('ascii')
+    results_integers = np.zeros([len(list_qumodes_to_sample)])
+    for j in range(len(list_qumodes_to_sample)):
+        binary_number = full_set_of_binary[j*circuit.num_qubits_per_qumode:((j+1)*circuit.num_qubits_per_qumode)]
+        print(binary_number)
+        results_integers[-(j+1)] = int(binary_number,2)
+    return results_integers
 
 def stateread(
     stateop, numberofqubits, numberofmodes, cutoff, verbose=True, little_endian=False
 ):
     """Print values for states of qubits and qumodes using the result of a
     simulation of the statevector, e.g. using stateop, _ = c2qa.util.simulate(circuit).
 
     Returns the states of the qubits and the Fock states of the qumodes with respective amplitudes.
     """
     st = np.array(stateop)  # convert state to np.array
     amp_cv = []
     amp_qb = []
     state = []
 
+    cutoff = 2**int(np.ceil(np.log2(cutoff))) # The cutoff needs to be a power of 2 for this code to work
+
     for i in range(len(st)):
         res = st[
             i
         ]  # go through vector element by element and find the positions of the non-zero elements with next if clause
         if np.abs(res) > 1e-10:
             pos = i  # position of amplitude (non-zero real)
             # print("position of non-zero real amplitude: ", pos, " res = ", res)
@@ -125,16 +169,16 @@
     occupation_cv = [sum(i) for i in zip(*amp_cv)]
     occupation_qb = [sum(i) for i in zip(*amp_qb)]
 
     if not little_endian:
         for i in range(len(state)):
             state[i][0] = state[i][0][::-1]
             state[i][1] = state[i][1][::-1]
-            occupation_cv = occupation_cv[::-1]
-            occupation_qb = occupation_qb[::-1]
+        occupation_cv = occupation_cv[::-1]
+        occupation_qb = occupation_qb[::-1]
 
     return [occupation_cv, occupation_qb], state
 
 
 def cv_fockcounts(counts, qubit_qumode_list, reverse_endianness=False):
     """Convert counts dictionary from Fock-basis binary representation into
     base-10 Fock basis (qubit measurements are left unchanged). Accepts a counts
```

### Comparing `bosonic-qiskit-8.0/c2qa/wigner.py` & `bosonic-qiskit-8.1/c2qa/wigner.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,15 @@
     trace: bool = True,
     file: str = None,
     axes_min: int = -6,
     axes_max: int = 6,
     axes_steps: int = 200,
     num_colors: int = 100,
     draw_grid: bool = False,
+    dpi: int = 100
 ):
     """Produce a Matplotlib figure for the Wigner function on the given state vector.
 
     Optionally perform partial trace.
 
     Args:
         circuit (CVCircuit): circuit with results to trace (to find Qubit index)
@@ -211,25 +212,27 @@
         data=w_fock,
         axes_min=axes_min,
         axes_max=axes_max,
         axes_steps=axes_steps,
         file=file,
         num_colors=num_colors,
         draw_grid=draw_grid,
+        dpi = dpi
     )
 
 
 def plot(
     data,
     axes_min: int = -6,
     axes_max: int = 6,
     axes_steps: int = 200,
     file: str = None,
     num_colors: int = 100,
     draw_grid: bool = False,
+    dpi = 100
 ):
     """Contour plot the given data array"""
     xvec = np.linspace(axes_min, axes_max, axes_steps)
 
     amax = np.amax(data)
     amin = np.amin(data)
     if amax == 0 and amin == 0:
@@ -252,15 +255,15 @@
         ax.grid()
 
 
     cb = fig.colorbar(cont, ax=ax, format=tick.FormatStrFormatter('%.2f'))
     cb.set_label(r"$W(x,p)$",rotation=270,labelpad=25)
 
     if file:
-        plt.savefig(file)
+        plt.savefig(file, dpi=dpi)
     else:
         plt.show()
 
 
 def plot_wigner_projection(circuit: CVCircuit, qubit, file: str = None, draw_grid: bool = False):
     """Plot the projection onto 0, 1, +, - for the given circuit.
```

### Comparing `bosonic-qiskit-8.0/setup.py` & `bosonic-qiskit-8.1/setup.py`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.0/tests/test_animate.py` & `bosonic-qiskit-8.1/tests/test_animate.py`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.0/tests/test_circuit.py` & `bosonic-qiskit-8.1/tests/test_parameterized.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,104 @@
+from pathlib import Path
+
+
 import c2qa
-import pytest
-import qiskit
 import numpy
+import qiskit
 
 
-def test_no_registers():
-    with pytest.raises(ValueError):
-        c2qa.CVCircuit()
+def assert_changed(state, result):
+    assert result.success
+    # print()
+    # print(circuit.draw("text"))
+    # print(state)
 
+    # TODO - better understand what the state vector results should be
+    assert count_nonzero(state) > 1
 
-def test_only_quantumregister():
-    with pytest.raises(ValueError):
-        qr = qiskit.QuantumRegister(1)
-        c2qa.CVCircuit(qr)
 
+def count_nonzero(statevector: qiskit.quantum_info.Statevector):
+    """Re-implement numpy.count_nonzero using numpy.isclose()."""
+    nonzero = len(statevector.data)
+    for state in statevector.data:
+        if numpy.isclose(state, 0):
+            nonzero -= 1
 
-def test_only_qumoderegister():
-    c2qa.CVCircuit(c2qa.QumodeRegister(1, 1))
+    return nonzero
 
 
-def test_multiple_qumoderegisters():
-    with pytest.warns(UserWarning):
-        c2qa.CVCircuit(c2qa.QumodeRegister(1, 1), c2qa.QumodeRegister(1, 1))
+def create_conditional(num_qumodes: int = 2, num_qubits_per_qumode: int = 2):
+    qmr = c2qa.QumodeRegister(num_qumodes, num_qubits_per_qumode)
+    qr = qiskit.QuantumRegister(2)
+    circuit = c2qa.CVCircuit(qmr, qr)
 
+    for qumode in range(num_qumodes):
+        circuit.cv_initialize(0, qmr[qumode])
 
-def test_correct():
-    c2qa.CVCircuit(qiskit.QuantumRegister(1), c2qa.QumodeRegister(1, 1))
+    circuit.initialize([0, 1], qr[1])  # qr[0] will init to zero
 
+    return circuit, qmr, qr
 
-def test_with_classical():
-    c2qa.CVCircuit(
-        qiskit.QuantumRegister(1),
-        c2qa.QumodeRegister(1, 1),
-        qiskit.ClassicalRegister(1),
-    )
 
+def test_parameterized_displacement(capsys):
+    with capsys.disabled():
+        circuit, qmr, qr = create_conditional()
 
-def test_with_initialize():
-    number_of_modes = 5
-    number_of_qubits = number_of_modes
-    number_of_qubits_per_mode = 2
+        alpha = qiskit.circuit.Parameter("alpha")
+        circuit.cv_d(alpha, qmr[0])
 
-    qmr = c2qa.QumodeRegister(
-        num_qumodes=number_of_modes, num_qubits_per_qumode=number_of_qubits_per_mode
-    )
-    qbr = qiskit.QuantumRegister(size=number_of_qubits)
-    cbr = qiskit.ClassicalRegister(size=1)
-    circuit = c2qa.CVCircuit(qmr, qbr, cbr)
+        bound_circuit = circuit.bind_parameters({alpha: 3.14})
 
-    sm = [0, 0, 1, 0, 0]
-    for i in range(qmr.num_qumodes):
-        circuit.cv_initialize(sm[i], qmr[i])
+        state, result = c2qa.util.simulate(bound_circuit)
+        assert_changed(state, result)
 
-    circuit.initialize(numpy.array([0, 1]), qbr[0])
 
-    state, result = c2qa.util.simulate(circuit)
-    assert result.success
+def test_complex_literals(capsys):
+    with capsys.disabled():
+        # a = qiskit.circuit.Parameter('𝛼')
+
+        qmr = c2qa.QumodeRegister(1, num_qubits_per_qumode=4)
+        qbr = qiskit.QuantumRegister(1)
+
+        minimal_circuit = c2qa.CVCircuit(qmr, qbr)
+
+        minimal_circuit.h(qbr[0])
 
+        minimal_circuit.cv_c_d(1j * 1, qmr[0], qbr[0])
 
-def test_with_delay(capsys):
+        # bound_circuit = minimal_circuit.bind_parameters({a: 1})
+
+        c2qa.util.simulate(minimal_circuit)
+
+
+def test_complex_parameters(capsys):
     with capsys.disabled():
-        number_of_modes = 1
-        number_of_qubits = 1
-        number_of_qubits_per_mode = 2
+        a = qiskit.circuit.Parameter("𝛼")
+
+        qmr = c2qa.QumodeRegister(1, num_qubits_per_qumode=4)
+        qbr = qiskit.QuantumRegister(1)
+
+        minimal_circuit = c2qa.CVCircuit(qmr, qbr)
 
-        qmr = c2qa.QumodeRegister(
-            num_qumodes=number_of_modes, num_qubits_per_qumode=number_of_qubits_per_mode
-        )
-        qbr = qiskit.QuantumRegister(size=number_of_qubits)
-        circuit = c2qa.CVCircuit(qmr, qbr)
+        minimal_circuit.h(qbr[0])
 
-        circuit.delay(100)
-        circuit.cv_d(1, qmr[0])
+        minimal_circuit.cv_c_d(1j * a, qmr[0], qbr[0])
 
-        state, result = c2qa.util.simulate(circuit)
-        assert result.success
+        bound_circuit = minimal_circuit.bind_parameters({a: 1})
+        c2qa.util.simulate(bound_circuit)
 
 
-def test_get_qubit_indices(capsys):
+def test_complex_parameters_float(capsys):
     with capsys.disabled():
-        number_of_modes = 2
-        number_of_qubits = 2
-        number_of_qubits_per_mode = 2
-
-        qmr = c2qa.QumodeRegister(
-            num_qumodes=number_of_modes, num_qubits_per_qumode=number_of_qubits_per_mode
-        )
-        qbr = qiskit.QuantumRegister(size=number_of_qubits)
-        cbr = qiskit.ClassicalRegister(size=1)
-        circuit = c2qa.CVCircuit(qmr, qbr, cbr)  
-
-        indices = circuit.get_qubit_indices([qmr[1]])
-        print(f"qmr[1] indices = {indices}")
-        assert indices == [2, 3]
-
-        indices = circuit.get_qubit_indices([qmr[0]])
-        print(f"qmr[0] indices = {indices}")
-        assert indices == [0, 1]
-
-        indices = circuit.get_qubit_indices([qbr[1]])
-        print(f"qbr[1] indices = {indices}")
-        assert indices == [5]
-
-        indices = circuit.get_qubit_indices([qbr[0]])
-        print(f"qbr[0] indices = {indices}")
-        assert indices == [4]
+        a = qiskit.circuit.Parameter("𝛼")
+
+        qmr = c2qa.QumodeRegister(1, num_qubits_per_qumode=4)
+        qbr = qiskit.QuantumRegister(1)
+
+        minimal_circuit = c2qa.CVCircuit(qmr, qbr)
+
+        minimal_circuit.h(qbr[0])
+
+        minimal_circuit.cv_c_d(1j * a, qmr[0], qbr[0])
+
+        bound_circuit = minimal_circuit.bind_parameters({a: 2})
+        c2qa.util.simulate(bound_circuit)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bosonic-qiskit-8.0/tests/test_gates.py` & `bosonic-qiskit-8.1/tests/test_gates.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,7 +350,21 @@
 def test_eswap():
     circuit, qmr = create_unconditional()
 
     phi = random.random()
     circuit.cv_eswap(phi, qmr[0], qmr[1])
 
     state, result = c2qa.util.simulate(circuit)
+
+def test_multiboson_sampling(capsys):
+    with capsys.disabled():
+        num_qubits=1
+        num_qumodes=2
+        num_qubits_per_qumode=2
+        qmrA = c2qa.QumodeRegister(num_qumodes = num_qumodes, num_qubits_per_qumode = num_qubits_per_qumode,name="qmrA_initial")
+        qmrB = c2qa.QumodeRegister(num_qumodes = num_qumodes, num_qubits_per_qumode = num_qubits_per_qumode,name="qmrB_initial")
+        qbr = qiskit.QuantumRegister(size=num_qubits,name='qbr_initial')
+        circuit = c2qa.CVCircuit(qmrA, qmrB, qbr)
+        circuit.cv_c_multiboson_sampling([0,1,2,3], qmrA[0], qbr[0])
+
+        state, result = c2qa.util.simulate(circuit)
+        assert result.success
```

### Comparing `bosonic-qiskit-8.0/tests/test_inconsistent_statevectors.py` & `bosonic-qiskit-8.1/tests/test_inconsistent_statevectors.py`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.0/tests/test_noise_model.py` & `bosonic-qiskit-8.1/tests/test_noise_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import numpy as np
 
 
 import qiskit
 import qiskit.providers.aer.noise as noise
 from qiskit.providers.aer.noise.noiseerror import NoiseError
 from qiskit.providers.aer.noise.passes.relaxation_noise_pass import RelaxationNoisePass
+from qiskit.tools.visualization import plot_histogram
 
 
 def test_noise_model(capsys):
     with capsys.disabled():
         num_qumodes = 1
         num_qubits_per_qumode = 2
         qmr = c2qa.QumodeRegister(num_qumodes, num_qubits_per_qumode)
@@ -559,8 +560,45 @@
         filename = "tests/test_relaxation_and_photon_loss_noise_passes.gif"
         c2qa.animate.animate_wigner(
             circuit,
             animation_segments=200,
             file=filename,
             noise_passes=noise_passes,
         )
-        assert Path(filename).is_file()
+        assert Path(filename).is_file()
+
+
+def test_multi_qumode_loss_probability(capsys):
+    with capsys.disabled():
+        num_qumodes = 2
+        num_qubits_per_qumode = 2
+        qmr = c2qa.QumodeRegister(num_qumodes, num_qubits_per_qumode)
+        circuit = c2qa.CVCircuit(qmr)
+
+        circuit.cv_initialize(1, qmr[0])
+        circuit.cv_initialize(1, qmr[1])
+        circuit.cv_bs(np.pi/4, qmr[0], qmr[1], duration=100, unit="ns")
+        circuit.cv_bs(-np.pi/4, qmr[0], qmr[1], duration=100, unit="ns")
+
+        photon_loss_rate = 10000000
+        noise_pass = c2qa.kraus.PhotonLossNoisePass(photon_loss_rate, circuit)
+
+        fity_fifty = False
+        print()
+        for i in range(20):
+            print("----------------------")
+            print(f"Iteration {i}")
+            state_vector, result = c2qa.util.simulate(circuit, noise_passes=noise_pass)
+            # plot_histogram(result.get_counts(circuit), filename=f"tests/test_manual_validate_beamsplitter-{i}.png")
+            occupation, fock_states = c2qa.util.stateread(state_vector, 0, num_qumodes, 2**num_qubits_per_qumode,verbose=True)
+
+            for qumode_state, qubit_state, amplitude in fock_states:
+                # print(f"{qumode_state} {qubit_state} {amplitude}")
+                qumode1 = qumode_state[0]
+                qumode2 = qumode_state[1]
+                probability = amplitude**2
+
+                if (qumode1 == 1 and qumode2 == 0) or (qumode1 == 0 and qumode1 == 1) and probability == 0.5:
+                    fity_fifty = True
+            
+        assert fity_fifty
+
```

### Comparing `bosonic-qiskit-8.0/tests/test_operators.py` & `bosonic-qiskit-8.1/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.0/tests/test_qiskit.py` & `bosonic-qiskit-8.1/tests/test_qiskit.py`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.0/tests/test_util.py` & `bosonic-qiskit-8.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `bosonic-qiskit-8.0/tests/test_wigner.py` & `bosonic-qiskit-8.1/tests/test_wigner.py`

 * *Files identical despite different names*

