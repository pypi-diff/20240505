# Comparing `tmp/nqrduck_pulseprogrammer-0.0.3.tar.gz` & `tmp/nqrduck_pulseprogrammer-0.0.4.tar.gz`

## Comparing `nqrduck_pulseprogrammer-0.0.3.tar` & `nqrduck_pulseprogrammer-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0   102155 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/docs/img/pulseprogrammer_labeled.png
--rw-r--r--   0        0        0   990292 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/docs/img/pulseprogrammer_tx_labeled.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/__init__.py
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/controller.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/model.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/pulseprogrammer.py
--rw-r--r--   0        0        0    25627 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/view.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/resources/pulseprogrammer.ini
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/LICENSE
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/README.md
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0   102155 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.4/docs/img/pulseprogrammer_labeled.png
+-rw-r--r--   0        0        0   990292 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.4/docs/img/pulseprogrammer_tx_labeled.png
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.4/src/nqrduck_pulseprogrammer/__init__.py
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.4/src/nqrduck_pulseprogrammer/controller.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.4/src/nqrduck_pulseprogrammer/model.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.4/src/nqrduck_pulseprogrammer/pulseprogrammer.py
+-rw-r--r--   0        0        0    25543 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.4/src/nqrduck_pulseprogrammer/view.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.4/src/nqrduck_pulseprogrammer/resources/pulseprogrammer.ini
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.4/README.md
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.4/PKG-INFO
```

### Comparing `nqrduck_pulseprogrammer-0.0.3/.github/workflows/python-publish.yml` & `nqrduck_pulseprogrammer-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck_pulseprogrammer-0.0.3/docs/img/pulseprogrammer_labeled.png` & `nqrduck_pulseprogrammer-0.0.4/docs/img/pulseprogrammer_labeled.png`

 * *Files identical despite different names*

### Comparing `nqrduck_pulseprogrammer-0.0.3/docs/img/pulseprogrammer_tx_labeled.png` & `nqrduck_pulseprogrammer-0.0.4/docs/img/pulseprogrammer_tx_labeled.png`

 * *Files identical despite different names*

### Comparing `nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/controller.py` & `nqrduck_pulseprogrammer-0.0.4/src/nqrduck_pulseprogrammer/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,66 @@
+"""Controller of  the pulse programmer module."""
+
 import logging
 import json
 import decimal
 from PyQt6.QtCore import pyqtSlot
 from nqrduck.helpers.serializer import DecimalEncoder
 from nqrduck.module.module_controller import ModuleController
 from nqrduck_spectrometer.pulsesequence import PulseSequence
 
 logger = logging.getLogger(__name__)
 
+
 class PulseProgrammerController(ModuleController):
-      
-    def on_loading(self, pulse_parameter_options : dict) -> None:
+    """Controller of the pulse programmer module.
+
+    This class is responsible for handling the logic of the pulse programmer module.
+    """
+
+    def on_loading(self, pulse_parameter_options: dict) -> None:
         """This method is called when the module is loaded. It sets the pulse parameter options in the model.
 
         Args:
             pulse_parameter_options (dict): The pulse parameter options.
         """
         logger.debug("Pulse programmer controller on loading")
         self.module.model.pulse_parameter_options = pulse_parameter_options
 
     @pyqtSlot(str)
-    def delete_event(self, event_name : str) -> None:
+    def delete_event(self, event_name: str) -> None:
         """This method deletes an event from the pulse sequence.
 
         Args:
             event_name (str): The name of the event to be deleted.
         """
         logger.debug("Deleting event %s", event_name)
         for event in self.module.model.pulse_sequence.events:
             if event.name == event_name:
                 self.module.model.pulse_sequence.events.remove(event)
                 break
         self.module.model.events_changed.emit()
 
     @pyqtSlot(str, str)
-    def change_event_name(self, old_name : str, new_name : str) -> None:
+    def change_event_name(self, old_name: str, new_name: str) -> None:
         """This method changes the name of an event.
 
         Args:
             old_name (str): The old name of the event.
             new_name (str): The new name of the event.
         """
         logger.debug("Changing event name from %s to %s", old_name, new_name)
         for event in self.module.model.pulse_sequence.events:
             if event.name == old_name:
                 event.name = new_name
                 break
         self.module.model.events_changed.emit()
 
     @pyqtSlot(str, str)
