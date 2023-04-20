# Comparing `tmp/multirotor-0.2.4.tar.gz` & `tmp/multirotor-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multirotor-0.2.4.tar", last modified: Sat Sep 17 22:07:53 2022, max compression
+gzip compressed data, was "multirotor-0.3.1.tar", last modified: Thu Apr 20 20:46:32 2023, max compression
```

## Comparing `multirotor-0.2.4.tar` & `multirotor-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2022-09-17 22:07:53.381185 multirotor-0.2.4/
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     1079 2022-09-17 22:07:53.381185 multirotor-0.2.4/PKG-INFO
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      823 2022-09-06 21:25:06.000000 multirotor-0.2.4/README.md
-drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2022-09-17 22:07:53.381185 multirotor-0.2.4/multirotor/
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)        0 2022-09-06 21:25:06.000000 multirotor-0.2.4/multirotor/__init__.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     8436 2022-09-17 21:59:05.000000 multirotor-0.2.4/multirotor/controller.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     2488 2022-09-06 21:25:06.000000 multirotor-0.2.4/multirotor/coords.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     2399 2022-09-06 21:25:06.000000 multirotor-0.2.4/multirotor/env.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    11113 2022-09-17 21:59:27.000000 multirotor-0.2.4/multirotor/helpers.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     6286 2022-09-06 21:25:06.000000 multirotor-0.2.4/multirotor/physics.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    19090 2022-09-09 17:19:35.000000 multirotor-0.2.4/multirotor/simulation.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     4403 2022-09-06 21:25:06.000000 multirotor-0.2.4/multirotor/trajectories.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     4757 2022-09-09 17:18:19.000000 multirotor-0.2.4/multirotor/vehicle.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     8591 2022-09-06 21:25:06.000000 multirotor-0.2.4/multirotor/visualize.py
-drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2022-09-17 22:07:53.381185 multirotor-0.2.4/multirotor.egg-info/
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     1079 2022-09-17 22:07:53.000000 multirotor-0.2.4/multirotor.egg-info/PKG-INFO
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      432 2022-09-17 22:07:53.000000 multirotor-0.2.4/multirotor.egg-info/SOURCES.txt
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)        1 2022-09-17 22:07:53.000000 multirotor-0.2.4/multirotor.egg-info/dependency_links.txt
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      102 2022-09-17 22:07:53.000000 multirotor-0.2.4/multirotor.egg-info/requires.txt
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)       11 2022-09-17 22:07:53.000000 multirotor-0.2.4/multirotor.egg-info/top_level.txt
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)       81 2022-09-06 21:25:06.000000 multirotor-0.2.4/pyproject.toml
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      486 2022-09-17 22:07:53.381185 multirotor-0.2.4/setup.cfg
+drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2023-04-20 20:46:32.349427 multirotor-0.3.1/
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     1079 2023-04-20 20:46:32.349427 multirotor-0.3.1/PKG-INFO
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      823 2022-09-06 21:25:06.000000 multirotor-0.3.1/README.md
+drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2023-04-20 20:46:32.349427 multirotor-0.3.1/multirotor/
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)        0 2022-09-06 21:25:06.000000 multirotor-0.3.1/multirotor/__init__.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     2484 2022-12-12 19:19:30.000000 multirotor-0.3.1/multirotor/coords.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     5515 2022-10-31 21:18:20.000000 multirotor-0.3.1/multirotor/env.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    16306 2023-04-11 13:43:29.000000 multirotor-0.3.1/multirotor/helpers.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     6548 2022-12-08 18:45:12.000000 multirotor-0.3.1/multirotor/physics.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    22647 2023-04-20 20:03:48.000000 multirotor-0.3.1/multirotor/simulation.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     9247 2023-03-18 19:01:32.000000 multirotor-0.3.1/multirotor/trajectories.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     5418 2023-04-11 13:45:56.000000 multirotor-0.3.1/multirotor/vehicle.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    12609 2023-04-07 17:31:02.000000 multirotor-0.3.1/multirotor/visualize.py
+drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2023-04-20 20:46:32.349427 multirotor-0.3.1/multirotor.egg-info/
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     1079 2023-04-20 20:46:32.000000 multirotor-0.3.1/multirotor.egg-info/PKG-INFO
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      407 2023-04-20 20:46:32.000000 multirotor-0.3.1/multirotor.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)        1 2023-04-20 20:46:32.000000 multirotor-0.3.1/multirotor.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      102 2023-04-20 20:46:32.000000 multirotor-0.3.1/multirotor.egg-info/requires.txt
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)       11 2023-04-20 20:46:32.000000 multirotor-0.3.1/multirotor.egg-info/top_level.txt
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)       81 2022-09-06 21:25:06.000000 multirotor-0.3.1/pyproject.toml
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      486 2023-04-20 20:46:32.353427 multirotor-0.3.1/setup.cfg
```

### Comparing `multirotor-0.2.4/PKG-INFO` & `multirotor-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multirotor
-Version: 0.2.4
+Version: 0.3.1
 Summary: Simulation testbed for multirotor vehicles.
 Keywords: multirotor,simulation,gym,uav
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: DEV
 Provides-Extra: CONTROL
