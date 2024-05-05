# Comparing `tmp/nqrduck_spectrometer_limenqr-0.0.5.tar.gz` & `tmp/nqrduck_spectrometer_limenqr-0.0.6.tar.gz`

## Comparing `nqrduck_spectrometer_limenqr-0.0.5.tar` & `nqrduck_spectrometer_limenqr-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/__init__.py
--rw-r--r--   0        0        0    27840 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/controller.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/limenqr.py
--rw-r--r--   0        0        0     9697 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/model.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/view.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/resources/limenqr.ini
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/resources/limenqr_widget.ui
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/LICENSE
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/README.md
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/__init__.py
+-rw-r--r--   0        0        0    30951 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/controller.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/limenqr.py
+-rw-r--r--   0        0        0    12094 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/model.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/view.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/resources/limenqr.ini
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/resources/limenqr_widget.ui
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/README.md
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/PKG-INFO
```

### Comparing `nqrduck_spectrometer_limenqr-0.0.5/.github/workflows/python-publish.yml` & `nqrduck_spectrometer_limenqr-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/controller.py` & `nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/controller.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,127 +1,170 @@
+"""Controller module for the Lime NQR spectrometer."""
+
 import logging
+from datetime import datetime
 import tempfile
 from pathlib import Path
 import numpy as np
+from scipy.signal import resample, decimate
 
 from limedriver.binding import PyLimeConfig
 from limedriver.hdf_reader import HDF
 
+from nqrduck.helpers.unitconverter import UnitConverter
 from nqrduck_spectrometer.base_spectrometer_controller import BaseSpectrometerController
 from nqrduck_spectrometer.measurement import Measurement
 from nqrduck_spectrometer.pulseparameters import TXPulse, RXReadout
 
+
 logger = logging.getLogger(__name__)
 
 
 class LimeNQRController(BaseSpectrometerController):
+    """Controller class for the Lime NQR spectrometer."""
+
     def __init__(self, module):
+        """Initializes the LimeNQRController."""
         super().__init__(module)
 
     def start_measurement(self):
+        """Starts the measurement procedure."""
         self.log_start_message()
 
         lime = self.initialize_lime()
         if lime is None:
             # Emit error message
-            self.emit_measurement_error("Error with Lime driver. Is the Lime driver installed?")
+            self.emit_measurement_error(
+                "Error with Lime driver. Is the Lime driver installed?"
+            )
             return -1
         elif lime.Npulses == 0:
             # Emit error message
-            self.emit_measurement_error("Error with pulse sequence. Is the pulse sequence empty?")
+            self.emit_measurement_error(
+                "Error with pulse sequence. Is the pulse sequence empty?"
+            )
             return -1
 
         self.setup_lime_parameters(lime)
         self.setup_temporary_storage(lime)
 
         self.emit_status_message("Started Measurement")
 
         if not self.perform_measurement(lime):
             self.emit_status_message("Measurement failed")
-            self.emit_measurement_error("Error with measurement data. Did you set an RX event?")
+            self.emit_measurement_error(
+                "Error with measurement data. Did you set an RX event?"
+            )
             return -1
 
         measurement_data = self.process_measurement_results(lime)
 
+        # Resample the RX data to the dwell time settings
+        dwell_time = self.module.model.get_setting_by_name(
+            self.module.model.RX_DWELL_TIME
+        ).value
+        dwell_time = UnitConverter.to_float(dwell_time) * 1e6
+        logger.debug("Dwell time: %s", dwell_time)
+        logger.debug(f"Last tdx value: {measurement_data.tdx[-1]}")
+
+        if dwell_time:
+            n_data_points = int(measurement_data.tdx[-1] / dwell_time)
+            logger.debug("Resampling to %s data points", n_data_points)
+            tdx = np.linspace(
+                0, measurement_data.tdx[-1], n_data_points, endpoint=False
+            )
+            tdy = resample(measurement_data.tdy, n_data_points)
+            name = measurement_data.name
+            measurement_data = Measurement(
+                name,
+                tdx,
+                tdy,
+                self.module.model.target_frequency,
+                IF_frequency=self.module.model.if_frequency,
+            )
+
         if measurement_data:
             self.emit_measurement_data(measurement_data)
             self.emit_status_message("Finished Measurement")
         else:
             self.emit_measurement_error("Measurement failed. Unable to retrieve data.")
 