-    def change_event_duration(self, event_name:str, duration) -> None:
+    def change_event_duration(self, event_name: str, duration) -> None:
         """This method changes the duration of an event.
 
         Args:
             event_name (str): The name of the event.
             duration (str): The new duration of the event.
         """
         logger.debug("Changing duration of event %s to %s", event_name, duration)
@@ -61,50 +68,63 @@
             if event.name == event_name:
                 try:
                     # The u is for microseconds
                     event.duration = duration + "u"
                 except decimal.InvalidOperation:
                     logger.error("Duration must be a positive number")
                     # Emit signal to the nqrduck core to show an error message
-                    self.module.nqrduck_signal.emit("notification", ["Error", "Duration must be a positive number"])
+                    self.module.nqrduck_signal.emit(
+                        "notification", ["Error", "Duration must be a positive number"]
+                    )
                 break
         self.module.model.events_changed.emit()
 
     @pyqtSlot(str)
     def on_move_event_left(self, event_name: str) -> None:
         """This method moves the event one position to the left if possible.
-        
+
         Args:
             event_name (str): The name of the event to be moved.
         """
         logger.debug("Moving event %s to the left", event_name)
         for i, event in enumerate(self.module.model.pulse_sequence.events):
             if event.name == event_name:
                 if i > 0:
-                    self.module.model.pulse_sequence.events[i], self.module.model.pulse_sequence.events[i-1] = self.module.model.pulse_sequence.events[i-1], self.module.model.pulse_sequence.events[i]
+                    (
+                        self.module.model.pulse_sequence.events[i],
+                        self.module.model.pulse_sequence.events[i - 1],
+                    ) = (
+                        self.module.model.pulse_sequence.events[i - 1],
+                        self.module.model.pulse_sequence.events[i],
+                    )
                     break
         self.module.model.events_changed.emit()
 
-
     @pyqtSlot(str)
-    def on_move_event_right(self, event_name : str) -> None:
+    def on_move_event_right(self, event_name: str) -> None:
         """This method moves the event one position to the right if possible.
-        
+
         Args:
             event_name (str): The name of the event to be moved.
         """
         logger.debug("Moving event %s to the right", event_name)
         for i, event in enumerate(self.module.model.pulse_sequence.events):
             if event.name == event_name:
                 if i < len(self.module.model.pulse_sequence.events) - 1:
-                    self.module.model.pulse_sequence.events[i], self.module.model.pulse_sequence.events[i+1] = self.module.model.pulse_sequence.events[i+1], self.module.model.pulse_sequence.events[i]
+                    (
+                        self.module.model.pulse_sequence.events[i],
+                        self.module.model.pulse_sequence.events[i + 1],
+                    ) = (
+                        self.module.model.pulse_sequence.events[i + 1],
+                        self.module.model.pulse_sequence.events[i],
+                    )
                     break
         self.module.model.events_changed.emit()
 
-    def save_pulse_sequence(self, path :str) -> None:
+    def save_pulse_sequence(self, path: str) -> None:
         """This method saves the pulse sequence to a file.
 
         Args:
             path (str): The path to the file.
         """
         logger.debug("Saving pulse sequence to %s", path)
         # Get the name of the file without the extension and without the path
@@ -112,26 +132,27 @@
         self.module.model.pulse_sequence.name = file_name
         logger.debug("Pulse sequence name: %s", self.module.model.pulse_sequence.name)
         self.module.model.pulse_sequence_changed.emit()
 
         sequence = self.module.model.pulse_sequence.to_json()
         with open(path, "w") as file:
             file.write(json.dumps(sequence, cls=DecimalEncoder))
-        
 
-    def load_pulse_sequence(self, path : str) -> None:
+    def load_pulse_sequence(self, path: str) -> None:
         """This method loads a pulse sequence from a file.
 
         Args:
             path (str): The path to the file.
         """
         logger.debug("Loading pulse sequence from %s", path)
         sequence = None
         with open(path) as file:
             sequence = file.read()
 
         sequence = json.loads(sequence)
 
