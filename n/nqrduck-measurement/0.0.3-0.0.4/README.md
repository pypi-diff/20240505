# Comparing `tmp/nqrduck_measurement-0.0.3.tar.gz` & `tmp/nqrduck_measurement-0.0.4.tar.gz`

## Comparing `nqrduck_measurement-0.0.3.tar` & `nqrduck_measurement-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0  5520293 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/docs/img/measurement_ui_labeled_v2.png
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/__init__.py
--rw-r--r--   0        0        0     8352 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/controller.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/measurement.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/model.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/signalprocessing_options.py
--rw-r--r--   0        0        0     9677 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/view.py
--rw-r--r--   0        0        0     8477 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/widget.py
--rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/resources/measurement_widget.ui
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/resources/mesurement.ini
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/LICENSE
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/README.md
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0  5520293 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/docs/img/measurement_ui_labeled_v2.png
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/__init__.py
+-rw-r--r--   0        0        0     9959 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/controller.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/measurement.py
+-rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/model.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/signalprocessing_options.py
+-rw-r--r--   0        0        0    14533 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/view.py
+-rw-r--r--   0        0        0     9123 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/widget.py
+-rw-r--r--   0        0        0     8047 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/resources/measurement_widget.ui
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/src/nqrduck_measurement/resources/mesurement.ini
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/README.md
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.4/PKG-INFO
```

### Comparing `nqrduck_measurement-0.0.3/.github/workflows/python-publish.yml` & `nqrduck_measurement-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.3/docs/img/measurement_ui_labeled_v2.png` & `nqrduck_measurement-0.0.4/docs/img/measurement_ui_labeled_v2.png`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.3/src/nqrduck_measurement/controller.py` & `nqrduck_measurement-0.0.4/src/nqrduck_measurement/controller.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """Controller for the measurement module."""
 
 import logging
 import json
-import numpy as np
-from decimal import Decimal
 from PyQt6.QtCore import pyqtSlot, pyqtSignal
 from PyQt6.QtWidgets import QApplication
-from nqrduck_spectrometer.pulsesequence import PulseSequence
 from .signalprocessing_options import Apodization
 from nqrduck.module.module_controller import ModuleController
 from nqrduck_spectrometer.measurement import Measurement
 
 logger = logging.getLogger(__name__)
 
 
@@ -21,14 +18,18 @@
 
     Args:
         module (Module): The module instance.
 
     Attributes:
         set_frequency_failure (pyqtSignal): Signal emitted when setting the frequency fails.
         set_averages_failure (pyqtSignal): Signal emitted when setting the averages fails.
+
+    Signals:
+        set_frequency_failure: Signal emitted when setting the frequency fails.
+        set_averages_failure: Signal emitted when setting the averages fails.
     """
 
     set_frequency_failure = pyqtSignal()
     set_averages_failure = pyqtSignal()
 
     def __init__(self, module):
         """Initialize the controller."""
@@ -152,15 +153,15 @@
             key == "failure_set_averages"
             and self.module.view._ui_form.averagesEdit.text() == value
         ):
             logger.debug("Received set averages failure.")
             self.set_averages_failure.emit()
         elif key == "active_spectrometer_changed":
             self.module.view._ui_form.spectrometerLabel.setText(
-                "Spectrometer: %s" % value
+                f"Spectrometer: {value}"
             )
 
     def save_measurement(self, file_name: str) -> None:
         """Save measurement to file.
 
         Args:
             file_name (str): Path to file.
@@ -225,7 +226,47 @@
 
         apodized_measurement = measurement.apodization(function)
 
         dialog.deleteLater()
 
         self.module.model.displayed_measurement = apodized_measurement
         self.module.model.add_measurement(apodized_measurement)
+
+    @pyqtSlot()
+    def change_displayed_measurement(self, measurement=None) -> None:
+        """Change the displayed measurement."""
+
+        if not self.module.model.measurements:
+            logger.debug("No measurements to display.")
+            return
+
+        if not measurement:
+            index = self.module.view._ui_form.selectionBox.value()
+            self.module.model.displayed_measurement = self.module.model.measurements[
+                index
+            ]
+            logger.debug(
+                f"Changing displayed measurement to {self.module.model.displayed_measurement.name}."
+            )
+        else:
+            logger.debug(f"Changing displayed measurement to {measurement.name}.")
+            self.module.model.displayed_measurement = measurement
+
+    @pyqtSlot(Measurement)
+    def delete_measurement(self, measurement: Measurement) -> None:
+        """Delete a measurement.
+
+        The measurement is removed from the list of measurements. Then the displayed measurement is updated.
+
+        Args:
+            measurement (Measurement): The measurement to delete.
+        """
+        logger.debug("Deleting measurement.")
+        self.module.model.remove_measurement(measurement)
+
+        if measurement == self.module.model.displayed_measurement:
+            if self.module.model.measurements:
+                self.module.model.displayed_measurement = (
+                    self.module.model.measurements[-1]
+                )
+            else:
+                self.module.model.displayed_measurement = None
```