-    def log_start_message(self):
-        """This method logs a message when the measurement is started."""
-        logger.debug("Starting measurement with spectrometer: %s", self.module.model.name)
-
-    def initialize_lime(self):
-        """This method initializes the limr object that is used to communicate with the pulseN driver.
-        
+    def log_start_message(self) -> None:
+        """Logs a message when the measurement is started."""
+        logger.debug(
+            "Starting measurement with spectrometer: %s", self.module.model.name
+        )
+
+    def initialize_lime(self) -> PyLimeConfig:
+        """Initializes the limr object that is used to communicate with the pulseN driver.
+
         Returns:
             PyLimeConfig: The PyLimeConfig object that is used to communicate with the pulseN driver
         """
         try:
             n_pulses = self.get_number_of_pulses()
             lime = PyLimeConfig(n_pulses)
             return lime
         except ImportError as e:
             logger.error("Error while importing limr: %s", e)
         except Exception as e:
             logger.error("Error while initializing Lime driver: %s", e)
             import traceback
+
             traceback.print_exc()
 
         return None
 
-    def setup_lime_parameters(self, lime):
-        """This method sets the parameters of the lime config according to the settings set in the spectrometer module.
-        
+    def setup_lime_parameters(self, lime: PyLimeConfig) -> None:
+        """Sets the parameters of the lime config according to the settings set in the spectrometer module.
+
         Args:
             lime (PyLimeConfig): The PyLimeConfig object that is used to communicate with the pulseN driver
         """
-        #lime.noi = -1
+        # lime.noi = -1
         lime.override_init = -1
-        # 
+        #
         # lime.nrp = 1
         lime.repetitions = 1
         lime = self.update_settings(lime)
         lime = self.translate_pulse_sequence(lime)
         lime.averages = self.module.model.averages
         self.log_lime_parameters(lime)
 
-    def setup_temporary_storage(self, lime):
-        """This method sets up the temporary storage for the measurement data.
-        
+    def setup_temporary_storage(self, lime: PyLimeConfig) -> None:
+        """Sets up the temporary storage for the measurement data.
+
         Args:
             lime (PyLimeConfig): The PyLimeConfig object that is used to communicate with the pulseN driver
         """
         temp_dir = tempfile.TemporaryDirectory()
         logger.debug("Created temporary directory at: %s", temp_dir.name)
-        lime.save_path = str(Path(temp_dir.name)) + "/"   # Temporary storage path
-        lime.file_pattern = "temp"                # Temporary filename prefix or related config
-    
-    def perform_measurement(self, lime):
-        """This method executes the measurement procedure.
-        
+        lime.save_path = str(Path(temp_dir.name)) + "/"  # Temporary storage path
+        lime.file_pattern = "temp"  # Temporary filename prefix or related config
+
+    def perform_measurement(self, lime: PyLimeConfig) -> bool:
+        """Executes the measurement procedure.
+
         Args:
             lime (PyLimeConfig): The PyLimeConfig object that is used to communicate with the pulseN driver
-            
+
         Returns:
             bool: True if the measurement was successful, False otherwise
         """
         logger.debug("Running the measurement procedure")
         try:
             lime.run()
             return True
         except Exception as e:
             logger.error("Failed to execute the measurement: %s", e)
             return False
 
-    def process_measurement_results(self, lime):
-        """This method processes the measurement results and returns a Measurement object.
-        
+    def process_measurement_results(self, lime: PyLimeConfig) -> Measurement:
+        """Processes the measurement results and returns a Measurement object.
+
         Args:
             lime (PyLimeConfig): The PyLimeConfig object that is used to communicate with the pulseN driver
 
         Returns:
             Measurement: The measurement data
         """
         rx_begin, rx_stop = self.translate_rx_event(lime)
@@ -129,119 +172,137 @@
             # Instead print the whole acquisition range
             rx_begin = 0
             rx_stop = lime.rectime_secs * 1e6
 
         logger.debug("RX event begins at: %sµs and ends at: %sµs", rx_begin, rx_stop)
         return self.calculate_measurement_data(lime, rx_begin, rx_stop)
 
-    def calculate_measurement_data(self, lime, rx_begin, rx_stop):
-        """This method calculates the measurement data from the limr object.
-        
+    def calculate_measurement_data(
+        self, lime: PyLimeConfig, rx_begin: float, rx_stop: float
+    ) -> Measurement:
+        """Calculates the measurement data from the limr object.
+
         Args:
             lime (PyLimeConfig): The PyLimeConfig object that is used to communicate with the pulseN driver
             rx_begin (float): The start time of the RX event in µs
             rx_stop (float): The stop time of the RX event in µs
 
         Returns:
             Measurement: The measurement data
         """
         try:
             path = lime.get_path()