-        loaded_sequence = PulseSequence.load_sequence(sequence, self.module.model.pulse_parameter_options)
-        
+        loaded_sequence = PulseSequence.load_sequence(
+            sequence, self.module.model.pulse_parameter_options
+        )
+
         self.module.model.pulse_sequence = loaded_sequence
-        self.module.model.events_changed.emit()
+        self.module.model.events_changed.emit()
```

### Comparing `nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/model.py` & `nqrduck_pulseprogrammer-0.0.4/src/nqrduck_pulseprogrammer/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,57 @@
+"""Model for the pulse programmer module."""
+
 import logging
 from collections import OrderedDict
 from PyQt6.QtCore import pyqtSignal
 from nqrduck.module.module_model import ModuleModel
 from nqrduck_spectrometer.pulsesequence import PulseSequence
 
 logger = logging.getLogger(__name__)
 
 
 class PulseProgrammerModel(ModuleModel):
+    """Model for the pulse programmer module.
+
+    This class is responsible for storing the data of the pulse programmer module.
+
+    Attributes:
+        FILE_EXTENSION (str): The file extension for pulse programmer files.
+
+    Signals:
+        pulse_parameter_options_changed: Emitted when the pulse parameter options change.
+        events_changed: Emitted when the events in the pulse sequence change.
+        pulse_sequence_changed: Emitted when the pulse sequence changes.
+    """
+
+    FILE_EXTENSION = "quack"
+
     pulse_parameter_options_changed = pyqtSignal()
     events_changed = pyqtSignal()
     pulse_sequence_changed = pyqtSignal()
 
     def __init__(self, module):
+        """Initializes the pulse programmer model.
+
+        Args:
+            module (Module): The module to which this model belongs.
+        """
         super().__init__(module)
         self.pulse_parameter_options = OrderedDict()
         self.pulse_sequence = PulseSequence("Untitled pulse sequence")
 
     def add_event(self, event_name: str, duration: float = 20):
         """Add a new event to the current pulse sequence.
 
         Args:
             event_name (str): A human-readable name for the event
             duration (float): The duration of the event in µs. Defaults to 20.
         """
         self.pulse_sequence.events.append(
-            PulseSequence.Event(event_name, "%.16gu" % float(duration))
+            PulseSequence.Event(event_name, f"{float(duration):.16g}u")
         )
         logger.debug(
             "Creating event %s with object id %s",
             event_name,
             id(self.pulse_sequence.events[-1]),
         )
 
@@ -46,23 +68,25 @@
             )
 
         logger.debug(self.pulse_sequence.to_json())
         self.events_changed.emit()
 
     @property
     def pulse_parameter_options(self):
+        """dict: The pulse parameter options."""
         return self._pulse_parameter_options
 
     @pulse_parameter_options.setter
     def pulse_parameter_options(self, value):
         self._pulse_parameter_options = value
         logger.debug("Pulse parameter options changed - emitting signal")
         self.pulse_parameter_options_changed.emit()
 
     @property
     def pulse_sequence(self):
+        """PulseSequence: The pulse sequence."""
         return self._pulse_sequence
 
     @pulse_sequence.setter
     def pulse_sequence(self, value):
         self._pulse_sequence = value
         self.pulse_sequence_changed.emit()