### Comparing `nqrduck_measurement-0.0.3/src/nqrduck_measurement/model.py` & `nqrduck_measurement-0.0.4/src/nqrduck_measurement/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,23 +29,32 @@
         measurements (list): List of measurements.
         displayed_measurement (Measurement): The displayed measurement data.
         measurement_frequency (float): The measurement frequency.
         averages (int): The number of averages.
 
         validator_measurement_frequency (DuckFloatValidator): Validator for the measurement frequency.
         validator_averages (DuckIntValidator): Validator for the number of averages.
+
+    Signals:
+        displayed_measurement_changed: Signal emitted when the displayed measurement changes.
+        measurements_changed: Signal emitted when the list of measurements changes.
+        view_mode_changed: Signal emitted when the view mode changes.
+
+        measurement_frequency_changed: Signal emitted when the measurement frequency changes.
+        averages_changed: Signal emitted when the number of averages changes.
     """
 
     FILE_EXTENSION = "meas"
     # This constants are used to determine which view is currently displayed.
     FFT_VIEW = "fft"
     TIME_VIEW = "time"
 
     displayed_measurement_changed = pyqtSignal(Measurement)
     measurements_changed = pyqtSignal(list)
+    
     view_mode_changed = pyqtSignal(str)
 
     measurement_frequency_changed = pyqtSignal(float)
     averages_changed = pyqtSignal(int)
 
     def __init__(self, module) -> None:
         """Initialize the model."""
@@ -82,29 +91,42 @@
     def measurements(self, value: list[Measurement]):
         self._measurements = value
         self.measurements_changed.emit(value)
 
     def add_measurement(self, measurement: Measurement):
         """Add a measurement to the list of measurements."""
         self.measurements.append(measurement)
+        # Change the maximum value of the selectionBox.
+        self.measurements_changed.emit(self.measurements)
+        self.displayed_measurement_changed.emit(measurement)
+
+    def remove_measurement(self, measurement : Measurement):
+        """Remove a measurement from the list of measurements."""
+        self.measurements.remove(measurement)
+        # Change the maximum value of the selectionBox.
         self.measurements_changed.emit(self.measurements)
 
     @property
     def displayed_measurement(self):
         """Displayed measurement data.
 
         This is the data that is displayed in the view.
         It can be data in time domain or frequency domain.
         """
         return self._displayed_measurement
 
     @displayed_measurement.setter
     def displayed_measurement(self, value: Measurement):
         self._displayed_measurement = value
-        self.displayed_measurement_changed.emit(value)
+        if value is  not None:
+            logger.debug("Displayed measurement: " + value.name)
+            self.displayed_measurement_changed.emit(value)
+        else:
+            self.module.view.update_displayed_measurement()
+
 
     @property
     def measurement_frequency(self):
         """Measurement frequency."""
         return self._measurement_frequency
 
     @measurement_frequency.setter
```

### Comparing `nqrduck_measurement-0.0.3/src/nqrduck_measurement/signalprocessing_options.py` & `nqrduck_measurement-0.0.4/src/nqrduck_measurement/signalprocessing_options.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Signal processing options."""
-import logging 
-from decimal import Decimal
-import numpy as np
+
+import logging
 import sympy
 from nqrduck_spectrometer.measurement import Measurement
 from nqrduck.helpers.functions import Function, GaussianFunction, CustomFunction
 from nqrduck.helpers.formbuilder import DuckFormBuilder, DuckFormFunctionSelectionField
 
 logger = logging.getLogger(__name__)
 
+
 class FIDFunction(Function):
     """The exponetial FID function."""
 
     name = "FID"
 
     def __init__(self) -> None:
         """Exponential FID function."""
@@ -41,20 +41,24 @@
             GaussianFunction(),
             CustomFunction(),
         ]
 
         self.duration = (self.measurement.tdx[-1] - self.measurement.tdx[0]) * 1e-6
 
         function_selection_field = DuckFormFunctionSelectionField(
-            text=None, tooltip=None, functions=functions, duration=self.duration, parent=parent, default_function=0
+            text=None,
+            tooltip=None,
+            functions=functions,
+            duration=self.duration,
+            parent=parent,
+            default_function=0,
         )
 
         self.add_field(function_selection_field)
 
     def get_function(self) -> Function:
         """Get the selected function.
 
         Returns:
             Function: The selected function.
         """
         return self.get_values()[0]
