# Comparing `tmp/nqrduck_broadband-0.0.13.tar.gz` & `tmp/nqrduck_broadband-0.0.14.tar.gz`

## Comparing `nqrduck_broadband-0.0.13.tar` & `nqrduck_broadband-0.0.14.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/CHANGELOG.md
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0  3114606 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/docs/img/broadband_ui_labeled_v2.png
--rw-r--r--   0        0        0   167243 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/docs/img/spectrum_assembly.png
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/src/nqrduck_broadband/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/src/nqrduck_broadband/broadband.py
--rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/src/nqrduck_broadband/controller.py
--rw-r--r--   0        0        0    12717 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/src/nqrduck_broadband/model.py
--rw-r--r--   0        0        0    14824 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/src/nqrduck_broadband/view.py
--rw-r--r--   0        0        0    12855 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/src/nqrduck_broadband/widget.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/src/nqrduck_broadband/resources/broadband.ini
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/src/nqrduck_broadband/resources/broadband_widget.ui
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/LICENSE
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/README.md
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/pyproject.toml
--rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.13/PKG-INFO
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/CHANGELOG.md
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0  3114606 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/docs/img/broadband_ui_labeled_v2.png
+-rw-r--r--   0        0        0   167243 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/docs/img/spectrum_assembly.png
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/src/nqrduck_broadband/__init__.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/src/nqrduck_broadband/broadband.py
+-rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/src/nqrduck_broadband/controller.py
+-rw-r--r--   0        0        0    15509 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/src/nqrduck_broadband/model.py
+-rw-r--r--   0        0        0    16027 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/src/nqrduck_broadband/view.py
+-rw-r--r--   0        0        0    12855 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/src/nqrduck_broadband/widget.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/src/nqrduck_broadband/resources/broadband.ini
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/src/nqrduck_broadband/resources/broadband_widget.ui
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/LICENSE
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/README.md
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/pyproject.toml
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 nqrduck_broadband-0.0.14/PKG-INFO
```

### Comparing `nqrduck_broadband-0.0.13/.github/workflows/python-publish.yml` & `nqrduck_broadband-0.0.14/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck_broadband-0.0.13/docs/img/broadband_ui_labeled_v2.png` & `nqrduck_broadband-0.0.14/docs/img/broadband_ui_labeled_v2.png`

 * *Files identical despite different names*

### Comparing `nqrduck_broadband-0.0.13/docs/img/spectrum_assembly.png` & `nqrduck_broadband-0.0.14/docs/img/spectrum_assembly.png`

 * *Files identical despite different names*

### Comparing `nqrduck_broadband-0.0.13/src/nqrduck_broadband/controller.py` & `nqrduck_broadband-0.0.14/src/nqrduck_broadband/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,91 @@
+"""This module contains the BroadbandController class."""
+
 import logging
 import numpy as np
 import json
 from PyQt6.QtCore import pyqtSlot, pyqtSignal, QTimer
 from PyQt6.QtWidgets import QApplication
 from nqrduck_spectrometer.measurement import Measurement
 from nqrduck.module.module_controller import ModuleController
 
 logger = logging.getLogger(__name__)
 
 
 class BroadbandController(ModuleController):
+    """Controller class for the Broadband module.
+
+    Signals:
+        start_broadband_measurement: Signal to start a broadband measurement.
+        set_averages_failure: Signal that the set averages command failed.
+        set_frequency_step_failure: Signal that the set frequency step command failed.
+    """
+
     start_broadband_measurement = pyqtSignal()
     set_averages_failure = pyqtSignal()
     set_frequency_step_failure = pyqtSignal()
 
     def __init__(self, module):
+        """Initializes the BroadbandController."""
         super().__init__(module)
 
     @pyqtSlot(str, object)
     def process_signals(self, key: str, value: object) -> None:
         """Process incoming signal from the nqrduck module.
 
         Args:
             key (str): Name of the signal.
             value (object): Value of the signal.
         """
         logger.debug(self.module.model.waiting_for_tune_and_match)
 
-        if key == "measurement_data" and  self.module.model.current_broadband_measurement is not None:
+        if (
+            key == "measurement_data"
+            and self.module.model.current_broadband_measurement is not None
+        ):
             logger.debug("Received single measurement.")
             self.module.model.current_broadband_measurement.add_measurement(value)
 
         elif (
             key == "failure_set_averages"
             and value == self.module.view._ui_form.averagesEdit.text()
         ):
             logger.debug("Received set averages failure.")
             self.set_averages_failure.emit()
         # receive LUT data
-        elif key  == "LUT_finished":
+        elif key == "LUT_finished":
             self.received_LUT(value)
 
-        elif key == "confirm_tune_and_match" and self.module.model.waiting_for_tune_and_match:
+        elif (
+            key == "confirm_tune_and_match"
+            and self.module.model.waiting_for_tune_and_match
+        ):
             logger.debug("Confirmed tune and match.")
             reflection = value
             logger.debug("Reflection: " + str(reflection))
             if reflection is not None:
-                self.module.model.current_broadband_measurement.add_tune_and_match(reflection)
+                self.module.model.current_broadband_measurement.add_tune_and_match(
+                    reflection
+                )
             self.module.nqrduck_signal.emit("start_measurement", None)
             QApplication.processEvents()
             self.module.model.waiting_for_tune_and_match = False
 