```

### Comparing `multirotor-0.2.4/README.md` & `multirotor-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `multirotor-0.2.4/multirotor/coords.py` & `multirotor-0.3.1/multirotor/coords.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 @njit
 def angular_to_euler_rate(
     angular_velocity: np.ndarray, orientation: np.ndarray
 ) -> np.ndarray:
     roll, pitch, yaw = orientation
     p, q, r = angular_velocity
-    roll_rate = p + q * tan(pitch) * (q * sin(roll) + r * cos(roll))
+    roll_rate = p + tan(pitch) * (q * sin(roll) + r * cos(roll))
     pitch_rate = q * cos(roll) - r * sin(roll)
     yaw_rate = (q * sin(roll) + r * cos(roll)) / cos(pitch)
     return np.asarray([roll_rate, pitch_rate, yaw_rate])
 
 
 
 @njit
```

### Comparing `multirotor-0.2.4/multirotor/physics.py` & `multirotor-0.3.1/multirotor/physics.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,17 +58,19 @@
     """
     Calculates the torque acting on the three body axes (roll, pitch, yaw), due 
     to a single propeller.
 
     Parameters
     ----------
     position_vector : np.ndarray
-        Position vector of force, relative to center of mass.
+        Position vector of force, relative to center of mass. If multiple vectors,
+        should be in shape 3 x n_vectors.
     force : np.ndarray
-        Force vector acting at that position (nominally thrust).
+        Force vector acting at that position (nominally thrust). If multiple vectors,
+        should be in shape 3 x n_vectors.
     moment_of_inertia : float
         Moment of inertia of the body.
     prop_angular_acceleration : float
         Angular acceleration experienced by propeller.
     drag_coefficient : float
         The drag coefficient of propeller.
     prop_angular_velocity : float
@@ -83,20 +85,22 @@
     """
     # TODO: See here
     # https://andrew.gibiansky.com/downloads/pdf/Quadcopter%20Dynamics,%20Simulation,%20and%20Control.pdf
     # Total moments in the body frame
     # yaw moments
     # tau = I . d omega/dt
     tau_rot = (
+        # angular acceleration of propellers is assumed to be negligible
         # clockwise * moment_of_inertia * prop_angular_acceleration + 
         clockwise * drag_coefficient * prop_angular_velocity**2
     )
     # tau = r x F