-
```

### Comparing `nqrduck_measurement-0.0.3/src/nqrduck_measurement/widget.py` & `nqrduck_measurement-0.0.4/src/nqrduck_measurement/widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Form implementation generated from reading ui file '../nqrduck-measurement/src/nqrduck_measurement/resources/measurement_widget.ui'
+# Form implementation generated from reading ui file 'measurement_widget.ui'
 #
-# Created by: PyQt6 UI code generator 6.5.1
+# Created by: PyQt6 UI code generator 6.7.0
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_Form(object):
     def setupUi(self, Form):
         Form.setObjectName("Form")
-        Form.resize(1920, 1080)
+        Form.resize(1807, 1080)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(Form.sizePolicy().hasHeightForWidth())
         Form.setSizePolicy(sizePolicy)
         self.horizontalLayout = QtWidgets.QHBoxLayout(Form)
         self.horizontalLayout.setObjectName("horizontalLayout")
@@ -79,14 +79,24 @@
         self.settingsLayout.addWidget(self.peakButton)
         self.fittingButton = QtWidgets.QPushButton(parent=Form)
         self.fittingButton.setObjectName("fittingButton")
         self.settingsLayout.addWidget(self.fittingButton)
         self.spsettingsButton = QtWidgets.QPushButton(parent=Form)
         self.spsettingsButton.setObjectName("spsettingsButton")
         self.settingsLayout.addWidget(self.spsettingsButton)
+        self.label = QtWidgets.QLabel(parent=Form)
+        font = QtGui.QFont()
+        font.setBold(True)
+        font.setWeight(75)
+        self.label.setFont(font)
+        self.label.setObjectName("label")
+        self.settingsLayout.addWidget(self.label)
+        self.measurementsList = QtWidgets.QListWidget(parent=Form)
+        self.measurementsList.setObjectName("measurementsList")
+        self.settingsLayout.addWidget(self.measurementsList)
         spacerItem1 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.settingsLayout.addItem(spacerItem1)
         self.dataLayout = QtWidgets.QVBoxLayout()
         self.dataLayout.setObjectName("dataLayout")
         self.exportButton = QtWidgets.QPushButton(parent=Form)
         self.exportButton.setObjectName("exportButton")
         self.dataLayout.addWidget(self.exportButton)
@@ -101,29 +111,32 @@
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.plotter.sizePolicy().hasHeightForWidth())
         self.plotter.setSizePolicy(sizePolicy)
         self.plotter.setObjectName("plotter")
         self.plotterLayout.addWidget(self.plotter)
+        self.horizontalLayout_4 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_4.setObjectName("horizontalLayout_4")
+        self.plotterLayout.addLayout(self.horizontalLayout_4)
         self.horizontalLayout_3 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_3.setObjectName("horizontalLayout_3")
         spacerItem2 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_3.addItem(spacerItem2)
         self.fftButton = QtWidgets.QToolButton(parent=Form)
         self.fftButton.setObjectName("fftButton")
         self.horizontalLayout_3.addWidget(self.fftButton)
         self.selectionBox = QtWidgets.QSpinBox(parent=Form)
         self.selectionBox.setObjectName("selectionBox")
         self.horizontalLayout_3.addWidget(self.selectionBox)
         spacerItem3 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_3.addItem(spacerItem3)
         self.horizontalLayout_3.setStretch(1, 1)
         self.plotterLayout.addLayout(self.horizontalLayout_3)
-        self.plotterLayout.setStretch(1, 1)
+        self.plotterLayout.setStretch(2, 1)
         self.horizontalLayout_2.addLayout(self.plotterLayout)
         self.horizontalLayout_2.setStretch(1, 1)
         self.horizontalLayout.addLayout(self.horizontalLayout_2)
 
         self.retranslateUi(Form)
         QtCore.QMetaObject.connectSlotsByName(Form)
 
@@ -138,12 +151,13 @@
         self.buttonStart.setText(_translate("Form", "Start Measurement"))
         self.spLabel.setText(_translate("Form", "Signal Processing"))
         self.apodizationButton.setText(_translate("Form", "Apodization"))
         self.baselineButton.setText(_translate("Form", "Baseline Correction"))
         self.peakButton.setText(_translate("Form", "Peak-Picking"))
         self.fittingButton.setText(_translate("Form", "Fitting"))
         self.spsettingsButton.setText(_translate("Form", "Settings"))
+        self.label.setText(_translate("Form", "Measurements:"))
         self.exportButton.setText(_translate("Form", "Export Measurement"))
         self.importButton.setText(_translate("Form", "Import Measurement"))
         self.fftButton.setText(_translate("Form", "FFT"))
 from nqrduck.contrib.mplwidget import MplWidget
 from nqrduck.helpers.duckwidgets import DuckFloatEdit, DuckIntEdit