-    def received_LUT(self, LUT : Measurement) -> None:
+    def received_LUT(self, LUT: Measurement) -> None:
         """This slot is called when the LUT data is received from the nqrduck module.
-        
+
         Args:
             LUT (Measurement): LUT data.
         """
         logger.debug("Received LUT data.")
         self.module.model.LUT = LUT
         self.change_start_frequency(self.module.model.LUT.start_frequency)
         self.change_stop_frequency(self.module.model.LUT.stop_frequency)
         self.change_frequency_step(self.module.model.LUT.frequency_step)
-        
+
     @pyqtSlot(str)
     def set_frequency(self, value: str) -> None:
         """Emits the set frequency signal to the nqrduck module.
 
         Args:
             value (str): Frequency in MHz.
         """
@@ -146,79 +165,83 @@
         # Start the first measurement
         QTimer.singleShot(500, lambda: self.start_single_measurement(start_frequency))
         QApplication.processEvents()
 
     @pyqtSlot()
     def on_broadband_measurement_added(self) -> None:
         """This slot is called when a single measurement is added to the broadband measurement.
+
         It then checks if there are more frequencies to measure and if so, starts the next measurement.
         Furthermore it updates the plots.
         """
         logger.debug("Broadband measurement added.")
         # Check if there are more frequencies to measure
         if not self.module.model.current_broadband_measurement.is_complete():
             # Get the next frequency to measure
-            next_frequency = (
-                self.module.model.current_broadband_measurement.get_next_measurement_frequency()
-            )
+            next_frequency = self.module.model.current_broadband_measurement.get_next_measurement_frequency()
             logger.debug("Next frequency: " + str(next_frequency))
-            QTimer.singleShot(500, lambda: self.start_single_measurement(next_frequency))
+            QTimer.singleShot(
+                500, lambda: self.start_single_measurement(next_frequency)
+            )
             QApplication.processEvents()
         else:
             self.module.view.add_info_text("Broadband measurement finished.")
 
     @pyqtSlot()
     def delete_LUT(self) -> None:
         """This slot is called when the LUT is deleted."""
         self.module.model.LUT = None
 
-    def start_single_measurement(self, frequency : float) -> None:
+    def start_single_measurement(self, frequency: float) -> None:
         """Starts a single measurement.
-        
+
         Args:
             frequency (float): Frequency in MHz.
         """
         logger.debug("Starting single measurement.")
-        self.module.view.add_info_text("Starting measurement at frequency: " + str(frequency))
+        self.module.view.add_info_text(
+            "Starting measurement at frequency: " + str(frequency)
+        )
         # First set the frequency of the spectrometer
         self.module.nqrduck_signal.emit("set_frequency", str(frequency))
         QApplication.processEvents()
         # If there is a LUT available, send the tune and match values as signal
         if self.module.model.LUT is not None:
             self.module.model.waiting_for_tune_and_match = True
             # We need the entry number of the LUT for the current frequency
-            
+
             self.module.nqrduck_signal.emit("set_tune_and_match", frequency * 1e-6)
             QApplication.processEvents()
         else:
             self.module.nqrduck_signal.emit("start_measurement", None)
             self.module.model.waiting_for_tune_and_match = False
             QApplication.processEvents()
 
-    def save_measurement(self, file_name : str) -> None:
+    def save_measurement(self, file_name: str) -> None:
         """Saves the current broadband measurement to a file.
-        
+
         Args:
             file_name (str): Name of the file.
         """
         logger.debug("Saving measurement to file: " + file_name)
         self.module.view.add_info_text("Saving measurement to file: " + file_name)
         QApplication.processEvents()
-    
+
         with open(file_name, "w") as f:
             json.dump(self.module.model.current_broadband_measurement.to_json(), f)
 
-
-    def load_measurement(self, file_name : str) -> None:
+    def load_measurement(self, file_name: str) -> None:
         """Loads a broadband measurement from a file.
-        
+
         Args:
             file_name (str): Name of the file.
         """
         logger.debug("Loading measurement from file: " + file_name)
 
-        with open(file_name, "r") as f:
+        with open(file_name) as f:
             measurement = json.load(f)
-            self.module.model.current_broadband_measurement = self.module.model.BroadbandMeasurement.from_json(measurement)
+            self.module.model.current_broadband_measurement = (
+                self.module.model.BroadbandMeasurement.from_json(measurement)
+            )
             self.module.view.add_info_text("Measurement loaded.")
             self.module.view.on_broadband_measurement_added()
             QApplication.processEvents()
```

### Comparing `nqrduck_broadband-0.0.13/src/nqrduck_broadband/model.py` & `nqrduck_broadband-0.0.14/src/nqrduck_broadband/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,273 +1,378 @@
+"""This module contains the BroadbandModel class which is the model for the Broadband module."""
+
 import logging
 import numpy as np
 from collections import OrderedDict
 from PyQt6.QtWidgets import QApplication
 from PyQt6.QtCore import pyqtSignal, QObject
 from nqrduck.module.module_model import ModuleModel
 from nqrduck_spectrometer.measurement import Measurement
 
 logger = logging.getLogger(__name__)
 
+
 class BroadbandModel(ModuleModel):
+    """Model class for the Broadband module.
+
+    Attributes:
+        FILE_EXTENSION (str): The file extension for the broadband module.
+        MIN_FREQUENCY (float): The minimum frequency for the broadband module.
+        MAX_FREQUENCY (float): The maximum frequency for the broadband module.
+        DEFAULT_FREQUENCY_STEP (float): The default frequency step for the broadband module.
+
+    Signals:
+        start_frequency_changed: Signal that the start frequency has changed.
+        stop_frequency_changed: Signal that the stop frequency has changed.
+        frequency_step_changed: Signal that the frequency step has changed.
+        LUT_changed: Signal that the LUT has changed.
+    """
+
     FILE_EXTENSION = "broad"
 
     MIN_FREQUENCY = 30.0
     MAX_FREQUENCY = 200.0
     DEFAULT_FREQUENCY_STEP = 0.1
 
     start_frequency_changed = pyqtSignal(float)
     stop_frequency_changed = pyqtSignal(float)
     frequency_step_changed = pyqtSignal(float)
     LUT_changed = pyqtSignal()
 
     def __init__(self, module) -> None:
+        """Initializes the BroadbandModel."""
         super().__init__(module)
         self.start_frequency = self.MIN_FREQUENCY
         self.stop_frequency = self.MAX_FREQUENCY
         self.DEFAULT_FREQUENCY_STEP = self.DEFAULT_FREQUENCY_STEP
         self.current_broadband_measurement = None
         self.waiting_for_tune_and_match = False
         self.LUT = None
 
     @property
     def start_frequency(self):
+        """The start frequency for the broadband measurement."""
         return self._start_frequency
 
     @start_frequency.setter
     def start_frequency(self, value):
         self._start_frequency = value
         self.start_frequency_changed.emit(value)
 
     @property
     def stop_frequency(self):
+        """The stop frequency for the broadband measurement."""
         return self._stop_frequency
 
     @stop_frequency.setter
     def stop_frequency(self, value):
         self._stop_frequency = value
         self.stop_frequency_changed.emit(value)
 
     @property
     def frequency_step(self):
+        """The frequency step for the broadband measurement."""
         return self._frequency_step
-    
+
     @frequency_step.setter
     def frequency_step(self, value):
         self._frequency_step = value
         self.frequency_step_changed.emit(value)
 
     @property
     def current_broadband_measurement(self):
+        """The current broadband measurement."""
         return self._current_broadband_measurement
-    
+
     @current_broadband_measurement.setter
     def current_broadband_measurement(self, value):
         self._current_broadband_measurement = value
 
     @property
     def LUT(self):
+        """The LUT for the broadband measurement."""
         return self._LUT
-    
+
     @LUT.setter
     def LUT(self, value):
         self._LUT = value
         self.LUT_changed.emit()
 
     class BroadbandMeasurement(QObject):
-        """This class represents a single broadband measurement."""
+        """This class represents a single broadband measurement.
+
+        Signals:
+            received_measurement: Signal that a measurement has been received.
+        """
 
         received_measurement = pyqtSignal()
-        
+
         def __init__(self, frequencies, frequency_step) -> None:
+            """Initializes the BroadbandMeasurement."""
             super().__init__()
             self._single_frequency_measurements = OrderedDict()
             for frequency in frequencies:
                 self._single_frequency_measurements[frequency] = None
 
             self.frequency_step = frequency_step
             self.reflection = {}
 
-        def add_measurement(self, measurement : "Measurement") -> None:
+        def add_measurement(self, measurement: "Measurement") -> None:
             """This method adds a single measurement to the broadband measurement.
-            
+
             Args:
-                measurement (Measurement): The measurement object."""
-            logger.debug("Adding measurement to broadband measurement at frequency: %s" % str(measurement.target_frequency))
-            self._single_frequency_measurements[measurement.target_frequency] = measurement
+            measurement (Measurement): The measurement object.
+            """
+            logger.debug(
+                f"Adding measurement to broadband measurement at frequency: {str(measurement.target_frequency)}"
+            )
+            self._single_frequency_measurements[measurement.target_frequency] = (
+                measurement
+            )
             self.assemble_broadband_spectrum()
             self.received_measurement.emit()
             QApplication.processEvents()
 
         def is_complete(self) -> bool:
             """This method checks if all frequencies have been measured.
-            
+
             Returns:
-                bool: True if all frequencies have been measured, False otherwise."""
+                bool: True if all frequencies have been measured, False otherwise.
+            """
             for measurement in self._single_frequency_measurements.values():
                 if measurement is None:
                     return False
             return True
-        
+
         def get_next_measurement_frequency(self) -> float:
             """This method returns the next frequency that has to be measured.
-            
+
             Returns:
-                float: The next frequency that has to be measured."""
+                float: The next frequency that has to be measured.
+            """
             for frequency, measurement in self._single_frequency_measurements.items():
                 if measurement is None:
                     return frequency
-                
+
         def get_last_completed_measurement(self) -> "Measurement":
-            """ This method returns the last completed measurement.
-            
+            """This method returns the last completed measurement.
+
             Returns:
-                Measurement: The last completed measurement."""
-            
-            for frequency, measurement in reversed(self._single_frequency_measurements.items()):
+                Measurement: The last completed measurement.
+            """
+            for frequency, measurement in reversed(
+                self._single_frequency_measurements.items()
+            ):
                 if measurement is not None:
                     return measurement
-                
+
         def get_finished_percentage(self) -> float:
             """Get the percentage of measurements that have been finished.
-            
+
             Returns:
-                float: The percentage of measurements that have been finished."""
-            
+                float: The percentage of measurements that have been finished.
+            """
             finished_measurements = 0
             for measurement in self._single_frequency_measurements.values():
                 if measurement is not None:
                     finished_measurements += 1
-            return finished_measurements / len(self._single_frequency_measurements) * 100
-        
+            return (
+                finished_measurements / len(self._single_frequency_measurements) * 100
+            )
+
         def assemble_broadband_spectrum(self) -> None:
             """This method assembles the broadband spectrum from the single frequency measurement data in frequency domain."""
             # First we get all of the single frequency measurements that have already been measured
             single_frequency_measurements = []
             for measurement in self._single_frequency_measurements.values():
                 if measurement is not None:
                     single_frequency_measurements.append(measurement)
 