-            hdf =  HDF(path)
+            hdf = HDF(path)
             evidx = self.find_evaluation_range_indices(hdf, rx_begin, rx_stop)
             tdx, tdy = self.extract_measurement_data(lime, hdf, evidx)
             fft_shift = self.get_fft_shift()
-            return Measurement(tdx, tdy, self.module.model.target_frequency, frequency_shift=fft_shift, IF_frequency=self.module.model.if_frequency)
+            # Measurement name date + module + target frequency + averages + sequence name
+            name = f"{datetime.now().strftime('%Y-%m-%d %H:%M:%S')} - LimeNQR - {self.module.model.target_frequency / 1e6} MHz - {self.module.model.averages} averages - {self.module.model.pulse_programmer.model.pulse_sequence.name}.quack"
+            logger.debug(f"Measurement name: {name}")
+            return Measurement(
+                name,
+                tdx,
+                tdy,
+                self.module.model.target_frequency,
+                frequency_shift=fft_shift,
+                IF_frequency=self.module.model.if_frequency,
+            )
         except Exception as e:
             logger.error("Error processing measurement result: %s", e)
             return None
 
-    def find_evaluation_range_indices(self, hdf, rx_begin, rx_stop):
-        """This method finds the indices of the evaluation range in the measurement data.
-        
+    def find_evaluation_range_indices(
+        self, hdf: HDF, rx_begin: float, rx_stop: float
+    ) -> list:
+        """Finds the indices of the evaluation range in the measurement data.
+
         Args:
-            HDF (HDF): The HDF object that is used to read the measurement data
+            hdf (HDF): The HDF object that is used to read the measurement data
             rx_begin (float): The start time of the RX event in µs
             rx_stop (float): The stop time of the RX event in µs
-        
+
         Returns:
-        list: The indices of the evaluation range in the measurement data
+            list: The indices of the evaluation range in the measurement data
         """
         return np.where((hdf.tdx > rx_begin) & (hdf.tdx < rx_stop))[0]
 
-    def extract_measurement_data(self, lime, hdf, indices):
-        """This method extracts the measurement data from the limr object.
-        
+    def extract_measurement_data(
+        self, lime: PyLimeConfig, hdf: HDF, indices: list
+    ) -> tuple:
+        """Extracts the measurement data from the PyLimeConfig object.
+
         Args:
             lime (PyLimeConfig): The PyLimeConfig object that is used to communicate with the pulseN driver
-            HDF (HDF): The HDF object that is used to read the measurement data
+            hdf (HDF): The HDF object that is used to read the measurement data
             indices (list): The indices of the evaluation range in the measurement data
 
         Returns:
             tuple: A tuple containing the time vector and the measurement data
         """
         tdx = hdf.tdx[indices] - hdf.tdx[indices][0]
         tdy = hdf.tdy[indices] / lime.averages
         # flatten the  tdy array
         tdy = tdy.flatten()
         return tdx, tdy
 
-    def get_fft_shift(self):
-        """This method returns the FFT shift value from the settings.
-        
+    def get_fft_shift(self) -> int:
+        """Rreturns the FFT shift value from the settings.
+
         Returns:
-        int: The FFT shift value
+            int: The FFT shift value
         """
-        fft_shift_enabled = self.module.model.get_setting_by_name(self.module.model.FFT_SHIFT).value
+        fft_shift_enabled = self.module.model.get_setting_by_name(
+            self.module.model.FFT_SHIFT
+        ).value
         return self.module.model.if_frequency if fft_shift_enabled else 0
 
-    def emit_measurement_data(self, measurement_data):
-        """This method emits the measurement data to the GUI.
-        
+    def emit_measurement_data(self, measurement_data: Measurement) -> None:
+        """Emits the measurement data to the GUI.
+
         Args:
             measurement_data (Measurement): The measurement data
         """
         logger.debug("Emitting measurement data")
         self.module.nqrduck_signal.emit("measurement_data", measurement_data)
 