```

### Comparing `nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/view.py` & `nqrduck_pulseprogrammer-0.0.4/src/nqrduck_pulseprogrammer/view.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""This module contains the view for the pulse programmer module. It is responsible for displaying the pulse sequence and the pulse parameter options."""
+
 import logging
 import functools
 from PyQt6.QtGui import QValidator
 from PyQt6.QtWidgets import (
     QFormLayout,
     QTableWidget,
     QVBoxLayout,
@@ -9,15 +11,14 @@
     QHBoxLayout,
     QLabel,
     QDialog,
     QLineEdit,
     QDialogButtonBox,
     QWidget,
     QToolButton,
-    QFileDialog,
     QSizePolicy,
 )
 from PyQt6.QtCore import pyqtSlot, pyqtSignal
 from nqrduck.module.module_view import ModuleView
 from nqrduck.assets.icons import Logos
 from nqrduck.helpers.duckwidgets import DuckFloatEdit, DuckEdit
 from nqrduck_spectrometer.pulseparameters import (
@@ -25,25 +26,29 @@
     NumericOption,
     FunctionOption,
 )
 from nqrduck.helpers.formbuilder import (
     DuckFormBuilder,
     DuckFormFunctionSelectionField,
     DuckFormCheckboxField,
-    DuckFormDropdownField,
     DuckFormFloatField,
-    DuckFormIntField,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class PulseProgrammerView(ModuleView):
+    """View for the pulse programmer module."""
 
     def __init__(self, module):
+        """Initializes the pulse programmer view.
+
+        Args:
+            module (Module): The module to which this view belongs.
+        """
         super().__init__(module)
 
         self.setup_pulsetable()
 
         self.setup_variabletables()
 
         logger.debug(
@@ -54,19 +59,17 @@
         )
 
     def setup_variabletables(self) -> None:
         """Setup the table for the variables."""
         pass
 
     def setup_pulsetable(self) -> None:
-        """Setup the table for the pulse sequence. Also add buttons for saving and loading pulse sequences and editing and creation of events"""
+        """Setup the table for the pulse sequence. Also add buttons for saving and loading pulse sequences and editing and creation of events."""
         # Create pulse table
-        self.title = QLabel(
-            "Pulse Sequence: %s" % self.module.model.pulse_sequence.name
-        )
+        self.title = QLabel(f"Pulse Sequence: {self.module.model.pulse_sequence.name}")
         # Make title bold
         font = self.title.font()
         font.setBold(True)
         self.title.setFont(font)
 
         # Table setup
         self.pulse_table = QTableWidget(self)
@@ -129,15 +132,15 @@
 
     @pyqtSlot()
     def on_pulse_sequence_changed(self) -> None:
         """This method is called whenever the pulse sequence changes. It updates the view to reflect the changes."""
         logger.debug(
             "Updating pulse sequence to %s", self.module.model.pulse_sequence.name
         )
-        self.title.setText("Pulse Sequence: %s" % self.module.model.pulse_sequence.name)
+        self.title.setText(f"Pulse Sequence: {self.module.model.pulse_sequence.name}")
 
     @pyqtSlot()
     def on_pulse_parameter_options_changed(self) -> None:
         """This method is called whenever the pulse parameter options change. It updates the view to reflect the changes."""
         logger.debug(
             "Updating pulse parameter options to %s",
             self.module.model.pulse_parameter_options.keys(),
@@ -173,17 +176,15 @@
         event_layout = QVBoxLayout()
         event_parameters_label = QLabel("Event lengths:")
         event_layout.addWidget(event_parameters_label)
 
         for event in self.module.model.pulse_sequence.events:
             logger.debug("Adding event to pulseprogrammer view: %s", event.name)
             # Create a label for the event
-            event_label = QLabel(
-                "%s : %.16g µs" % (event.name, (event.duration * 1e6))
-            )
+            event_label = QLabel(f"{event.name} : {event.duration * 1e6:.16g} µs")
             event_layout.addWidget(event_label)
 
         # Delete the old widget and create a new one
         self.event_widget.deleteLater()
         self.event_widget = QWidget()
         self.event_widget.setLayout(event_layout)
         self.layout().addWidget(self.event_widget)
@@ -256,15 +257,22 @@
                 func = functools.partial(
                     self.on_table_button_clicked, event=event, parameter=parameter
                 )
                 button.clicked.connect(func)
 
     @pyqtSlot()
     def on_table_button_clicked(self, event, parameter) -> None:
-        """This method is called whenever a button in the pulse table is clicked. It opens a dialog to set the options for the parameter."""
+        """This method is called whenever a button in the pulse table is clicked.
+
+        It opens a dialog to set the options for the parameter.
+
+        Args:
+            event (PulseSequence.Event): The event for which the parameter options should be set.
+            parameter (str): The name of the parameter for which the options should be set.
+        """
         logger.debug("Button for event %s and parameter %s clicked", event, parameter)
         # Create a QDialog to set the options for the parameter.
         description = f"Set options for {parameter}"
         dialog = DuckFormBuilder(parameter, description=description, parent=self)
 
         # Adding fields for the options
         form_options = []
@@ -325,43 +333,61 @@
 
             self.set_parameter_icons()
 
     @pyqtSlot()
     def on_save_button_clicked(self) -> None:
         """This method is called whenever the save button is clicked. It opens a dialog to select a file to save the pulse sequence to."""
         logger.debug("Save button clicked")
-        file_manager = QFileManager(self)
+        file_manager = self.FileManager(self.module.model.FILE_EXTENSION, parent=self)
         file_name = file_manager.saveFileDialog()
         if file_name:
             self.module.controller.save_pulse_sequence(file_name)
 
     @pyqtSlot()
     def on_load_button_clicked(self) -> None:
         """This method is called whenever the load button is clicked. It opens a dialog to select a file to load the pulse sequence from."""
         logger.debug("Load button clicked")
-        file_manager = QFileManager(self)
+        file_manager = self.FileManager(self.module.model.FILE_EXTENSION, parent=self)
         file_name = file_manager.loadFileDialog()
         if file_name:
-            self.module.controller.load_pulse_sequence(file_name)
+            try:
+                self.module.controller.load_pulse_sequence(file_name)
+            except KeyError:
+                self.module.nqrduck_signal.emit(
+                    "notification",
+                    [
+                        "Error",
+                        "Error loading pulse sequence -  maybe the version of the pulse sequence is not compatible?",
+                    ],
+                )
 
 
 class EventOptionsWidget(QWidget):
     """This class is a widget that can be used to set the options for a pulse parameter.