-            logger.debug("Assembling broadband spectrum from %d single frequency measurements." % len(single_frequency_measurements))
+            logger.debug(
+                "Assembling broadband spectrum from %d single frequency measurements."
+                % len(single_frequency_measurements)
+            )
             fdy_assembled = np.array([])
             fdx_assembled = np.array([])
             # We cut out step_size / 2 around the IF of the spectrum and assemble the broadband spectrum
             for measurement in single_frequency_measurements:
                 # This finds the center of the spectrum if the IF is not 0 it will cut out step_size / 2 around the IF
-                logger.debug("IF frequency: %f" % measurement.IF_frequency)
+                logger.debug(f"IF frequency: {measurement.IF_frequency:f}")
                 logger.debug(measurement.fdx)
                 offset = measurement.IF_frequency * 1e-6
-                logger.debug("Offset: %f" % offset)
+                logger.debug(f"Offset: {offset:f}")
 
-                #center = np.where(measurement.fdx == offset)[0][0]
+                # center = np.where(measurement.fdx == offset)[0][0]
                 # Find closest to offset
                 center = self.find_nearest(measurement.fdx, offset)
-                
+
                 logger.debug("Center: %d" % center)
                 # This finds the nearest index of the lower and upper frequency step
-                logger.debug("Frequency step: %f" % self.frequency_step)
+                logger.debug(f"Frequency step: {self.frequency_step:f}")
                 logger.debug(measurement.fdx)
-                idx_xf_lower = self.find_nearest(measurement.fdx, offset - ((self.frequency_step/2) * 1e-6)) 
-                idx_xf_upper = self.find_nearest(measurement.fdx, offset + ((self.frequency_step/2) * 1e-6))
+                idx_xf_lower = self.find_nearest(
+                    measurement.fdx, offset - ((self.frequency_step / 2) * 1e-6)
+                )
+                idx_xf_upper = self.find_nearest(
+                    measurement.fdx, offset + ((self.frequency_step / 2) * 1e-6)
+                )
 
                 # This interpolates the y values of the lower and upper frequency step
-                yf_interp_lower = np.interp(offset-self.frequency_step/2 * 1e-6, [measurement.fdx[idx_xf_lower], measurement.fdx[center]], 
-                                        [abs(measurement.fdy)[idx_xf_lower], abs(measurement.fdy)[center]])
-            
-                yf_interp_upper = np.interp(offset+self.frequency_step/2 * 1e-6, [measurement.fdx[center], measurement.fdx[idx_xf_upper]], 
-                                        [abs(measurement.fdy)[center], abs(measurement.fdy)[idx_xf_lower]]) 
-                
+                yf_interp_lower = np.interp(
+                    offset - self.frequency_step / 2 * 1e-6,
+                    [measurement.fdx[idx_xf_lower], measurement.fdx[center]],
+                    [abs(measurement.fdy)[idx_xf_lower], abs(measurement.fdy)[center]],
+                )
+
+                yf_interp_upper = np.interp(
+                    offset + self.frequency_step / 2 * 1e-6,
+                    [measurement.fdx[center], measurement.fdx[idx_xf_upper]],
+                    [abs(measurement.fdy)[center], abs(measurement.fdy)[idx_xf_lower]],
+                )
+
                 try:
                     # We take the last point of the previous spectrum and the first point of the current spectrum and average them
                     fdy_assembled[-1] = (fdy_assembled[-1] + yf_interp_lower) / 2
                     # Then we append the data from idx_xf_lower + 1 (because of the averaged datapoint) to idx_xf_upper
-                    fdy_assembled = np.append(fdy_assembled, abs(measurement.fdy)[idx_xf_lower+1:idx_xf_upper-1])
+                    fdy_assembled = np.append(
+                        fdy_assembled,
+                        abs(measurement.fdy)[idx_xf_lower + 1 : idx_xf_upper - 1],
+                    )
                     fdy_assembled = np.append(fdy_assembled, yf_interp_upper)
-                    
+
                     # We append the frequency values of the current spectrum and shift them by the target frequency
-                    fdx_assembled = np.append(fdx_assembled, -self.frequency_step/2 * 1e-6 + measurement.target_frequency * 1e-6)
-                    fdx_assembled = np.append(fdx_assembled, measurement.fdx[idx_xf_lower + 1:idx_xf_upper - 1] + measurement.target_frequency * 1e-6 - offset)
+                    fdx_assembled = np.append(
+                        fdx_assembled,
+                        -self.frequency_step / 2 * 1e-6
+                        + measurement.target_frequency * 1e-6,
+                    )
+                    fdx_assembled = np.append(
+                        fdx_assembled,
+                        measurement.fdx[idx_xf_lower + 1 : idx_xf_upper - 1]
+                        + measurement.target_frequency * 1e-6
+                        - offset,
+                    )
 
                 # On the first run we will get an Index Error
                 except IndexError:
                     fdy_assembled = np.array([yf_interp_lower])
-                    fdy_assembled = np.append(fdy_assembled, abs(measurement.fdy)[idx_xf_lower+1:idx_xf_upper-1])
+                    fdy_assembled = np.append(
+                        fdy_assembled,
+                        abs(measurement.fdy)[idx_xf_lower + 1 : idx_xf_upper - 1],
+                    )
                     fdy_assembled = np.append(fdy_assembled, yf_interp_upper)
 