-    def emit_status_message(self, message):
-        """This method emits a status message to the GUI.
-        
+    def emit_status_message(self, message: str) -> None:
+        """Emits a status message to the GUI.
+
         Args:
             message (str): The status message
         """
         self.module.nqrduck_signal.emit("statusbar_message", message)
 
-    def emit_measurement_error(self, error_message):
-        """This method emits a measurement error to the GUI.
-        
+    def emit_measurement_error(self, error_message: str) -> None:
+        """Emits a measurement error to the GUI.
+
         Args:
             error_message (str): The error message
         """
         logger.error(error_message)
         self.module.nqrduck_signal.emit("measurement_error", error_message)
 
-    def log_lime_parameters(self, lime):
-        """This method logs the parameters of the limr object.
-        
+    def log_lime_parameters(self, lime: PyLimeConfig) -> None:
+        """Logs the parameters of the limr object.
+
         Args:
             lime (PyLimeConfig): The PyLimeConfig object that is used to communicate with the pulseN driver
         """
         # for key, value in lime.__dict__.items():
-            # logger.debug("Lime parameter %s has value %s", key, value)
+        # logger.debug("Lime parameter %s has value %s", key, value)
         logger.debug("Lime parameter %s has value %s", "srate", lime.srate)
 
-    def update_settings(self, lime):
-        """This method sets the parameters of the limr object according to the settings set in the spectrometer module.
+    def update_settings(self, lime: PyLimeConfig) -> PyLimeConfig:
+        """Sets the parameters of the limr object according to the settings set in the spectrometer module.
 
         Args:
             lime (PyLimeConfig): The PyLimeConfig object that is used to communicate with the pulseN driver
 
         Returns:
-        lime: The updated limr object
+            lime: The updated limr object
         """
         logger.debug(
             "Updating settings for spectrometer: %s for measurement",
             self.module.model.name,
         )
         c3_tim = [0, 0, 0, 0]
         # I don't like this code
@@ -255,15 +316,17 @@
                     lime.channel = setting.get_setting()
                 elif setting.name == self.module.model.TX_MATCHING:
                     lime.TX_matching = setting.get_setting()
                 elif setting.name == self.module.model.RX_MATCHING:
                     lime.RX_matching = setting.get_setting()
                 # Careful this doesn't only set the IF frequency but the local oscillator frequency
                 elif setting.name == self.module.model.IF_FREQUENCY:
-                    lime.frq = self.module.model.target_frequency - setting.get_setting()
+                    lime.frq = (
+                        self.module.model.target_frequency - setting.get_setting()
+                    )
                     self.module.model.if_frequency = setting.get_setting()
                 elif setting.name == self.module.model.ACQUISITION_TIME:
                     lime.rectime_secs = setting.get_setting()
                 # Gate settings
                 elif setting.name == self.module.model.GATE_ENABLE:
                     c3_tim[0] = int(setting.value)
                 elif setting.name == self.module.model.GATE_PADDING_LEFT:
@@ -305,39 +368,49 @@
                     lime.RX_QcorrGain = setting.get_setting()
                 elif setting.name == self.module.model.RX_PHASE_ADJUSTMENT:
                     lime.RX_IQcorrPhase = setting.get_setting()
 
         lime.c3_tim = c3_tim
         return lime
 
