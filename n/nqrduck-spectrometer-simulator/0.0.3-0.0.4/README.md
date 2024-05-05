# Comparing `tmp/nqrduck_spectrometer_simulator-0.0.3.tar.gz` & `tmp/nqrduck_spectrometer_simulator-0.0.4.tar.gz`

## Comparing `nqrduck_spectrometer_simulator-0.0.3.tar` & `nqrduck_spectrometer_simulator-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.3/src/nqrduck_spectrometer_simulator/__init__.py
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.3/src/nqrduck_spectrometer_simulator/controller.py
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.3/src/nqrduck_spectrometer_simulator/model.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.3/src/nqrduck_spectrometer_simulator/simulator.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.3/src/nqrduck_spectrometer_simulator/view.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.3/src/nqrduck_spectrometer_simulator/resources/simulator.ini
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.3/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.3/LICENSE
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.3/README.md
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.4/src/nqrduck_spectrometer_simulator/__init__.py
+-rw-r--r--   0        0        0    14900 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.4/src/nqrduck_spectrometer_simulator/controller.py
+-rw-r--r--   0        0        0    12183 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.4/src/nqrduck_spectrometer_simulator/model.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.4/src/nqrduck_spectrometer_simulator/simulator.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.4/src/nqrduck_spectrometer_simulator/view.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.4/src/nqrduck_spectrometer_simulator/resources/simulator.ini
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.4/README.md
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 nqrduck_spectrometer_simulator-0.0.4/PKG-INFO
```

### Comparing `nqrduck_spectrometer_simulator-0.0.3/.github/workflows/python-publish.yml` & `nqrduck_spectrometer_simulator-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_simulator-0.0.3/src/nqrduck_spectrometer_simulator/controller.py` & `nqrduck_spectrometer_simulator-0.0.4/src/nqrduck_spectrometer_simulator/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,32 @@
+"""The controller module for the simulator spectrometer."""
+
 import logging
+from datetime import datetime
 import numpy as np
 from nqrduck_spectrometer.base_spectrometer_controller import BaseSpectrometerController
 from nqrduck_spectrometer.measurement import Measurement
 from nqrduck_spectrometer.pulseparameters import TXPulse, RXReadout
 from nqr_blochsimulator.classes.pulse import PulseArray
 from nqr_blochsimulator.classes.sample import Sample
 from nqr_blochsimulator.classes.simulation import Simulation
 
 logger = logging.getLogger(__name__)
 
 
 class SimulatorController(BaseSpectrometerController):
+    """The controller class for the nqrduck simulator module."""
+
     def __init__(self, module):
+        """Initializes the SimulatorController."""
         super().__init__(module)
 
     def start_measurement(self):
         """This method  is called when the start_measurement signal is received from the core.
+
         It will becalled if the simulator is the  active  spectrometer.
         This will start the simulation based on the settings and the pulse sequence.
         """
         logger.debug("Starting simulation")
         sample = self.get_sample_from_settings()
         logger.debug("Sample: %s", sample.name)
 
@@ -27,34 +34,40 @@
         logger.debug("Dwell time: %s", dwell_time)
 
         try:
             pulse_array = self.translate_pulse_sequence(dwell_time)
         except ValueError:
             logger.warning("Could not translate pulse sequence")
             self.module.nqrduck_signal.emit(
-                "measurement_error", "Could not translate pulse sequence. Did you configure one?"
+                "measurement_error",
+                "Could not translate pulse sequence. Did you configure one?",
             )
             return
 
-        simulation = self.get_simulation(sample, pulse_array)        
+        simulation = self.get_simulation(sample, pulse_array)
 
         result = simulation.simulate()
 
         tdx = (
             np.linspace(0, float(self.calculate_simulation_length()), len(result)) * 1e6
         )
 
         rx_begin, rx_stop = self.translate_rx_event()
         # If we have a RX event, we need to cut the result to the RX event
         if rx_begin and rx_stop:
             evidx = np.where((tdx > rx_begin) & (tdx < rx_stop))[0]
             tdx = tdx[evidx]
             result = result[evidx]
 
+        # Measurement name date + module + target frequency + averages + sequence name
+        name = f"{datetime.now().strftime('%Y-%m-%d %H:%M:%S')} - Simulator - {self.module.model.target_frequency / 1e6} MHz - {self.module.model.averages} averages - {self.module.model.pulse_programmer.model.pulse_sequence.name}"
+        logger.debug(f"Measurement name: {name}")
+
         measurement_data = Measurement(
+            name,
             tdx,
             result / simulation.averages,
             sample.resonant_frequency,
             # frequency_shift=self.module.model.if_frequency,
         )
 
         # Emit the data to the nqrduck core
