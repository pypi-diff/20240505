# Comparing `tmp/hydra-ui-1.0.0.tar.gz` & `tmp/hydra-ui-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydra-ui-1.0.0.tar", last modified: Fri Feb 16 15:45:46 2024, max compression
+gzip compressed data, was "hydra-ui-1.1.0.tar", last modified: Sun May  5 17:09:36 2024, max compression
```

## Comparing `hydra-ui-1.0.0.tar` & `hydra-ui-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 rweathers  (1000) rweathers  (1000)        0 2024-02-16 15:45:46.222350 hydra-ui-1.0.0/
--rw-r--r--   0 rweathers  (1000) rweathers  (1000)      560 2024-02-16 15:45:46.214350 hydra-ui-1.0.0/PKG-INFO
--rw-r--r--   0 rweathers  (1000) rweathers  (1000)    36433 2024-02-16 14:37:57.000000 hydra-ui-1.0.0/hydra.py
-drwxr-xr-x   0 rweathers  (1000) rweathers  (1000)        0 2024-02-16 15:45:46.214350 hydra-ui-1.0.0/hydra_ui.egg-info/
--rw-r--r--   0 rweathers  (1000) rweathers  (1000)      560 2024-02-16 15:45:45.000000 hydra-ui-1.0.0/hydra_ui.egg-info/PKG-INFO
--rw-r--r--   0 rweathers  (1000) rweathers  (1000)      145 2024-02-16 15:45:46.000000 hydra-ui-1.0.0/hydra_ui.egg-info/SOURCES.txt
--rw-r--r--   0 rweathers  (1000) rweathers  (1000)        1 2024-02-16 15:45:45.000000 hydra-ui-1.0.0/hydra_ui.egg-info/dependency_links.txt
--rw-r--r--   0 rweathers  (1000) rweathers  (1000)        6 2024-02-16 15:45:45.000000 hydra-ui-1.0.0/hydra_ui.egg-info/top_level.txt
--rw-r--r--   0 rweathers  (1000) rweathers  (1000)       38 2024-02-16 15:45:46.222350 hydra-ui-1.0.0/setup.cfg
--rw-r--r--   0 rweathers  (1000) rweathers  (1000)      601 2024-02-16 14:38:14.000000 hydra-ui-1.0.0/setup.py
+drwxr-xr-x   0 rweathers  (1000) rweathers  (1000)        0 2024-05-05 17:09:36.770106 hydra-ui-1.1.0/
+-rw-r--r--   0 rweathers  (1000) rweathers  (1000)      758 2024-05-05 17:09:36.770106 hydra-ui-1.1.0/PKG-INFO
+-rw-r--r--   0 rweathers  (1000) rweathers  (1000)    40874 2024-05-05 16:50:32.000000 hydra-ui-1.1.0/hydra.py
+drwxr-xr-x   0 rweathers  (1000) rweathers  (1000)        0 2024-05-05 17:09:36.770106 hydra-ui-1.1.0/hydra_ui.egg-info/
+-rw-r--r--   0 rweathers  (1000) rweathers  (1000)      758 2024-05-05 17:09:36.000000 hydra-ui-1.1.0/hydra_ui.egg-info/PKG-INFO
+-rw-r--r--   0 rweathers  (1000) rweathers  (1000)      145 2024-05-05 17:09:36.000000 hydra-ui-1.1.0/hydra_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 rweathers  (1000) rweathers  (1000)        1 2024-05-05 17:09:36.000000 hydra-ui-1.1.0/hydra_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 rweathers  (1000) rweathers  (1000)        6 2024-05-05 17:09:36.000000 hydra-ui-1.1.0/hydra_ui.egg-info/top_level.txt
+-rw-r--r--   0 rweathers  (1000) rweathers  (1000)       38 2024-05-05 17:09:36.770106 hydra-ui-1.1.0/setup.cfg
+-rw-r--r--   0 rweathers  (1000) rweathers  (1000)      827 2024-05-05 17:08:28.000000 hydra-ui-1.1.0/setup.py
```

### Comparing `hydra-ui-1.0.0/PKG-INFO` & `hydra-ui-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: hydra-ui
-Version: 1.0.0
+Version: 1.1.0
 Summary: A framework for developing hybrid CLI/GUI programs.
 Home-page: https://github.com/rweathers/hydra
 Author: Ryan Weathers
 Author-email: ryanweathers63@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
+Description-Content-Type: text/x-rst
+
+Hydra is a framework for developing hybrid CLI/GUI programs in Python. It is a lightweight wrapper around Tk and is pure Python, with no external dependencies.
```

### Comparing `hydra-ui-1.0.0/hydra.py` & `hydra-ui-1.1.0/hydra.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 # 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
-# Version: 1.0.0 (2024-02-16)
+# Version: 1.1.0 (2024-05-05)
 ################################################################################
 
 import csv
 import configparser
 import decimal
 import glob
 import os