-    def translate_pulse_sequence(self, lime):
-        """This method translates the pulse sequence to the limr object.
-        
+    def translate_pulse_sequence(self, lime: PyLimeConfig) -> PyLimeConfig:
+        """Ttranslates the pulse sequence to the limr object.
+
         Args:
             lime (PyLimeConfig): The PyLimeConfig object that is used to communicate with the pulseN driver
         """
         events = self.fetch_pulse_sequence_events()
 
         first_pulse = True
 
         for event in events:
             self.log_event_details(event)
             for parameter in event.parameters.values():
                 self.log_parameter_details(parameter)
 
                 if self.is_translatable_tx_parameter(parameter):
-                    pulse_shape, pulse_amplitude = self.prepare_pulse_amplitude(event, parameter)
-                    pulse_amplitude, modulated_phase = self.modulate_pulse_amplitude(pulse_amplitude, event, lime)
+                    pulse_shape, pulse_amplitude = self.prepare_pulse_amplitude(
+                        event, parameter
+                    )
+                    pulse_amplitude, modulated_phase = self.modulate_pulse_amplitude(
+                        pulse_amplitude, event, lime
+                    )
 
                     if first_pulse:  # If the pulse frequency list is empty
-                        pfr, pdr, pam, pof, pph = self.initialize_pulse_lists(lime, pulse_amplitude, pulse_shape, modulated_phase)
+                        pfr, pdr, pam, pof, pph = self.initialize_pulse_lists(
+                            lime, pulse_amplitude, pulse_shape, modulated_phase
+                        )
                         first_pulse = False
                     else:
-                        pfr_ext, pdr_ext, pam_ext, pph_ext = self.extend_pulse_lists(lime, pulse_amplitude, pulse_shape, modulated_phase)
-                        pof_ext =  self.calculate_and_set_offsets(lime, pulse_shape, events, event, pulse_amplitude)
+                        pfr_ext, pdr_ext, pam_ext, pph_ext = self.extend_pulse_lists(
+                            pulse_amplitude, pulse_shape, modulated_phase
+                        )
+                        pof_ext = self.calculate_and_set_offsets(
+                            lime, pulse_shape, events, event, pulse_amplitude
+                        )
 
                         pfr.extend(pfr_ext)
                         pdr.extend(pdr_ext)
                         pam.extend(pam_ext)
                         pof.extend(pof_ext)
                         pph.extend(pph_ext)
 
@@ -346,19 +419,20 @@
         lime.p_amp = pam
         lime.p_offs = pof
         lime.p_pha = pph
         # Set repetition time event as last event's duration and update number of pulses
         lime.reptime_secs = float(event.duration)
         lime.Npulses = len(lime.p_frq)
         return lime
-    
-    def get_number_of_pulses(self):
-        """This method calculates the number of pulses in the pulse sequence before the LimeDriverBinding is initialized.
+
+    def get_number_of_pulses(self) -> int:
+        """Calculates the number of pulses in the pulse sequence before the LimeDriverBinding is initialized.
+
         This makes sure it"s initialized with the correct size of the pulse lists.
-        
+
         Returns:
             int: The number of pulses in the pulse sequence
         """
         events = self.fetch_pulse_sequence_events()
         num_pulses = 0
         for event in events:
             for parameter in event.parameters.values():
@@ -367,125 +441,152 @@
                     num_pulses += len(pulse_amplitude)
                     logger.debug("Number of pulses: %s", num_pulses)
 
         return num_pulses
 
     # Helper functions below:
 
-    def fetch_pulse_sequence_events(self):
-        """This method fetches the pulse sequence events from the pulse programmer module.
-        
+    def fetch_pulse_sequence_events(self) -> list:
+        """Fetches the pulse sequence events from the pulse programmer module.
+
         Returns:
             list: The pulse sequence events
         """
         return self.module.model.pulse_programmer.model.pulse_sequence.events
 
-    def log_event_details(self, event):
+    def log_event_details(self, event) -> None:
+        """Logs the details of an event."""
         logger.debug("Event %s has parameters: %s", event.name, event.parameters)
 
-    def log_parameter_details(self, parameter):
+    def log_parameter_details(self, parameter) -> None:
+        """Logs the details of a parameter."""
         logger.debug("Parameter %s has options: %s", parameter.name, parameter.options)
 
     def is_translatable_tx_parameter(self, parameter):
-        """This method checks if a parameter a pulse with a transmit pulse shape (amplitude nonzero)
-        
+        """Checks if a parameter a pulse with a transmit pulse shape (amplitude nonzero).
+
         Args:
-        parameter (Parameter): The parameter to check
+            parameter (Parameter): The parameter to check
         """
-        return (parameter.name == self.module.model.TX and
-                parameter.get_option_by_name(TXPulse.RELATIVE_AMPLITUDE).value > 0)
+        return (
+            parameter.name == self.module.model.TX
+            and parameter.get_option_by_name(TXPulse.RELATIVE_AMPLITUDE).value > 0
+        )
 
     def prepare_pulse_amplitude(self, event, parameter):
-        """This method prepares the pulse amplitude for the limr object.
-        
+        """Prepares the pulse amplitude for the limr object.
+
         Args:
             event (Event): The event that contains the parameter
             parameter (Parameter): The parameter that contains the pulse shape and amplitude