```

### Comparing `nqrduck_measurement-0.0.3/src/nqrduck_measurement/resources/measurement_widget.ui` & `nqrduck_measurement-0.0.4/src/nqrduck_measurement/resources/measurement_widget.ui`

 * *Files 2% similar despite different names*

#### Comparing `nqrduck_measurement-0.0.3/src/nqrduck_measurement/resources/measurement_widget.ui` & `nqrduck_measurement-0.0.4/src/nqrduck_measurement/resources/measurement_widget.ui`

```diff
@@ -2,15 +2,15 @@
 <ui version="4.0">
   <class>Form</class>
   <widget class="QWidget" name="Form">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>1920</width>
+        <width>1807</width>
         <height>1080</height>
       </rect>
     </property>
     <property name="sizePolicy">
       <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
         <horstretch>0</horstretch>
         <verstretch>0</verstretch>
@@ -19,15 +19,15 @@
     <property name="windowTitle">
       <string>Form</string>
     </property>
     <layout class="QHBoxLayout" name="horizontalLayout">
       <item>
         <layout class="QHBoxLayout" name="horizontalLayout_2" stretch="0,1">
           <item>
-            <layout class="QVBoxLayout" name="settingsLayout" stretch="0,0,0,0,0,0,0,0,0,0,0,0,0">
+            <layout class="QVBoxLayout" name="settingsLayout" stretch="0,0,0,0,0,0,0,0,0,0,0,0,0,0,0">
               <item>
                 <widget class="QLabel" name="titleLabel">
                   <property name="font">
                     <font>
                       <weight>75</weight>
                       <bold>true</bold>
                     </font>
@@ -147,14 +147,30 @@
                 <widget class="QPushButton" name="spsettingsButton">
                   <property name="text">
                     <string>Settings</string>
                   </property>
                 </widget>
               </item>
               <item>
+                <widget class="QLabel" name="label">
+                  <property name="font">
+                    <font>
+                      <weight>75</weight>
+                      <bold>true</bold>
+                    </font>
+                  </property>
+                  <property name="text">
+                    <string>Measurements:</string>
+                  </property>
+                </widget>
+              </item>
+              <item>
+                <widget class="QListWidget" name="measurementsList"/>
+              </item>
+              <item>
                 <spacer name="verticalSpacer">
                   <property name="orientation">
                     <enum>Qt::Vertical</enum>
                   </property>
                   <property name="sizeHint" stdset="0">
                     <size>
                       <width>20</width>
@@ -180,26 +196,29 @@
                     </widget>
                   </item>
                 </layout>
               </item>
             </layout>
           </item>
           <item>
-            <layout class="QVBoxLayout" name="plotterLayout" stretch="0,1">
+            <layout class="QVBoxLayout" name="plotterLayout" stretch="0,0,1">
               <item>
                 <widget class="MplWidget" name="plotter" native="true">
                   <property name="sizePolicy">
                     <sizepolicy hsizetype="Expanding" vsizetype="Expanding">
                       <horstretch>0</horstretch>
                       <verstretch>0</verstretch>
                     </sizepolicy>
                   </property>
                 </widget>
               </item>
               <item>
+                <layout class="QHBoxLayout" name="horizontalLayout_4"/>
+              </item>
+              <item>
                 <layout class="QHBoxLayout" name="horizontalLayout_3" stretch="0,1,0,0">
                   <item>
                     <spacer name="horizontalSpacer">
                       <property name="orientation">
                         <enum>Qt::Horizontal</enum>
                       </property>
                       <property name="sizeHint" stdset="0">
```

### Comparing `nqrduck_measurement-0.0.3/LICENSE` & `nqrduck_measurement-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.3/README.md` & `nqrduck_measurement-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.3/pyproject.toml` & `nqrduck_measurement-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "nqrduck-measurement"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="jupfi", email="support@nqrduck.cool" },
 ]
 
 description = "A module for the NQRduck program (a simple python script™) to perform single frequency measurements."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `nqrduck_measurement-0.0.3/PKG-INFO` & `nqrduck_measurement-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nqrduck-measurement
-Version: 0.0.3
+Version: 0.0.4
 Summary: A module for the NQRduck program (a simple python script™) to perform single frequency measurements.
 Project-URL: Homepage, https://nqrduck.cool
 Project-URL: Bug Tracker, https://github.com/nqrduck/nqrduck-measurement/issues
 Project-URL: Source Code, https://github.com/nqrduck/nqrduck-measurement
 Author-email: jupfi <support@nqrduck.cool>
 License: MIT License
```