+
     This widget is then added to the the first row of the according event column in the pulse table.
     It has a edit button that opens a dialog that allows the user to change the options for the event (name and duration).
     Furthermore it has a delete button that deletes the event from the pulse sequence.
+
+    Signals:
+        delete_event: Emitted when the delete button is clicked.
+        change_event_duration: Emitted when the duration of the event is changed.
+        change_event_name: Emitted when the name of the event is changed.
+        move_event_left: Emitted when the move left button is clicked.
+        move_event_right: Emitted when the move right button is clicked.
     """
 
     delete_event = pyqtSignal(str)
     change_event_duration = pyqtSignal(str, str)
     change_event_name = pyqtSignal(str, str)
     move_event_left = pyqtSignal(str)
     move_event_right = pyqtSignal(str)
 
     def __init__(self, event):
+        """Initializes the EventOptionsWidget."""
         super().__init__()
         self.event = event
 
         layout = QVBoxLayout()
         upper_layout = QHBoxLayout()
         # Edit button
         self.edit_button = QToolButton()
@@ -407,23 +433,24 @@
 
         self.setLayout(layout)
         self.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding)
 
     @pyqtSlot()
     def edit_event(self) -> None:
         """This method is called when the edit button is clicked. It opens a dialog that allows the user to change the event name and duration.
+
         If the user clicks ok, the change_event_name and change_event_duration signals are emitted.
         """
         logger.debug("Edit button clicked for event %s", self.event.name)
 
         # Create a QDialog to edit the event
         dialog = QDialog(self)
         dialog.setWindowTitle("Edit event")
         layout = QVBoxLayout()
-        label = QLabel("Edit event %s" % self.event.name)
+        label = QLabel(f"Edit event {self.event.name}")
         layout.addWidget(label)
 
         # Create the inputs for event name, duration
         event_form_layout = QFormLayout()
         name_label = QLabel("Name:")
         name_lineedit = QLineEdit(self.event.name)
         event_form_layout.addRow(name_label, name_lineedit)
@@ -453,23 +480,25 @@
             if duration_lineedit.text() != str(self.event.duration):
                 self.change_event_duration.emit(
                     self.event.name, duration_lineedit.text()
                 )
 
     @pyqtSlot()
     def create_delete_event_dialog(self) -> None:
-        """This method is called when the delete button is clicked. It creates a dialog that asks the user if he is sure he wants to delete the event.
+        """This method is called when the delete button is clicked.
+
+        It creates a dialog that asks the user if he is sure he wants to delete the event.
         If the user clicks yes, the delete_event signal is emitted.
         """
         # Create an 'are you sure' dialog
         logger.debug("Delete button clicked")
         dialog = QDialog(self)
         dialog.setWindowTitle("Delete event")
         layout = QVBoxLayout()