-        
+
         Returns:
         tuple: A tuple containing the pulse shape and the pulse amplitude
         """
         pulse_shape = parameter.get_option_by_name(TXPulse.TX_PULSE_SHAPE).value
-        pulse_amplitude = abs(pulse_shape.get_pulse_amplitude(event.duration)) * \
-                          (parameter.get_option_by_name(TXPulse.RELATIVE_AMPLITUDE).value / 100)
+        pulse_amplitude = abs(pulse_shape.get_pulse_amplitude(event.duration)) * (
+            parameter.get_option_by_name(TXPulse.RELATIVE_AMPLITUDE).value / 100
+        )
         pulse_amplitude = np.clip(pulse_amplitude, -0.99, 0.99)
+
         return pulse_shape, pulse_amplitude
 
-    def modulate_pulse_amplitude(self, pulse_amplitude, event, lime):
-        """This method modulates the pulse amplitude for the limr object. We need to do this to have the pulse at IF frequency instead  of LO frequency.
-        
+    def modulate_pulse_amplitude(
+        self, pulse_amplitude: float, event, lime: PyLimeConfig
+    ) -> tuple:
+        """Modulates the pulse amplitude for the limr object. We need to do this to have the pulse at IF frequency instead  of LO frequency.
+
         Args:
             pulse_amplitude (float): The pulse amplitude
             event (Event): The event that contains the parameter
             lime (PyLimeConfig) : The PyLimeConfig object that is used to communicate with the pulseN driver
-        
+
         Returns:
             tuple: A tuple containing the modulated pulse amplitude and the modulated phase
         """
         # num_samples = int(float(event.duration) * lime.sra)
         num_samples = int(float(event.duration) * lime.srate)
         tdx = np.linspace(0, float(event.duration), num_samples, endpoint=False)
         shift_signal = np.exp(1j * 2 * np.pi * self.module.model.if_frequency * tdx)
+
+        # The pulse amplitude needs to be resampled to the number of samples
+        logger.debug("Resampling pulse amplitude to %s samples", num_samples)
+        pulse_amplitude = resample(pulse_amplitude, num_samples)
+
         pulse_complex = pulse_amplitude * shift_signal
         modulated_amplitude = np.abs(pulse_complex)
         modulated_phase = self.unwrap_phase(np.angle(pulse_complex))
         return modulated_amplitude, modulated_phase
 
-    def unwrap_phase(self, phase):
+    def unwrap_phase(self, phase: float) -> float:
         """This method unwraps the phase of the pulse.
-        
+
         Args:
-        phase (float): The phase of the pulse
+            phase (float): The phase of the pulse
         """
         return (np.unwrap(phase) + 2 * np.pi) % (2 * np.pi)
 
-    def initialize_pulse_lists(self, lime, pulse_amplitude, pulse_shape, modulated_phase):
+    def initialize_pulse_lists(
+        self,
+        lime: PyLimeConfig,
+        pulse_amplitude: np.array,
+        pulse_shape,
+        modulated_phase: np.array,
+    ) -> tuple:
         """This method initializes the pulse lists of the limr object.
-        
+
         Args:
             lime (PyLimeConfig): The PyLimeConfig object that is used to communicate with the pulseN driver
-            pulse_amplitude (float): The pulse amplitude
-            pulse_shape (PulseShape): The pulse shape
-            modulated_phase (float): The modulated phase
+            pulse_amplitude (np.array): The pulse amplitude
+            pulse_shape (Function): The pulse shape
+            modulated_phase (np.array): The modulated phase
         """
         pfr = [float(self.module.model.if_frequency)] * len(pulse_amplitude)
-        # We set the first  len(pulse_amplitude) of the p_dur 
+        # We set the first  len(pulse_amplitude) of the p_dur
         pdr = [float(pulse_shape.resolution)] * len(pulse_amplitude)
         pam = list(pulse_amplitude)
-        pof = ([self.module.model.OFFSET_FIRST_PULSE] +
-                    [int(pulse_shape.resolution * lime.srate)] * (len(pulse_amplitude) - 1))
+        pof = [self.module.model.OFFSET_FIRST_PULSE] + [
+            int(pulse_shape.resolution * lime.srate)
+        ] * (len(pulse_amplitude) - 1)
         pph = list(modulated_phase)
 
-        return  pfr, pdr, pam, pof, pph
+        return pfr, pdr, pam, pof, pph
 
-    def extend_pulse_lists(self, lime, pulse_amplitude, pulse_shape, modulated_phase):
+    def extend_pulse_lists(self, pulse_amplitude, pulse_shape, modulated_phase):
         """This method extends the pulse lists of the limr object.
-        
+
         Args:
-            lime (PyLimeConfig): The PyLimeConfig object that is used to communicate with the pulseN driver
             pulse_amplitude (float): The pulse amplitude
             pulse_shape (PulseShape): The pulse shape
             modulated_phase (float): The modulated phase
+
+        Returns:
+            tuple: A tuple containing the extended pulse lists (frequency, duration, amplitude, phase)
         """