-                    first_time_values = (measurement.fdx[idx_xf_lower:idx_xf_upper] + measurement.target_frequency * 1e-6 - offset)
-                    first_time_values[0] =  -self.frequency_step/2 * 1e-6 + measurement.target_frequency * 1e-6
-                    first_time_values[-1] = +self.frequency_step/2 * 1e-6 + measurement.target_frequency * 1e-6
-                    
+                    first_time_values = (
+                        measurement.fdx[idx_xf_lower:idx_xf_upper]
+                        + measurement.target_frequency * 1e-6
+                        - offset
+                    )
+                    first_time_values[0] = (
+                        -self.frequency_step / 2 * 1e-6
+                        + measurement.target_frequency * 1e-6
+                    )
+                    first_time_values[-1] = (
+                        +self.frequency_step / 2 * 1e-6
+                        + measurement.target_frequency * 1e-6
+                    )
+
                     fdx_assembled = np.array(first_time_values)
-            
+
             self.broadband_data_fdx = fdx_assembled.flatten()
             self.broadband_data_fdy = fdy_assembled.flatten()
-        
+
         def add_tune_and_match(self, magnitude) -> None:
             """This method adds the tune and match values to the last completed measurement.
-            
+
             Args:
-                magnitude (float): The magnitude of the tune and match values."""
+            magnitude (float): The magnitude of the tune and match values.
+            """
             logger.debug("Adding tune and match values toat next measurement frequency")
             next_measurement_frequency = self.get_next_measurement_frequency()
             self.reflection[next_measurement_frequency] = magnitude
 
+        def find_nearest(self, array: np.array, value: float) -> int:
+            """This method finds the nearest value in an array to a given value.
+
+            Args:
+                array (np.array): The array to search in.
+                value (float): The value to search for.
 
-        def find_nearest(self, array, value) -> int:
+            Returns:
+                int: The index of the nearest value in the array.
+            """
             array = np.asarray(array)
             idx = (np.abs(array - value)).argmin()
             return idx
-        
+
         def to_json(self):
-            """Converts the broadband measurement to a json-compatible format."""
+            """Converts the broadband measurement to a json-compatible format.
+
+            Returns:
+                dict: The json-compatible format of the broadband measurement.
+            """
             return {
-                "single_frequency_measurements": [measurement.to_json() for measurement in self.single_frequency_measurements.values()],
-                "reflection": self.reflection
+                "single_frequency_measurements": [
+                    measurement.to_json()
+                    for measurement in self.single_frequency_measurements.values()
+                ],
+                "reflection": self.reflection,
             }
-        
+
         @classmethod
-        def from_json(cls, json):
-            """Converts the json format to a broadband measurement."""
+        def from_json(cls, json: dict):
+            """Converts the json format to a broadband measurement.
+
+            Args:
+                json (dict): The json format of the broadband measurement.
+
+            Returns:
+                BroadbandMeasurement: The broadband measurement object.
+            """
             # We create a broadband measurement object with the frequencies and frequency step from the first single frequency measurement
-            frequencies = [measurement["target_frequency"] for measurement in json["single_frequency_measurements"]]
-            
+            frequencies = [
+                measurement["target_frequency"]
+                for measurement in json["single_frequency_measurements"]
+            ]
 
             # We need to calculate the frequency step from the first two measurements
             frequency_step = frequencies[1] - frequencies[0]
 
             broadband_measurement = cls(frequencies, frequency_step)
 
             # We add all of the single frequency measurements to the broadband measurement
             for measurement in json["single_frequency_measurements"]:
-                broadband_measurement.add_measurement(Measurement.from_json(measurement))
+                broadband_measurement.add_measurement(
+                    Measurement.from_json(measurement)
+                )
 
             # We assemble the broadband spectrum
             broadband_measurement.assemble_broadband_spectrum()
 
             return broadband_measurement
 
         @property
         def single_frequency_measurements(self) -> dict:
             """This property contains the dict of all frequencies that have to be measured."""
             return self._single_frequency_measurements
-        
+
         @single_frequency_measurements.setter
         def single_frequency_measurements(self, value):
             self._single_frequency_measurements = value
 
         @property
         def broadband_data_fdx(self):
-            """ This property contains the broadband data and is assembled by the differen single_frequency measurements in frequency domain."""
+            """This property contains the broadband data and is assembled by the different single_frequency measurements in frequency domain."""
             return self._broadband_data_fdx
 
         @broadband_data_fdx.setter
         def broadband_data_fdx(self, value):
             self._broadband_data_fdx = value
 
         @property
         def broadband_data_fdy(self):
-            """ This property contains the broadband data and is assembled by the differen single_frequency measurements in frequency domain."""
+            """This property contains the broadband data and is assembled by the different single_frequency measurements in frequency domain."""
             return self._broadband_data_fdy
-        
+
         @broadband_data_fdy.setter
         def broadband_data_fdy(self, value):
             self._broadband_data_fdy = value
```

### Comparing `nqrduck_broadband-0.0.13/src/nqrduck_broadband/view.py` & `nqrduck_broadband-0.0.14/src/nqrduck_broadband/view.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,47 @@
+"""This module contains the view of the broadband module."""
 import logging
 from datetime import datetime
 from PyQt6.QtCore import pyqtSlot, pyqtSignal, Qt
 from PyQt6.QtWidgets import QWidget, QMessageBox, QApplication, QLabel, QVBoxLayout
 from nqrduck.assets.icons import Logos
 from nqrduck.module.module_view import ModuleView
 from .widget import Ui_Form
 
 logger = logging.getLogger(__name__)
 
 
 class BroadbandView(ModuleView):
+    """View class for the Broadband module.
+    
+    Signals:
+        start_broadband_measurement: Signal to start a broadband measurement.
+    """
     start_broadband_measurement = pyqtSignal()
 
     def __init__(self, module):
+        """Initializes the BroadbandView."""
         super().__init__(module)
 
         widget = QWidget()
         self._ui_form = Ui_Form()
         self._ui_form.setupUi(self)
         self.widget = widget
 
         logger.debug(
-            "Facecolor %s" % str(self._ui_form.broadbandPlot.canvas.ax.get_facecolor())
+            f"Facecolor {str(self._ui_form.broadbandPlot.canvas.ax.get_facecolor())}"
         )
 
         self.connect_signals()
 
         # Add logos
         self._ui_form.start_measurementButton.setIcon(Logos.Play_16x16())
-        self._ui_form.start_measurementButton.setIconSize(self._ui_form.start_measurementButton.size())
+        self._ui_form.start_measurementButton.setIconSize(
+            self._ui_form.start_measurementButton.size()
+        )
 
         self._ui_form.exportButton.setIcon(Logos.Save16x16())
         self._ui_form.exportButton.setIconSize(self._ui_form.exportButton.size())
 
         self._ui_form.importButton.setIcon(Logos.Load16x16())
         self._ui_form.importButton.setIconSize(self._ui_form.importButton.size())
 
@@ -63,17 +72,21 @@
         )
 
         self.module.model.start_frequency_changed.connect(
             self.on_start_frequency_change
         )
         self.module.model.stop_frequency_changed.connect(self.on_stop_frequency_change)
         self.module.model.frequency_step_changed.connect(self.on_frequency_step_change)
-        
-        self._ui_form.start_measurementButton.clicked.connect(self.start_measurement_clicked)
-        self.start_broadband_measurement.connect(self.module._controller.start_broadband_measurement)
+
+        self._ui_form.start_measurementButton.clicked.connect(
+            self.start_measurement_clicked
+        )
+        self.start_broadband_measurement.connect(
+            self.module._controller.start_broadband_measurement
+        )
 
         self._ui_form.averagesEdit.editingFinished.connect(
             lambda: self.on_editing_finished(self._ui_form.averagesEdit.text())
         )
 
         self.module.controller.set_averages_failure.connect(
             self.on_set_averages_failure
@@ -91,18 +104,18 @@
         # Save and load buttons
         self._ui_form.exportButton.clicked.connect(self.on_save_button_clicked)
         self._ui_form.importButton.clicked.connect(self.on_load_button_clicked)
 
     @pyqtSlot()
     def start_measurement_clicked(self) -> None:
         """This method is called when the start measurement button is clicked.