@@ -276,14 +276,71 @@
 		"""
 		if not self.inputs["quiet"]:
 			p = progress(self.last_update, text, started, processed, total)
 			if p is not None:
 				self.last_update = p[0]
 				print(p[1].ljust(self.twidth)[0:self.twidth], end="\r", flush=True)
 	
+	def user_message(self, message):
+		"""Show a message to the user.
+		
+		Paramaters:
+			message - Message text.
+		"""
+		print(message)
+		_ = input("Press enter to continue...")
+		
+	def user_warning(self, message):
+		"""Show a warning message to the user.
+		
+		Paramaters:
+			message - Message text.
+		"""
+		print("WARNING:", message)
+		_ = input("Press enter to continue...")
+		
+	def user_error(self, message):
+		"""Show an error message to the user.
+		
+		Paramaters:
+			message - Message text.
+		"""
+		print("ERROR:", message)
+		_ = input("Press enter to continue...")
+	
+	def user_confirm(self, message, include_cancel=False):
+		"""Ask the user for confirmation and return True, False or None.
+		
+		Paramaters:
+			message - Message text.
+			include_cancel - Flag to enable the cancel option.
+		"""
+		if include_cancel: message += " ([y]es/[n]o/[c]ancel): "
+		else: message += " ([y]es/[n]o): "
+		
+		while True:
+			response = input(message)
+			if response[0:1].lower() == "y": return True
+			elif response[0:1].lower() == "n": return False
+			elif (response[0:1].lower() == "c") and include_cancel: return None
+	
+	def user_input(self, message, default=""):
+		"""Ask the user for a value and return it.
+		
+		Paramaters:
+			message - Message text.
+			default - A default value.
+		"""
+		if default == "": message = "{}: ".format(message)
+		else: message = "{} [default={}]: ".format(message, default)
+		
+		response = input(message)
+		if (response == "") and (default != ""): response = default
+		return response
+	
 	def get_action(self, inputs):
 		"""Return the BaseAction subclass to use.
 		
 		Parameters:
 			inputs - User input dictionary.
 		"""
 		pass
@@ -298,15 +355,15 @@
 			elif self.inputs["license"]:
 				self.print_license()
 			else:
 				if not self.inputs["quiet"]: print("")
 				
 				action = self.get_action(self.inputs)
 				try:
-					action = action(self.inputs, self.output_progress)
+					action = action(self.inputs, self.output_progress, self.user_message, self.user_warning, self.user_error, self.user_confirm, self.user_input, "cli")
 				except TypeError as e:
 					raise TypeError("{}.get_action must return a subclass of BaseAction, received: {}".format(self.__class__.__name__, action))
 				message = action.execute()
 				
 				if not self.inputs["quiet"]:
 					self.output_progress("")
 					print(message)
@@ -317,14 +374,24 @@
 			print("")
 			if self.inputs.get("verbose", False):
 				import traceback
 				print(traceback.format_exc())
 			
 			error_output(e, self.prog["error"])
 
+class InputDialog(tk.simpledialog._QueryString):
+	"""Dialog with only an Ok button."""
+	def buttonbox(self):
+		box = tk.Frame(self)
+		w = tk.Button(box, text="OK", width=10, command=self.ok, default=tk.ACTIVE)
+		w.pack(side=tk.LEFT, padx=5, pady=5)
+		self.bind("<Return>", self.ok)
+		self.bind("<Escape>", self.cancel)
+		box.pack()
+
 class BaseGUI(tk.Frame):
 	"""Base class for defining the graphical user interface.
 	
 	Attributes:
 		prog - Program constants dictionary.
 		conf - Configuration dictionary.
 		icon - Base-64 encoded string representing the icon.