-        pfr = ([float(self.module.model.if_frequency)] * len(pulse_amplitude))
-        pdr = ([float(pulse_shape.resolution)] * len(pulse_amplitude))
-        pam = (list(pulse_amplitude))
-        pph = (list(modulated_phase))
+        pfr = [float(self.module.model.if_frequency)] * len(pulse_amplitude)
+        pdr = [float(pulse_shape.resolution)] * len(pulse_amplitude)
+        pam = list(pulse_amplitude)
+        pph = list(modulated_phase)
 
         return pfr, pdr, pam, pph
 
-    def calculate_and_set_offsets(self, lime, pulse_shape, events, current_event, pulse_amplitude):
+    def calculate_and_set_offsets(
+        self, lime: PyLimeConfig, pulse_shape, events, current_event, pulse_amplitude
+    ) -> list:
         """This method calculates and sets the offsets for the limr object.
-        
+
         Args:
             lime (PyLimeConfig): The PyLimeConfig object that is used to communicate with the pulseN driver
-            pulse_shape (PulseShape): The pulse shape
+            pulse_shape (Function): The pulse shape
             events (list): The pulse sequence events
             current_event (Event): The current event
             pulse_amplitude (float): The pulse amplitude
+
+        Returns:
+            list: The offsets for the limr object
         """
         blank_durations = self.get_blank_durations_before_event(events, current_event)
 
         # Calculate the total time that has passed before the current event
         total_blank_duration = sum(blank_durations)
         # Calculate the offset for the current pulse
         # The first pulse offset is already set, so calculate subsequent ones
@@ -496,120 +597,133 @@
 
         # Set the offset for the remaining samples of the current pulse (excluding the first sample)
         # We subtract 1 because we have already set the offset for the current pulse's first sample
         offset_per_sample = int(float(pulse_shape.resolution) * lime.srate)
         pof.extend([offset_per_sample] * (len(pulse_amplitude) - 1))
         return pof
 
-    def get_blank_durations_before_event(self, events, current_event):
+    # This method could be refactored in a potential pulse sequence module
+    def get_blank_durations_before_event(self, events, current_event) -> list:
         """This method returns the blank durations before the current event.
-        
+
         Args:
             events (list): The pulse sequence events
             current_event (Event): The current event
-            
+
         Returns:
             list: The blank durations before the current event
         """
         blank_durations = []
-        previous_events_without_tx_pulse = self.get_previous_events_without_tx_pulse(events, current_event)
+        previous_events_without_tx_pulse = self.get_previous_events_without_tx_pulse(
+            events, current_event
+        )
         for event in previous_events_without_tx_pulse:
             blank_durations.append(float(event.duration))
         return blank_durations
 
-    def get_previous_events_without_tx_pulse(self, events, current_event):
+    # This method could be refactored in a potential pulse sequence module
+    def get_previous_events_without_tx_pulse(self, events, current_event) -> list:
         """This method returns the previous events without a transmit pulse.
-        
+
         Args:
             events (list): The pulse sequence events
             current_event (Event): The current event
-        
+
         Returns:
             list: The previous events without a transmit pulse
         """
         index = events.index(current_event)
         previous_events = events[:index]
         result = []
         for event in reversed(previous_events):
-            translatable = any(self.is_translatable_tx_parameter(param) for param in event.parameters.values())
+            translatable = any(
+                self.is_translatable_tx_parameter(param)
+                for param in event.parameters.values()
+            )
             if not translatable:
                 result.append(event)
             else:
                 break
-        return reversed(result)  # Reversed to maintain the original order if needed elsewhere
+        return reversed(
+            result
+        )  # Reversed to maintain the original order if needed elsewhere
 
-
-    def translate_rx_event(self, lime):
+    def translate_rx_event(self, lime: PyLimeConfig) -> tuple:
         """This method translates the RX event of the pulse sequence to the limr object.
 
         Args:
             lime (PyLimeConfig): The PyLimeConfig object that is used to communicate with the pulseN driver
 
         Returns:
             tuple: A tuple containing the start and stop time of the RX event in µs
         """