+
         It shows a dialog asking the user if he really wants to start the measurement.
         If the user clicks yes the start_broadband_measurement signal is emitted.
         """
-
         # Create a QMessageBox object
         msg_box = QMessageBox(parent=self)
         msg_box.setText("Start the measurement?")
         msg_box.setStandardButtons(
             QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No
         )
 
@@ -115,29 +128,35 @@
         # Process the user's choice
         if choice == QMessageBox.StandardButton.Yes:
             self.start_broadband_measurement.emit()
 
     @pyqtSlot()
     def on_save_button_clicked(self) -> None:
         """This method is called when the save button is clicked.
+
         It shows a file dialog to the user to select a file to save the measurement to.
         """
         logger.debug("Save button clicked.")
-        file_manager = self.QFileManager(self.module.model.FILE_EXTENSION, parent=self.widget)
+        file_manager = self.FileManager(
+            self.module.model.FILE_EXTENSION, parent=self.widget
+        )
         file_name = file_manager.saveFileDialog()
         if file_name:
             self.module.controller.save_measurement(file_name)
 
     @pyqtSlot()
     def on_load_button_clicked(self) -> None:
         """This method is called when the load button is clicked.
+
         It shows a file dialog to the user to select a file to load the measurement from.
         """
         logger.debug("Load button clicked.")
-        file_manager = self.QFileManager(self.module.model.FILE_EXTENSION, parent=self.widget)
+        file_manager = self.FileManager(
+            self.module.model.FILE_EXTENSION, parent=self.widget
+        )
         file_name = file_manager.loadFileDialog()
         if file_name:
             self.module.controller.load_measurement(file_name)
 
     def init_plots(self) -> None:
         """Initialize the plots."""
         # Initialization of broadband spectrum
@@ -172,124 +191,188 @@
         self._ui_form.broadbandPlot.canvas.ax.set_xlabel("Frequency in MHz")
         self._ui_form.broadbandPlot.canvas.ax.set_ylabel("Magnitude a.u.")
         self._ui_form.broadbandPlot.canvas.ax.grid()
 
     @pyqtSlot(float)
     def on_start_frequency_change(self, start_frequency: float) -> None:
         """This method is called when the start frequency is changed.
+
         It adjusts the view to the new start frequency.
+
+        Args:
+            start_frequency (float) : The new start frequency.
         """
         logger.debug(
             "Adjusting view to new start frequency: " + str(start_frequency * 1e-6)
         )
         self._ui_form.broadbandPlot.canvas.ax.set_xlim(left=start_frequency * 1e-6)
         self._ui_form.broadbandPlot.canvas.draw()
         self._ui_form.broadbandPlot.canvas.flush_events()
         self._ui_form.start_frequencyField.setText(str(start_frequency * 1e-6))
 
     @pyqtSlot(float)
     def on_stop_frequency_change(self, stop_frequency: float) -> None:
         """This method is called when the stop frequency is changed.