@@ -986,14 +1053,59 @@
 		"""
 		p = progress(self.last_update, text, started, processed, total)
 		if p is not None:
 			self.last_update = p[0]
 			self.widgets["progress"].setval(p[1])
 			self.update()
 	
+	def user_message(self, message):
+		"""Show a message to the user.
+		
+		Paramaters:
+			message - Message text.
+		"""
+		tk.messagebox.showinfo("Information", message)
+	
+	def user_warning(self, message):
+		"""Show a warning message to the user.
+		
+		Paramaters:
+			message - Message text.
+		"""
+		tk.messagebox.showwarning("Warning", message)
+		
+	def user_error(self, message):
+		"""Show an error message to the user.
+		
+		Paramaters:
+			message - Message text.
+		"""
+		tk.messagebox.showerror("Error", message)
+	
+	def user_confirm(self, message, include_cancel=False):
+		"""Ask the user for confirmation and return True, False or None.
+		
+		Paramaters:
+			message - Message text.
+			include_cancel - Flag to enable the cancel option.
+		"""
+		if include_cancel: return tk.messagebox.askyesnocancel("Confirm", message)
+		else: return tk.messagebox.askyesno("Confirm", message)	
+	
+	def user_input(self, message, default=""):
+		"""Ask the user for a value and return it.
+		
+		Paramaters:
+			message - Message text.
+			default - A default value.
+		"""
+		while True:
+			response = InputDialog("Input", message, initialvalue=default, parent=self).result
+			if response is not None: return response
+	
 	def get_action(self, inputs):
 		"""Return the BaseAction subclass to use.
 		
 		Parameters:
 			inputs - User input dictionary.
 		"""
 		pass
@@ -1005,15 +1117,15 @@
 			self.disable_widgets()
 			
 			inputs = self.conf.copy()
 			for name in self.widgets: inputs[name] = self.widgets[name].getval()
 			
 			action = self.get_action(inputs)
 			try:
-				action = action(inputs, self.set_progress)
+				action = action(inputs, self.set_progress, self.user_message, self.user_warning, self.user_error, self.user_confirm, self.user_input, "gui")
 			except TypeError as e:
 				raise TypeError("{}.get_action must return a subclass of BaseAction, received: {}".format(self.__class__.__name__, action))
 			message = action.execute()
 			
 			self.config(cursor="")
 			tk.messagebox.showinfo("Success", message)
 			self.widgets["progress"].setval("")
@@ -1029,25 +1141,43 @@
 
 class BaseAction:
 	"""Base class for defining actions.
 	
 	Attributes:
 		inputs - User input dictionary.
 		progress - Callback function for user progress updates.
+		user_message - Callback function for user messages.
+		user_warning - Callback function for user warnings.
+		user_error - Callback function for user errors.
+		user_confirm - Callback function for user confirmations.
+		user_input - Callback function for user input.
+		interface - Defines the interface used to execute the action.
 	"""
 	
-	def __init__(self, inputs, progress=None):
+	def __init__(self, inputs, progress=None, user_message=None, user_warning=None, user_error=None, user_confirm=None, user_input=None, interface=None):
 		"""Initialize the object.
 		
 		Parameters:
 			inputs - User input dictionary.
 			progress - Callback function for user progress updates.
+			user_message - Callback function for user messages.
+			user_warning - Callback function for user warnings.
+			user_error - Callback function for user errors.
+			user_confirm - Callback function for user confirmations.
+			user_input - Callback function for user input.
+			interface - Defines the interface used to execute the action.
 		"""
 		self.inputs = inputs
 		self.progress = progress if progress is not None else lambda *_: None
+		self.user_message = user_message if user_message is not None else lambda *_: None
+		self.user_warning = user_warning if user_warning is not None else lambda *_: None
+		self.user_error = user_error if user_error is not None else lambda *_: None
+		self.user_confirm = user_confirm if user_confirm is not None else lambda *_: None
+		self.user_input = user_input if user_input is not None else lambda *_: None
+		self.interface = interface
 	
 	def standardize(self):
 		"""Standardize the user's inputs."""
 		pass
 	
 	def validate(self):
 		"""Raise an exception if any of the user's inputs are invalid."""
```

### Comparing `hydra-ui-1.0.0/hydra_ui.egg-info/PKG-INFO` & `hydra-ui-1.1.0/hydra_ui.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: hydra-ui
-Version: 1.0.0
+Version: 1.1.0
 Summary: A framework for developing hybrid CLI/GUI programs.
 Home-page: https://github.com/rweathers/hydra
 Author: Ryan Weathers
 Author-email: ryanweathers63@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
+Description-Content-Type: text/x-rst
+
+Hydra is a framework for developing hybrid CLI/GUI programs in Python. It is a lightweight wrapper around Tk and is pure Python, with no external dependencies.
```

### Comparing `hydra-ui-1.0.0/setup.py` & `hydra-ui-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from setuptools import setup
 
 setup(
 	name="hydra-ui",
-	version="1.0.0",
+	version="1.1.0",
 	description="A framework for developing hybrid CLI/GUI programs.",
+	long_description="Hydra is a framework for developing hybrid CLI/GUI programs in Python. It is a lightweight wrapper around Tk and is pure Python, with no external dependencies.",
+	long_description_content_type="text/x-rst",
 	url="https://github.com/rweathers/hydra",
 	author="Ryan Weathers",
 	author_email="ryanweathers63@gmail.com",
 	license="GPLv3+",
 	classifiers=[
 		"Development Status :: 5 - Production/Stable",
 		"Intended Audience :: Developers",
```