-        CORRECTION_FACTOR = self.module.model.get_setting_by_name(self.module.model.RX_OFFSET).value
+        CORRECTION_FACTOR = self.module.model.get_setting_by_name(
+            self.module.model.RX_OFFSET
+        ).value
         events = self.module.model.pulse_programmer.model.pulse_sequence.events
 
         rx_event = self.find_rx_event(events)
         if not rx_event:
             return None, None
 
-        previous_events_duration = self.calculate_previous_events_duration(events, rx_event)
+        previous_events_duration = self.calculate_previous_events_duration(
+            events, rx_event
+        )
         rx_duration = float(rx_event.duration)
 
         offset = self.calculate_offset(lime)
 
-        rx_begin = float(previous_events_duration) + float(offset) + float(CORRECTION_FACTOR)
+        rx_begin = (
+            float(previous_events_duration) + float(offset) + float(CORRECTION_FACTOR)
+        )
         rx_stop = rx_begin + rx_duration
         return rx_begin * 1e6, rx_stop * 1e6
 
     def find_rx_event(self, events):
         """This method finds the RX event in the pulse sequence.
-        
+
         Args:
             events (list): The pulse sequence events
-        
+
         Returns:
             Event: The RX event
         """
         for event in events:
             parameter = event.parameters.get(self.module.model.RX)
             if parameter and parameter.get_option_by_name(RXReadout.RX).value:
                 self.log_event_details(event)
                 self.log_parameter_details(parameter)
                 return event
         return None
 
     def calculate_previous_events_duration(self, events, rx_event):
         """This method calculates the duration of the previous events.
-        
+
         Args:
             events (list): The pulse sequence events
             rx_event (Event): The RX event
-        
+
         Returns:
             float: The duration of the previous events
         """
         previous_events = events[: events.index(rx_event)]
         return sum(event.duration for event in previous_events)
 
-    def calculate_offset(self, lime):
+    def calculate_offset(self, lime: PyLimeConfig) -> float:
         """This method calculates the offset for the RX event.
 
         Args:
-            lime (limr): The limr object that is used to communicate with the pulseN driver 
-        
+            lime (limr): The limr object that is used to communicate with the pulseN driver
+
         Returns:
             float: The offset for the RX event
         """
         return self.module.model.OFFSET_FIRST_PULSE * (1 / lime.srate)
 
-
-    def set_frequency(self, value: float):
+    def set_frequency(self, value: float) -> None:
         """This method sets the target frequency of the spectrometer.
 
         Args:
             value (float): The target frequency in MHz
         """
         logger.debug("Setting frequency to: %s", value)
         try:
@@ -618,15 +732,15 @@
         except ValueError:
             logger.warning("Could not set frequency to: %s", value)
             self.module.nqrduck_signal.emit(
                 "notification", ["Error", "Could not set frequency to: " + value]
             )
             self.module.nqrduck_signal.emit("failure_set_frequency", value)
 
-    def set_averages(self, value: int):
+    def set_averages(self, value: int) -> None:
         """This method sets the number of averages for the spectrometer.
 
         Args:
         value (int): The number of averages
         """
         logger.debug("Setting averages to: %s", value)
         try:
```

### Comparing `nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/resources/limenqr_widget.ui` & `nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/resources/limenqr_widget.ui`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_limenqr-0.0.5/LICENSE` & `nqrduck_spectrometer_limenqr-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_limenqr-0.0.5/README.md` & `nqrduck_spectrometer_limenqr-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_limenqr-0.0.5/pyproject.toml` & `nqrduck_spectrometer_limenqr-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "nqrduck-spectrometer-limenqr"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="jupfi", email="support@nqrduck.cool" },
 ]
 
 description = "A submodule for the nqrduck-spectrometer module which implements the functionality for the LimeNQR spectrometer."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `nqrduck_spectrometer_limenqr-0.0.5/PKG-INFO` & `nqrduck_spectrometer_limenqr-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nqrduck-spectrometer-limenqr
-Version: 0.0.5
+Version: 0.0.6
 Summary: A submodule for the nqrduck-spectrometer module which implements the functionality for the LimeNQR spectrometer.
 Project-URL: Homepage, https://nqrduck.cool
 Project-URL: Bug Tracker, https://github.com/nqrduck/nqrduck-spectrometer-limenqr/issues
 Project-URL: Source Code, https://github.com/nqrduck/nqrduck-spectrometer-limenqr
 Author-email: jupfi <support@nqrduck.cool>
 License: MIT License
```