-        label = QLabel("Are you sure you want to delete event %s?" % self.event.name)
+        label = QLabel(f"Are you sure you want to delete event {self.event.name}?")
         layout.addWidget(label)
         buttons = QDialogButtonBox(
             QDialogButtonBox.StandardButton.Yes | QDialogButtonBox.StandardButton.No
         )
         buttons.accepted.connect(dialog.accept)
         buttons.rejected.connect(dialog.reject)
         layout.addWidget(buttons)
@@ -490,14 +519,15 @@
         self.move_event_right.emit(self.event.name)
 
 
 class AddEventDialog(QDialog):
     """This dialog is created whenever a new event is added to the pulse sequence. It allows the user to enter a name for the event."""
 
     def __init__(self, parent=None):
+        """Initializes the AddEventDialog."""
         super().__init__(parent)
 
         self.setWindowTitle("Add Event")
 
         self.layout = QFormLayout(self)
 
         self.name_layout = QHBoxLayout()
@@ -540,18 +570,18 @@
 
         Returns:
         str: The name entered by the user
         """
         return self.name_input.text()
 
     def get_duration(self) -> float:
-        """Returns the duration entered by the user, or a fallback value."
+        """Returns the duration entered by the user, or a fallback value.
 
         Returns:
-        float: The duration value provided by the user, or 20
+            float: The duration value provided by the user, or 20
         """
         return self.duration_lineedit.text() or 20
 
     def check_input(self) -> None:
         """Checks if the name and duration entered by the user is valid. If it is, the dialog is accepted. If not, the user is informed of the error."""
         if (
             self.duration_lineedit.validator.validate(self.duration_lineedit.text(), 0)[
@@ -589,54 +619,7 @@
                     .parent()
                     .module.model.pulse_sequence.events
                 ]
             ):
                 return (QValidator.State.Invalid, value, position)
 
             return (QValidator.State.Acceptable, value, position)
-
-
-# This class should be refactored in the module view so it can be used by all modules
-class QFileManager:
-    """This class provides methods for opening and saving files."""
-
-    def __init__(self, parent=None):
-        self.parent = parent
-
-    def loadFileDialog(self) -> str:
-        """Opens a file dialog for the user to select a file to open.
-
-        Returns:
-            str: The path of the file selected by the user.
-        """
-        fileName, _ = QFileDialog.getOpenFileName(
-            self.parent,
-            "QFileManager - Open File",
-            "",
-            "Quack Files (*.quack);;All Files (*)",
-            options=QFileDialog.Option.ReadOnly,
-        )
-        if fileName:
-            return fileName
-        else:
-            return None
-
-    def saveFileDialog(self) -> str:
-        """Opens a file dialog for the user to select a file to save.
-
-        Returns:
-            str: The path of the file selected by the user.
-        """
-        fileName, _ = QFileDialog.getSaveFileName(
-            self.parent,
-            "QFileManager - Save File",
-            "",
-            "Quack Files (*.quack);;All Files (*)",
-            options=QFileDialog.Option.DontUseNativeDialog,
-        )
-        if fileName:
-            # Append the .quack extension if not present
-            if not fileName.endswith(".quack"):
-                fileName += ".quack"
-            return fileName
-        else:
-            return None
```

### Comparing `nqrduck_pulseprogrammer-0.0.3/LICENSE` & `nqrduck_pulseprogrammer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nqrduck_pulseprogrammer-0.0.3/README.md` & `nqrduck_pulseprogrammer-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nqrduck_pulseprogrammer-0.0.3/pyproject.toml` & `nqrduck_pulseprogrammer-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nqrduck-pulseprogrammer"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="jupfi", email="support@nqrduck.cool" },
 ]
 
 description = "A module for the NQRduck program (a simple python script™) to do pulse programming."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `nqrduck_pulseprogrammer-0.0.3/PKG-INFO` & `nqrduck_pulseprogrammer-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nqrduck-pulseprogrammer
-Version: 0.0.3
+Version: 0.0.4
 Summary: A module for the NQRduck program (a simple python script™) to do pulse programming.
 Project-URL: Homepage, https://nqrduck.cool
 Project-URL: Bug Tracker, https://github.com/nqrduck/nqrduck-pulseprogrammer/issues
 Project-URL: Source Code, https://github.com/nqrduck/nqrduck-pulseprogrammer
 Author-email: jupfi <support@nqrduck.cool>
 License: MIT License
```