@@ -202,15 +215,15 @@
             pulse_array (PulseArray): The pulse sequence translated to a PulseArray object.
 
         Returns:
             Simulation: The simulation object created from the settings and the pulse sequence.
         """
         model = self.module.model
 
-        noise = float(model.get_setting_by_name(model.NOISE).value)
+        # noise = float(model.get_setting_by_name(model.NOISE).value)
         simulation = Simulation(
             sample=sample,
             pulse=pulse_array,
             number_isochromats=int(
                 model.get_setting_by_name(model.NUMBER_ISOCHROMATS).value
             ),
             initial_magnetization=float(
@@ -272,15 +285,15 @@
         Returns:
         tuple: A tuple containing the start and stop time of the RX event in µs
         """
         # This is a correction factor for the RX event. The offset of the first pulse is 2.2µs longer than from the specified samples.
         events = self.module.model.pulse_programmer.model.pulse_sequence.events
 
         previous_events_duration = 0
-        offset = 0
+        # offset = 0
         rx_duration = 0
         for event in events:
             logger.debug("Event %s has parameters: %s", event.name, event.parameters)
             for parameter in event.parameters.values():
                 logger.debug(
                     "Parameter %s has options: %s", parameter.name, parameter.options
                 )
@@ -302,29 +315,34 @@
             return rx_begin * 1e6, rx_stop * 1e6
 
         else:
             return None, None
 
     def set_frequency(self, value: str) -> None:
         """This method is called when the set_frequency signal is received from the core.
+
         For the simulator this just prints a  warning that the simulator is selected.
+
+        Args:
+            value (str) : The new frequency in MHz.
         """
         logger.debug("Setting frequency to: %s", value)
         try:
             self.module.model.target_frequency = float(value)
             logger.debug("Successfully set frequency to: %s", value)
         except ValueError:
             logger.warning("Could not set frequency to: %s", value)
             self.module.nqrduck_signal.emit(
                 "notification", ["Error", "Could not set frequency to: " + value]
             )
             self.module.nqrduck_signal.emit("failure_set_frequency", value)
 
     def set_averages(self, value: str) -> None:
         """This method is called when the set_averages signal is received from the core.
+
         It sets the averages in the model used for the simulation.
 
         Args:
             value (str): The value to set the averages to.
         """
         logger.debug("Setting averages to: %s", value)
         try:
```

### Comparing `nqrduck_spectrometer_simulator-0.0.3/src/nqrduck_spectrometer_simulator/model.py` & `nqrduck_spectrometer_simulator-0.0.4/src/nqrduck_spectrometer_simulator/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+"""The model module for the simulator spectrometer."""
+
 import logging
 from nqrduck_spectrometer.base_spectrometer_model import BaseSpectrometerModel
 from nqrduck_spectrometer.pulseparameters import TXPulse, RXReadout
 from nqrduck_spectrometer.settings import (
     FloatSetting,
     IntSetting,
     StringSetting,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class SimulatorModel(BaseSpectrometerModel):
+    """Model class for the simulator spectrometer."""
+
     # Simulation settings
     NUMBER_POINTS = "N. simulation points"
     NUMBER_ISOCHROMATS = "N. of isochromats"
     INITIAL_MAGNETIZATION = "Initial magnetization"
     GRADIENT = "Gradient (mT/m))"
     NOISE = "Noise (uV)"
 
@@ -57,14 +61,15 @@
     SAMPLE = "Sample"
 
     # Pulse parameter constants
     TX = "TX"
     RX = "RX"
 
     def __init__(self, module):
+        """Initializes the SimulatorModel."""
         super().__init__(module)
 
         # Simulation settings
         number_of_points_setting = IntSetting(
             self.NUMBER_POINTS,
             8192,
             "Number of points used for the simulation. This influences the dwell time in combination with the total event simulation given by the pulse sequence.",
@@ -157,27 +162,23 @@
 
         power_amplifier_power_setting = FloatSetting(
             self.POWER_AMPLIFIER_POWER,
             110,
             "The power output capability of the power amplifier, determines the strength of pulses that can be generated.",
             min_value=0.1,
         )
-        self.add_setting(
-            power_amplifier_power_setting, self.HARDWARE
-        )
+        self.add_setting(power_amplifier_power_setting, self.HARDWARE)
 
         gain_setting = FloatSetting(
             self.GAIN,
             6000,
             "The amplification factor of the receiver chain, impacting the final measured signal amplitude.",
             min_value=0.1,
         )
-        self.add_setting(
-            gain_setting, self.HARDWARE
-        )
+        self.add_setting(gain_setting, self.HARDWARE)
 
         temperature_setting = FloatSetting(
             self.TEMPERATURE,
             300,
             "The absolute temperature during the experiment. This influences the SNR of the measurement.",
             min_value=0.1,
             max_value=400,
@@ -241,17 +242,15 @@
 
         resonant_frequency_setting = FloatSetting(
             self.RESONANT_FREQUENCY,
             83.56e6,
             "The resonant frequency of the observed transition.",
             min_value=1e5,
         )
-        self.add_setting(
-            resonant_frequency_setting, self.SAMPLE
-        )
+        self.add_setting(resonant_frequency_setting, self.SAMPLE)
 
         gamma_setting = FloatSetting(
             self.GAMMA,
             4.342e7,
             "The gyromagnetic ratio of the sample’s nuclei.",
             min_value=0,
         )
@@ -259,15 +258,14 @@
 
         # This could be updated to a selection setting
         nuclear_spin_setting = FloatSetting(
             self.NUCLEAR_SPIN,
             9 / 2,
             "The nuclear spin of the sample’s nuclei.",
             min_value=0,
-
         )
         self.add_setting(nuclear_spin_setting, self.SAMPLE)
 
         spin_factor_setting = FloatSetting(
             self.SPIN_FACTOR,
             2,
             "The spin factor represents the scaling coefficient for observable nuclear spin transitions along the x-axis, derived from the Pauli I x 0 -matrix elements.",
@@ -321,35 +319,42 @@
 
         # Pulse parameter options
         self.add_pulse_parameter_option(self.TX, TXPulse)
         # self.add_pulse_parameter_option(self.GATE, Gate)
         self.add_pulse_parameter_option(self.RX, RXReadout)
 
         self.averages = 1
-        self.target_frequency  = 100e6
+        self.target_frequency = 100e6
 
         # Try to load the pulse programmer module
         try:
             from nqrduck_pulseprogrammer.pulseprogrammer import pulse_programmer
 
             self.pulse_programmer = pulse_programmer
             logger.debug("Pulse programmer found.")
             self.pulse_programmer.controller.on_loading(self.pulse_parameter_options)
         except ImportError:
             logger.warning("No pulse programmer found.")
 
     @property
     def averages(self):
+        """The number of averages used for the simulation.
+
+        More averages improve the signal-to-noise ratio of the simulated signal.
+        """
         return self._averages
 
     @averages.setter
     def averages(self, value):
         self._averages = value
 
     @property
     def target_frequency(self):
+        """The target frequency for the simulation.
+
+        Doesn't do anything at the moment.
+        """
         return self._target_frequency
-    
+
     @target_frequency.setter
     def target_frequency(self, value):
         self._target_frequency = value
-
```

### Comparing `nqrduck_spectrometer_simulator-0.0.3/.gitignore` & `nqrduck_spectrometer_simulator-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_simulator-0.0.3/LICENSE` & `nqrduck_spectrometer_simulator-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_simulator-0.0.3/README.md` & `nqrduck_spectrometer_simulator-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_simulator-0.0.3/pyproject.toml` & `nqrduck_spectrometer_simulator-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "nqrduck-spectrometer-simulator"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="jupfi", email="support@nqrduck.cool" },
 ]
 
 description = "A submodule for the nqrduck-spectrometer module which implements the functionality of a NQR bloch simulator. This should enable easy simulation of NQR experiments."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `nqrduck_spectrometer_simulator-0.0.3/PKG-INFO` & `nqrduck_spectrometer_simulator-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nqrduck-spectrometer-simulator
-Version: 0.0.3
+Version: 0.0.4
 Summary: A submodule for the nqrduck-spectrometer module which implements the functionality of a NQR bloch simulator. This should enable easy simulation of NQR experiments.
 Project-URL: Homepage, https://nqrduck.cool
 Project-URL: Bug Tracker, https://github.com/nqrduck/nqrduck-spectrometer-simulator/issues
 Project-URL: Source Code, https://github.com/nqrduck/nqrduck-spectrometer-simulator
 Author-email: jupfi <support@nqrduck.cool>
 License: MIT License
```