-    tau = np.cross(position_vector, force)
-    # print(moment_of_inertia, prop_angular_acceleration)
+    # numba does not support axis arguments for cross(), so taking transpose and
+    # then undoing it for result:
+    tau = np.cross(position_vector.T, force.T).T
     tau[2] = tau[2] + tau_rot
     return tau
 
 
 
 @njit
 def apply_forces_torques(
```

### Comparing `multirotor-0.2.4/multirotor/simulation.py` & `multirotor-0.3.1/multirotor/simulation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Callable, List, Tuple
 from copy import deepcopy
 
 import numpy as np
-from numpy import (cos, sin)
 from scipy.integrate import odeint, trapezoid
 
 from .vehicle import MotorParams, PropellerParams, SimulationParams, VehicleParams, BatteryParams
 from .coords import body_to_inertial, direction_cosine_matrix, rotating_frame_derivative, angular_to_euler_rate
 from .physics import thrust, torque, apply_forces_torques
 from .helpers import control_allocation_matrix
 
@@ -41,15 +40,15 @@
 
     def reset(self):
         self.speed = 0.
         if self.motor is not None:
             self.motor.reset()
 
 
-    def apply_speed(self, u: float) -> float:
+    def apply_speed(self, u: float, **kwargs) -> float:
         """
         Calculate the actual speed of the propeller after the speed signal is
         given. This method is *pure* and does not change the state of the propeller.
         It is used by the multirotor's dxdt_* methods to calculate derivatives.
 
         Parameters
         ----------
@@ -58,19 +57,19 @@
 
         Returns
         -------
         float
             The actual speed
         """
         if self.motor is not None:
-            return self.motor.apply_speed(u)
+            return self.motor.apply_speed(u, **kwargs)
         return u
 
 
-    def step(self, u: float) -> float:
+    def step(self, u: float, **kwargs) -> float:
         """
         Step through the speed command. This method changes the state of the 
         propeller.
 
         Parameters
         ----------
         u : float
@@ -78,15 +77,15 @@
 
         Returns
         -------
         float
             The actual speed achieved.
         """
         if self.motor is not None:
-            self.speed = self.motor.step(u)
+            self.speed = self.motor.step(u, **kwargs)
         else:
             self.speed = u
         return self.speed
 
 
     def _thrust_constant(self, speed,airstream_velocity: np.ndarray=np.zeros(3)) -> float:
         return self.params.k_thrust * speed**2
@@ -130,58 +129,81 @@
     def reset(self) -> float:
         self.speed = 0.
         self.voltage = 0.
         self.current = 0.
         self._last_angular_acc = 0.
 
 
-    def apply_speed(self, u: float) -> float:
+    def current_average(self, max_voltage: float) -> float:
+        """
+        Average current consumption given the duty cycle of the speed controller.
+        Duty cycle depends on max voltage which causes 100% duty cycle.
+
+        Parameters
+        ----------
+        max_voltage : float
+            The peak voltage corresponding to 100% duty cycle.
+
+        Returns
+        -------
+        float
+            Current consumption
+        """
+        duty_cycle = self.voltage / max_voltage
+        return self.current * duty_cycle
+
+
+    def apply_speed(self, u: float, max_voltage: float=np.inf) -> float:
         """
         Apply a voltage speed signal to the motor. This method is pure and doesn't
         change the state of the motor.
 
         Parameters
         ----------
         u : float
             Voltage signal.
+        max_voltage : float, optional
+            The maximum voltage supply from power source. By default infinite.
 
         Returns
         -------
         float
             The speed of the motor (rad /s)
         """
         # This method simply calls step() but restores the state of the object
         # afterwards, thus making it a "pure" function.
         voltage, current, last_acc, last_speed = \
             self.voltage, self.current, self._last_angular_acc, self.speed
 
-        speed = self.step(u)
+        speed = self.step(u, max_voltage=max_voltage)
 
         self.voltage, self.current, self._last_angular_acc, self.speed = \
             voltage, current, last_acc, last_speed
         return speed
 
 
-    def step(self, u: float) -> float:
+    def step(self, u: float, max_voltage: float=np.inf) -> float:
         """
         Apply a voltage speed signal to the motor. This method changes the state
         of the motor.
 
         Parameters
         ----------
         u : float
-            Voltage signal.
+            Speed signal (rad/s).
+        max_voltage : float, optional
+            The maximum voltage supply from power source. By default infinite.
 
         Returns
         -------
         float
             The speed of the motor (rad /s)
         """
-        self.voltage = self.params.speed_voltage_scaling * u
-        self.current = (self.voltage - self.speed * self.params.k_emf) / self.params.resistance
+        self.voltage = np.clip(self.params.speed_voltage_scaling * u, 0, max_voltage)
+        self.current = np.clip((self.voltage - self.speed * self.params.k_emf) / self.params.resistance, 0, self.params.max_current)
         torque = self.params.k_torque * self.current
         # Subtract drag torque and dynamic friction from electrical torque
         net_torque = torque - \
                      self.params.k_df * self.speed - \
                      self.params.k_drag * self.speed**2
         accs = (self._last_angular_acc, net_torque / self.params.moment_of_inertia)
         self.speed += \
@@ -194,23 +216,29 @@
 
 
 
 class Battery:
     """
     Models the state of charge of the battery of the Multirotor.
     """
-    # TODO
+
 
     def __init__(self, params: BatteryParams, simulation: SimulationParams) -> None:
         self.params = deepcopy(params)
         self.simulation = simulation
 
 
     def reset(self):
-        pass
+        self.voltage = self.params.max_voltage
+        return self.voltage
+
+
+    @property
+    def state(self) -> float:
+        return self.voltage
 
 
     def step(self):
         pass
 
 
 
@@ -228,24 +256,29 @@
             The parameters are copied by this class, so any changes made to the params
             object is isolated from this instance.
         simulation : SimulationParams
             The simulation parameters.
         """
         self.params: VehicleParams = deepcopy(params)
         self.simulation: SimulationParams = simulation
+        self.dtype = self.params.inertia_matrix.dtype if simulation.dtype is None \
+                     else simulation.dtype
         self.state: np.ndarray = None
-        self.propellers: List[Propeller] = None
-        self.propeller_vectors: np.ndarray = None
         self.t: float = 0.
+        self._dxdt = None
         self.dxdt_decimals = max(1, 1 - int(np.log10(self.simulation.dt)))
-        self.propellers = []
+
+        self.propellers: List[Propeller] = []
         for params in self.params.propellers:
             self.propellers.append(Propeller(params, self.simulation))
-        self.dtype = self.params.inertia_matrix.dtype if simulation.dtype is None \
-                     else simulation.dtype
+
+        if self.params.battery is not None:
+            self.battery = Battery(self.params.battery, self.simulation)
+        else:
+            self.battery = Battery(BatteryParams(max_voltage=np.inf), self.simulation)
         self.reset()
 
 
     def reset(self) -> np.ndarray:
         """
         Reset the state of the vehicle. This includes resetting each propeller
         and re-calculating inertia and allocation matrices.
@@ -256,24 +289,25 @@
         -------
         np.ndarray
             The state of the vehicle.
         """
         self.t = 0.
         for p in self.propellers:
             p.reset()
-        x = cos(self.params.angles) * self.params.distances
-        y = sin(self.params.angles) * self.params.distances
-        z = np.zeros_like(y)
-        self.propeller_vectors = np.vstack((x, y, z)).astype(self.dtype)
+        if self.battery is not None:
+            self.battery.reset()
 
         self.alloc, self.alloc_inverse = control_allocation_matrix(self.params)
         self.alloc = self.alloc.astype(self.dtype)
+        self.params.propeller_vectors = self.params.propeller_vectors.astype(self.dtype)
         self.alloc_inverse = self.alloc_inverse.astype(self.dtype)
+        self.params.inertia_matrix = self.params.inertia_matrix.astype(self.dtype)
         self.params.inertia_matrix_inverse = self.params.inertia_matrix_inverse.astype(self.dtype)
         self.state = np.zeros(12, dtype=self.dtype)
+        self._dxdt = np.zeros_like(self.state)
         return self.state
 
 
     @property
     def position(self):
         """Position in the inertial frame."""
         return self.state[0:3]
@@ -282,22 +316,37 @@
     @property
     def velocity(self) -> np.ndarray:
         """Body-frame velocity"""
         return self.state[3:6]
 
 
     @property
-    def world_velocity(self) -> np.ndarray:
+    def inertial_velocity(self) -> np.ndarray:
         """Velocity in the intertial frame."""
         dcm = direction_cosine_matrix(*self.orientation)
         v_inertial = body_to_inertial(self.velocity, dcm)
         return v_inertial
 
 
     @property
+    def acceleration(self) -> np.ndarray:
+        """Body-frame acceleration"""
+        return self._dxdt[3:6]
+
+
+    @property
+    def inertial_acceleration(self) -> np.ndarray:
+        """Acceleration in the intertial frame."""
+        dcm = direction_cosine_matrix(*self.orientation)
+        a_inertial = body_to_inertial(self.acceleration, dcm)
+        return a_inertial
+
+
+
+    @property
     def orientation(self) -> np.ndarray:
         """Euler rotations (roll, pitch, yaw)"""
         return self.state[6:9]
 
 
     @property
     def angular_rate(self) -> np.ndarray:
@@ -312,14 +361,24 @@
 
 
     @property
     def weight(self) -> float:
         return self.simulation.g * self.params.mass
 
 
+    @property
+    def current_average(self) -> float:
+        """Duty-cycle adjusted currrent draw from battery."""
+        peak_voltage = self.battery.params.max_voltage
+        currents = np.asarray([p.motor.current for p in self.propellers])
+        voltages = np.asarray([p.motor.voltage for p in self.propellers])
+        duty_cycle = voltages / peak_voltage
+        return np.sum(duty_cycle * currents)
+
+
     def get_forces_torques(self, speeds: np.ndarray, state: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
         """
         Calculate the forces and torques acting on the vehicle's center of gravity
         given its current state and speed of propellers.
 
         Parameters
         ----------
@@ -332,34 +391,34 @@
         -------
         Tuple[np.ndarray, np.ndarray]
             The forces and torques acting on the body.
         """
         linear_vel_body = state[:3]
         angular_vel_body = state[3:6]
         airstream_velocity_inertial = rotating_frame_derivative(
-            self.propeller_vectors,
+            self.params.propeller_vectors,
             linear_vel_body,
             angular_vel_body)
 
         thrust_vec = np.zeros((3, len(self.propellers)), dtype=self.dtype)
         torque_vec = np.zeros_like(thrust_vec)
 
         for i, (speed, prop, clockwise) in enumerate(zip(
                 speeds,
                 self.propellers,
                 self.params.clockwise)
         ):
             last_speed = prop.speed
-            speed = prop.apply_speed(speed)
+            speed = prop.apply_speed(speed, max_voltage=self.battery.voltage)
             angular_acc = (speed - last_speed) / self.simulation.dt
             thrust_vec[2, i] = prop.thrust(
                 speed, airstream_velocity_inertial[:, i]
             )
             torque_vec[:, i] = torque(
-                self.propeller_vectors[:,i], thrust_vec[:,i],
+                self.params.propeller_vectors[:,i], thrust_vec[:,i],
                 prop.params.moment_of_inertia, angular_acc,
                 prop.params.k_drag, speed,
                 clockwise
             )
         forces = thrust_vec.sum(axis=1)
         torques = torque_vec.sum(axis=1)
         return forces, torques
@@ -386,48 +445,57 @@
         """
         # This method must not have any side-effects. It should not change the
         # state of the vehicle. This method is called multiple times from the 
         # same state by the odeint() function, and the results should be consistent.
         # Do not need to get forces/torques on body, since the action array
         # already is a 6d vector of forces/torques.
         # forces, torques = self.get_forces_torques(u, x)
-        xdot = apply_forces_torques(
-            u[:3], u[3:], x, self.simulation.g,
+        dxdt = apply_forces_torques(
+            u[:3], u[3:], x.astype(self.dtype), self.simulation.g,
             self.params.mass, self.params.inertia_matrix, self.params.inertia_matrix_inverse)
-        return np.around(xdot, self.dxdt_decimals)
+        return np.around(dxdt, self.dxdt_decimals)
 
 
-    def dxdt_speeds(self, t: float, x: np.ndarray, u: np.ndarray, params=None):
+    def dxdt_speeds(
+        self, t: float, x: np.ndarray, u: np.ndarray,
+        disturb_forces: np.ndarray=0., disturb_torques: np.ndarray=0., params=None
+    ):
         """
         Calculate the rate of change of state given the propeller speeds on the
         system (rad/s).
 
         Parameters
         ----------
         t : float
             Time. Currently this function is time invariant.
         x : np.ndarray
             State of the vehicle.
         u : np.ndarray
             A p-vector of propeller speeds (rad/s), where p=number of propellers.
+        disturb_forces : np.ndarray, optional
+            Disturbinng x,y,z forces in the vehicle's local frame, by default 0.
+        disturb_torques : np.ndarray, optional
+            Disturbing x,y,z torques in the vehicle's local frame, by default 0.
 
         Returns
         -------
         np.ndarray
             The rate of change of state.
         """
         # This method must not have any side-effects. It should not change the
         # state of the vehicle. This method is called multiple times from the 
         # same state by the odeint() function, and the results should be consistent.
         forces, torques = self.get_forces_torques(
             u, x)
-        xdot = apply_forces_torques(
-            forces, torques, x, self.simulation.g,
+        # print('dxdt-x', self.t // self.simulation.dt, x.dtype)
+        dxdt = apply_forces_torques(
+            forces+disturb_forces, torques+disturb_torques, x.astype(self.dtype), self.simulation.g,
             self.params.mass, self.params.inertia_matrix, self.params.inertia_matrix_inverse)
-        return np.around(xdot, self.dxdt_decimals)
+        # print('dxdt', self.t // self.simulation.dt, dxdt.dtype)
+        return np.around(dxdt, self.dxdt_decimals)
 
 
     def step_dynamics(self, u: np.ndarray) -> np.ndarray:
         """
         Given the 6-vector of x,y,z-forces and roll,pitch,yaw-torques, calculate
         the next state of the vehicle.
 
@@ -439,55 +507,71 @@
 
         Returns
         -------
         np.ndarray
             The new state of the vehicle.
         """
         self.t += self.simulation.dt
+        self._dxdt = self.dxdt_dynamics(t=self.t, x=self.state, u=u)
         self.state = odeint(
             self.dxdt_dynamics, self.state, (0, self.simulation.dt),
             args=(u,),
             rtol=1e-4, atol=1e-4, tfirst=True
         )[-1]
-        self.state = np.around(self.state, 4)
+        self.state = np.around(self.state, 4).astype(self.dtype)
         # TODO: inverse solve for speed = forces to set propeller speeds
         return self.state
 
 
-    def step_speeds(self, u: np.ndarray) -> np.ndarray:
+    def step_speeds(
+        self, u: np.ndarray, disturb_forces: np.ndarray=0.,
+        disturb_torques: np.ndarray=0.
+    ) -> np.ndarray:
         """
         Given the n-vector of propeller speed signals, calculate
         the next state of the vehicle. Where n is number of propellers.
 
         Parameters
         ----------
         u : np.ndarray
             The speed signals to be sent to each propeller's step() method. Can
             be the actual speed (rad/s) or the voltage signal (V) if a motor
             is used and MotorParams.speed_voltage_scaling constant is set.
+        disturb_forces : np.ndarray, optional
+            Disturbinng x,y,z forces in the vehicle's local frame, by default 0.
+        disturb_torques : np.ndarray, optional
+            Disturbing x,y,z torques in the vehicle's local frame, by default 0.
 
         Returns
         -------
         np.ndarray
             The new state of the vehicle.
         """
         self.t += self.simulation.dt
+        self._dxdt = self.dxdt_speeds(
+            t=self.t, x=self.state, u=u,
+            disturb_forces=disturb_forces, disturb_torques=disturb_torques
+        )
+        # print('pre-x', self.t // self.simulation.dt, self.state.dtype)
         self.state = odeint(
-            self.dxdt_speeds, self.state, (0, self.simulation.dt), args=(u,),
+            self.dxdt_speeds, self.state, (0, self.simulation.dt),
+            args=(u, disturb_forces, disturb_torques),
             rtol=1e-4, atol=1e-4, tfirst=True
         )[-1]
-        self.state = np.around(self.state, 4)
+        self.state = np.around(self.state, 4).astype(self.dtype)
+        # print('post-x', self.t // self.simulation.dt, self.state.dtype)
         for u_, prop in zip(u, self.propellers):
-            prop.step(u_)
+            prop.step(u_, max_voltage=self.battery.voltage)
+        self.battery.step()
         return self.state
 
 
     def allocate_control(self, thrust: float, torques: np.ndarray) -> np.ndarray:
         """
-        Allocate control to propellers by converting presscribed forces and torqes
+        Allocate control to propellers by converting prescribed forces and torqes
         into propeller speeds. Uses the control allocation matrix.
 
         Parameters
         ----------
         thrust : float
             The thrust in the body z-direction.
         torques : np.ndarray
@@ -495,15 +579,15 @@
 
         Returns
         -------
         np.ndarray
             The prescribed propeller speeds (rad /s)
         """
         # TODO: njit it? np.linalg.lstsq can be compiled
-        vec = np.asarray([thrust, *torques])
+        vec = np.asarray([thrust, *torques], self.dtype)
         # return np.sqrt(np.linalg.lstsq(self.alloc, vec, rcond=None)[0])
         return np.sqrt(
             np.clip(self.alloc_inverse @ vec, a_min=0., a_max=None)
         )
 
 
     def nonlinear_dynamics_controls_system(
```

### Comparing `multirotor-0.2.4/multirotor/vehicle.py` & `multirotor-0.3.1/multirotor/vehicle.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,24 +13,26 @@
      # See: http://learningrc.com/motor-kv/, http://web.mit.edu/first/scooter/motormath.pdf
     k_motor: float = None
     "Motor constant k_m, where speed = k_m * back_emf, and k_m = 1/k_e"
     k_emf: float = None
     "Back-EMF constant k_e, relates motor speed induced voltage, back_emf = k_e * omega"
     k_torque: float = None
     "Torque constant k_q, where torque Q = k_q * current. Equal to k_e"
-    k_drag: float = None
+    k_drag: float = None # overwritten by PropellerParams, if provided there
     "Aerodynamic drag coefficient, where torque = k_drag * omega^2"
     moment_of_inertia: float = 0.
     "Moment of inertia about rotational axis"
     k_df: float = 0.
     "Viscous damping coefficient. Torque = d_f * speed"
     static_friction: float = 0.
     speed_voltage_scaling: float = 1.
     """Scaling constant to convert speed signal (rad/s) into speed controller voltage (V).
     If 1, means input action is same as Voltage"""
+    max_current: float = np.inf
+    "Max allowed current"
 
 
     def __post_init__(self):
         # See: https://www.motioncontroltips.com/faq-difference-between-torque-back-emf-motor-constant/
         # For an ideal square-wave motor, torque and back-emf constants are same
         self.k_torque = self.k_torque or self.k_emf
         self.k_emf = self.k_emf or self.k_torque
@@ -83,32 +85,51 @@
             self.motor.k_drag = self.k_drag
         # Pitch angel is reduced to allow for even lift as blade velocity increases
         # with increasing radius. Assuming linear reduction from root to tip.
 
 
 
 @dataclass
+class BatteryParams:
+
+    max_voltage: float = np.inf
+    "Maximum voltage of the battery"
+
+
+
+@dataclass
 class VehicleParams:
 
     propellers: List[PropellerParams]
     angles: np.ndarray
     "Angle (radians) of propeller arm from the positive x-axis (forward) of the body frame."
     distances: np.ndarray
     "Distance (m) of each propeller from the centre of mass."
     clockwise: np.ndarray = None
     """1 if motor spins clockwise, -1 if anti-clockwise, looking from the top.
     Defaults to alternating clockwise/anti-clockwise."""
 
+    battery: BatteryParams = None
+    "The battery parameters"
     mass: float = 1.
+    # TODO: Should moments of inertia of propeller motors be added to this matrix
+    # manually? Currently we assume this represents the whole vehicle.
     inertia_matrix: np.matrix = np.eye(3)
+    "3x3 intertia matrix describing the rotational properties of the body."
 
 
     def __post_init__(self):
+        self.nprops = len(self.propellers)
+        "Number of propellers"
         self.distances = self.distances.astype(float)
         self.inertia_matrix_inverse = np.linalg.inv(self.inertia_matrix)
+        x = np.cos(self.angles) * self.distances
+        y = np.sin(self.angles) * self.distances
+        z = np.zeros_like(y)
+        self.propeller_vectors = np.vstack((x, y, z))
         if self.clockwise is None:
             self.clockwise = np.ones(len(self.propellers), dtype=int)
             self.clockwise[::2] = 1
             self.clockwise[1::2] = -1
 
 
 
@@ -119,15 +140,7 @@
     """Timestep of simulation"""
     g: float = 9.81
     """Gravitational acceleration"""
     rho: float = 1.225
     "Air density kg/m^3 at MSL"
     dtype: type = None
     "Default data type for arrays. If None, inferred from VehicleParams inertia_matrix."
-
-
-
-@dataclass
-class BatteryParams:
-
-    max_voltage: float = 20
-    "Maximum voltage of the battery"
```

### Comparing `multirotor-0.2.4/multirotor.egg-info/PKG-INFO` & `multirotor-0.3.1/multirotor.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multirotor
-Version: 0.2.4
+Version: 0.3.1
 Summary: Simulation testbed for multirotor vehicles.
 Keywords: multirotor,simulation,gym,uav
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: DEV
 Provides-Extra: CONTROL
```