+
         It adjusts the view to the new stop frequency.
+
+        Args:
+            stop_frequency (float) : The new stop frequency.
         """
         logger.debug(
             "Adjusting view to new stop frequency: " + str(stop_frequency * 1e-6)
         )
         self._ui_form.broadbandPlot.canvas.ax.set_xlim(right=stop_frequency * 1e-6)
         self._ui_form.broadbandPlot.canvas.draw()
         self._ui_form.broadbandPlot.canvas.flush_events()
         self._ui_form.stop_frequencyField.setText(str(stop_frequency * 1e-6))
 
     @pyqtSlot(float)
-    def on_frequency_step_change(self, frequency_step : float) -> None:
+    def on_frequency_step_change(self, frequency_step: float) -> None:
         """This method is called when the frequency step is changed.
+
         It adjusts the view to the new frequency step.
+
+        Args:
+            frequency_step (float) : The new frequency step.
         """
-        logger.debug("Adjusting view to new frequency step: " + str(frequency_step * 1e-6))
-        self._ui_form.broadbandPlot.canvas.ax.set_xlim(right=frequency_step*1e-6)
+        logger.debug(
+            "Adjusting view to new frequency step: " + str(frequency_step * 1e-6)
+        )
+        self._ui_form.broadbandPlot.canvas.ax.set_xlim(right=frequency_step * 1e-6)
         self._ui_form.broadbandPlot.canvas.draw()
         self._ui_form.broadbandPlot.canvas.flush_events()
         # Fix float representation
-        frequency_step = str("{:.2f}".format(frequency_step * 1e-6))
+        frequency_step = str(f"{frequency_step * 1e-6:.2f}")
         self._ui_form.frequencystepEdit.setText(frequency_step)
 
     @pyqtSlot()
     def on_editing_finished(self, value: str) -> None:
         """This method is called when the user finished editing a field.
+
         It sets the value of the field in the model.
+
+        Args:
+            value (str) : The value of the field.
         """
         logger.debug("Editing finished by.")
         self.sender().setStyleSheet("")
         if self.sender() == self._ui_form.averagesEdit:
             self.module.controller.set_averages(value)
 
     @pyqtSlot()
     def on_set_averages_failure(self) -> None:
         """This method is called when the averages could not be set.
+
         It sets the border of the averages field to red indicating that the entered value was not valid.
         """
         logger.debug("Set averages failure.")
         self._ui_form.averagesEdit.setStyleSheet("border: 1px solid red;")
 
     @pyqtSlot()
     def on_set_frequency_step_failure(self) -> None:
         """This method is called when the frequency step could not be set.
+
         It sets the border of the frequency step field to red indicating that the entered value was not valid.
         """
         logger.debug("Set frequency step failure.")
         self._ui_form.frequencystepEdit.setStyleSheet("border: 1px solid red;")
 
     @pyqtSlot()
     def on_broadband_measurement_added(self) -> None:
         """This method is called when a new broadband measurement is added to the model.
+
         It updates the plots and the progress bar.
         """
         # Get last measurement from the broadband measurement object that is not None
         logger.debug("Updating broadband plot.")
-        measurement = (
-            self.module.model.current_broadband_measurement.get_last_completed_measurement()
-        )
+        measurement = self.module.model.current_broadband_measurement.get_last_completed_measurement()
 
         td_plotter = self._ui_form.time_domainPlot.canvas.ax
         fd_plotter = self._ui_form.frequency_domainPlot.canvas.ax
         broadband_plotter = self._ui_form.broadbandPlot.canvas.ax
 
         td_plotter.clear()
         fd_plotter.clear()
         broadband_plotter.clear()
 
-        td_plotter.plot(measurement.tdx, measurement.tdy.real, label="Real", linestyle="-", alpha=0.35, color="red")
-        td_plotter.plot(measurement.tdx, measurement.tdy.imag, label="Imaginary", linestyle="-", alpha=0.35, color="green")
-        td_plotter.plot(measurement.tdx, abs(measurement.tdy), label="Magnitude", color="blue")
+        td_plotter.plot(
+            measurement.tdx,
+            measurement.tdy.real,
+            label="Real",
+            linestyle="-",
+            alpha=0.35,
+            color="red",
+        )
+        td_plotter.plot(
+            measurement.tdx,
+            measurement.tdy.imag,
+            label="Imaginary",
+            linestyle="-",
+            alpha=0.35,
+            color="green",
+        )
+        td_plotter.plot(
+            measurement.tdx, abs(measurement.tdy), label="Magnitude", color="blue"
+        )
         td_plotter.legend()
 
-        fd_plotter.plot(measurement.fdx * 1e-6, measurement.fdy.real, label="Real", linestyle="-", alpha=0.35, color="red")
-        fd_plotter.plot(measurement.fdx * 1e-6, measurement.fdy.imag, label="Imaginary", linestyle="-", alpha=0.35, color="green")
-        fd_plotter.plot(measurement.fdx * 1e-6, abs(measurement.fdy), label="Magnitude", color="blue")
+        fd_plotter.plot(
+            measurement.fdx * 1e-6,
+            measurement.fdy.real,
+            label="Real",
+            linestyle="-",
+            alpha=0.35,
+            color="red",
+        )
+        fd_plotter.plot(
+            measurement.fdx * 1e-6,
+            measurement.fdy.imag,
+            label="Imaginary",
+            linestyle="-",
+            alpha=0.35,
+            color="green",
+        )
+        fd_plotter.plot(
+            measurement.fdx * 1e-6,
+            abs(measurement.fdy),
+            label="Magnitude",
+            color="blue",
+        )
         fd_plotter.legend()
 
         # Plot real and imag part again here in time and frequency domain
         broadband_plotter.plot(
             self.module.model.current_broadband_measurement.broadband_data_fdx,
             self.module.model.current_broadband_measurement.broadband_data_fdy,
         )
 
         # Plot S11 values on the twin axis of the broadband plot
-        frequencies  = self.module.model.current_broadband_measurement.reflection.keys()
+        frequencies = self.module.model.current_broadband_measurement.reflection.keys()
         frequencies = [frequency * 1e-6 for frequency in frequencies]
 
-        reflection_values = self.module.model.current_broadband_measurement.reflection.values()
+        reflection_values = (
+            self.module.model.current_broadband_measurement.reflection.values()
+        )
         if reflection_values:
-            self._ui_form.broadbandPlot.canvas.S11ax = self._ui_form.broadbandPlot.canvas.ax.twinx()
+            self._ui_form.broadbandPlot.canvas.S11ax = (
+                self._ui_form.broadbandPlot.canvas.ax.twinx()
+            )
             S11plotter = self._ui_form.broadbandPlot.canvas.S11ax
             S11plotter.clear()
             # Make second axis for S11 value
             self._ui_form.broadbandPlot.canvas.S11ax.set_ylabel("S11 in dB")
             self._ui_form.broadbandPlot.canvas.S11ax.set_ylim([-40, 0])
-            S11plotter.plot(frequencies, reflection_values, color="red", marker="x", linestyle="None")
+            S11plotter.plot(
+                frequencies,
+                reflection_values,
+                color="red",
+                marker="x",
+                linestyle="None",
+            )
 
         self.set_timedomain_labels()
         self.set_frequencydomain_labels()
         self.set_broadband_labels()
 
         self._ui_form.time_domainPlot.canvas.draw()
         self._ui_form.frequency_domainPlot.canvas.draw()
@@ -316,18 +399,18 @@
             self._ui_form.activeLUTLabel.setText(self.module.model.LUT.TYPE)
         else:
             self._ui_form.start_frequencyField.setEnabled(True)
             self._ui_form.stop_frequencyField.setEnabled(True)
             self._ui_form.frequencystepEdit.setEnabled(True)
             self._ui_form.activeLUTLabel.setText("None")
 
-    def add_info_text(self, text : str) -> None:
+    def add_info_text(self, text: str) -> None:
         """Add a text to the info box with a timestamp.
 
         Args:
             text (str): The text to add to the info box.
         """
         timestamp = datetime.now().strftime("%H:%M:%S")
-        text = "[%s] %s" % (timestamp, text)
+        text = f"[{timestamp}] {text}"
         text_label = QLabel(text)
         text_label.setStyleSheet("font-size: 25px;")
         self._ui_form.scrollAreaWidgetContents.layout().addWidget(text_label)
```

### Comparing `nqrduck_broadband-0.0.13/src/nqrduck_broadband/widget.py` & `nqrduck_broadband-0.0.14/src/nqrduck_broadband/widget.py`

 * *Files identical despite different names*

### Comparing `nqrduck_broadband-0.0.13/src/nqrduck_broadband/resources/broadband_widget.ui` & `nqrduck_broadband-0.0.14/src/nqrduck_broadband/resources/broadband_widget.ui`

 * *Files identical despite different names*

### Comparing `nqrduck_broadband-0.0.13/LICENSE` & `nqrduck_broadband-0.0.14/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Julia Pfitzer
+Copyright (c) 2023 jupfi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `nqrduck_broadband-0.0.13/README.md` & `nqrduck_broadband-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `nqrduck_broadband-0.0.13/pyproject.toml` & `nqrduck_broadband-0.0.14/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nqrduck-broadband"
-version = "0.0.13"
+version = "0.0.14"
 authors = [
   { name="jupfi", email="support@nqrduck.cool" },
 ]
 
 description = "A module for the NQRduck program (a simple python script™) to do broadband magnetic resonance measurements."
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "matplotlib",
     "pyqt6",
     "nqrduck",
+    "nqrduck-spectrometer",
 ]
 
 [project.entry-points."nqrduck"]
 "nqrduck-broadband" = "nqrduck_broadband.broadband:Broadband"
 
 [tool.ruff]
 exclude = [
```

### Comparing `nqrduck_broadband-0.0.13/PKG-INFO` & `nqrduck_broadband-0.0.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.3
 Name: nqrduck-broadband
-Version: 0.0.13
+Version: 0.0.14
 Summary: A module for the NQRduck program (a simple python script™) to do broadband magnetic resonance measurements.
 Project-URL: Homepage, https://nqrduck.cool
 Project-URL: Bug Tracker, https://github.com/nqrduck/nqrduck-broadband/issues
 Project-URL: Source Code, https://github.com/nqrduck/nqrduck-broadband
 Author-email: jupfi <support@nqrduck.cool>
 License: MIT License
         
-        Copyright (c) 2023 Julia Pfitzer
+        Copyright (c) 2023 jupfi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -27,17 +27,18 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Requires-Dist: matplotlib
 Requires-Dist: nqrduck
+Requires-Dist: nqrduck-spectrometer
 Requires-Dist: pyqt6
 Description-Content-Type: text/markdown
 
 # NQRduck Module: nqrduck-broadband
 
 A module for the [nqrduck](https://github.com/nqrduck/nqrduck) project. This module is used for broadband magnetic resonance experiments.
```

