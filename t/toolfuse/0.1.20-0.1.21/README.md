# Comparing `tmp/toolfuse-0.1.20.tar.gz` & `tmp/toolfuse-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolfuse-0.1.20.tar", max compression
+gzip compressed data, was "toolfuse-0.1.21.tar", max compression
```

## Comparing `toolfuse-0.1.20.tar` & `toolfuse-0.1.21.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1065 2024-04-08 15:50:27.204544 toolfuse-0.1.20/LICENSE
--rw-r--r--   0        0        0     3333 2024-04-08 16:29:21.395807 toolfuse-0.1.20/README.md
--rw-r--r--   0        0        0      803 2024-05-03 14:54:55.333238 toolfuse-0.1.20/pyproject.toml
--rw-r--r--   0        0        0      341 2024-04-08 15:50:27.209682 toolfuse-0.1.20/toolfuse/__init__.py
--rw-r--r--   0        0        0    24683 2024-05-03 14:54:29.536468 toolfuse-0.1.20/toolfuse/base.py
--rw-r--r--   0        0        0      197 2024-04-27 21:02:03.126589 toolfuse-0.1.20/toolfuse/models.py
--rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 toolfuse-0.1.20/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 15:50:27.204544 toolfuse-0.1.21/LICENSE
+-rw-r--r--   0        0        0     3333 2024-04-08 16:29:21.395807 toolfuse-0.1.21/README.md
+-rw-r--r--   0        0        0      803 2024-05-05 02:33:54.568795 toolfuse-0.1.21/pyproject.toml
+-rw-r--r--   0        0        0      341 2024-04-08 15:50:27.209682 toolfuse-0.1.21/toolfuse/__init__.py
+-rw-r--r--   0        0        0    29844 2024-05-05 02:28:00.102882 toolfuse-0.1.21/toolfuse/base.py
+-rw-r--r--   0        0        0      197 2024-04-27 21:02:03.126589 toolfuse-0.1.21/toolfuse/models.py
+-rw-r--r--   0        0        0      996 2024-05-05 02:09:19.322511 toolfuse-0.1.21/toolfuse/multi.py
+-rw-r--r--   0        0        0      567 2024-05-04 18:04:39.119408 toolfuse-0.1.21/toolfuse/util.py
+-rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 toolfuse-0.1.21/PKG-INFO
```

### Comparing `toolfuse-0.1.20/LICENSE` & `toolfuse-0.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.20/README.md` & `toolfuse-0.1.21/README.md`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.20/pyproject.toml` & `toolfuse-0.1.21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "toolfuse"
-version = "0.1.20"
+version = "0.1.21"
 description = "Tools for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "toolfuse"}]
 
 [tool.poetry.dependencies]
```

### Comparing `toolfuse-0.1.20/toolfuse/base.py` & `toolfuse-0.1.21/toolfuse/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -266,33 +266,39 @@
         """
         if not isinstance(observation, Observation):
             raise ValueError(
                 "Actions are not observable. Use the 'use' method to perform an action."
             )
         return observation(*args, **kwargs)
 
-    def json_schema(self, actions_only: bool = False) -> List[Dict[str, Any]]:
+    def json_schema(
+        self, actions_only: bool = False, exclude_names: List[str] = []
+    ) -> List[Dict[str, Any]]:
         """
-        Returns a list of JSON schemas representing the tool's actions.
+        Returns a list of JSON schemas representing the tool's actions and, optionally, observations,
+        excluding any actions or observations with names listed in 'exclude_names'.
 
-        Each schema provides a structured description of an action's interface, including its name,
+        Each schema provides a structured description of an action's or observation's interface, including its name,
         expected arguments, and other metadata.
 
         Args:
             actions_only (bool, optional): If True, only the action schemas will be returned. Defaults to False.
+            exclude_names (List[str], optional): A list of action or observation names to exclude from the schema output.
 
         Returns:
-            List[Dict[str, Any]]: A list of dictionaries, each representing the JSON schema of an action.
+            List[Dict[str, Any]]: A list of dictionaries, each representing the JSON schema of an action or observation not excluded.
         """
         out = []
         for action in self.actions():
-            out.append(action.schema)
+            if action.name not in exclude_names:
+                out.append(action.schema)
         if not actions_only:
             for observation in self.observations():
-                out.append(observation.schema)
+                if observation.name not in exclude_names:
+                    out.append(observation.schema)
         return out
 
     def find_action(self, name: str) -> Optional[Action]:
         """
         Searches for an action or observation by name and returns it if found.
 
         This method checks both the actions and observations lists for a match.
@@ -342,14 +348,143 @@
         module = getmodule(self)
         if not module:
             raise ValueError("Tool not associated with a module")
         mod_parts = module.__name__.split(".")
         version = pkgversion(mod_parts[0])
         return V1ToolRef(module=module.__name__, name=self.name(), version=version)
 
+    def add_action(self, method: Callable) -> None:
+        """
+        Adds a new action to the tool using only the method provided. Name, schema,
+        and description are derived automatically.
+
+        Args:
+            method (Callable): The callable method that implements the action.
+        """
+        name = method.__name__
+        schema = self._generate_schema(
+            method
+        )  # Assuming a method to generate schema automatically
+        description = self._parse_docstring(method)
+
+        action = Action(name, method, schema, description)
+        self._actions_list.append(action)
+
+    def add_observation(self, method: Callable) -> None:
+        """
+        Adds a new observation to the tool using only the method provided. Name, schema,
+        and description are derived automatically.
+
+        Args:
+            method (Callable): The callable method that implements the observation.
+        """
+        name = method.__name__
+        schema = self._generate_schema(
+            method
+        )  # Assuming a method to generate schema automatically
+        description = self._parse_docstring(method)
+
+        observation = Observation(name, method, schema, description)
+        self._observations_list.append(observation)
+
+    def _generate_schema(self, method: Callable) -> Dict[str, Any]:
+        """
+        Generates a schema based on the method signature. This can be as simple or as
+        complex as needed depending on how parameters are to be handled.
+
+        Args:
+            method (Callable): The method for which to generate a schema.
+
+        Returns:
+            Dict[str, Any]: A schema representing the parameters and their types.
+        """
+        # Example implementation using inspect to generate parameter types
+        params = inspect.signature(method).parameters
+        return {param: str(ptype.annotation) for param, ptype in params.items()}
+
+    def add_actions(self, methods: List[Callable]) -> None:
+        """
+        Adds multiple actions to the tool using a list of methods. Each method's name, schema,
+        and description are derived automatically.
+
+        Args:
+            methods (List[Callable]): A list of callable methods that implement actions.
+        """
+        for method in methods:
+            self.add_action(method)
+
+    def add_observations(self, methods: List[Callable]) -> None:
+        """
+        Adds multiple observations to the tool using a list of methods. Each method's name, schema,
+        and description are derived automatically.
+
+        Args:
+            methods (List[Callable]): A list of callable methods that implement observations.
+        """
+        for method in methods:
+            self.add_observation(method)
+
+    def _add_action(
+        self,
+        method: Callable,
+        name: Optional[str] = None,
+        schema: Optional[Dict] = None,
+        description: Optional[str] = None,
+    ) -> None:
+        """
+        Adds a new action to the tool using the provided method.
+        If the action with the same name already exists, it won't add it again.
+        """
+        if not name:
+            name = method.__name__
+        if any(action.name == name for action in self._actions_list):
+            return  # Prevent duplicate actions
+        action = Action(
+            name, method, schema or {}, description or self._parse_docstring(method)
+        )
+        self._actions_list.append(action)
+
+    def _add_observation(
+        self,
+        method: Callable,
+        name: Optional[str] = None,
+        schema: Optional[Dict] = None,
+        description: Optional[str] = None,
+    ) -> None:
+        """
+        Adds a new observation to the tool using the provided method.
+        """
+        if not name:
+            name = method.__name__
+        if any(obs.name == name for obs in self._observations_list):
+            return  # Prevent duplicate observations
+        observation = Observation(
+            name, method, schema or {}, description or self._parse_docstring(method)
+        )
+        self._observations_list.append(observation)
+
+    def merge(self, other: "Tool") -> None:
+        """
+        Merges the actions and observations from another tool into this tool.
+
+        Args:
+            other (Tool): The tool to merge into this tool.
+        """
+        for action in other.actions():
+            self._add_action(
+                action.method, action.name, action.schema, action.description
+            )
+        for observation in other.observations():
+            self._add_observation(
+                observation.method,
+                observation.name,
+                observation.schema,
+                observation.description,
+            )
+
 
 def tool_from_cls(cls: Type[T]) -> Type[Tool]:
     """
     Dynamically creates a subclass of `Tool` that integrates methods from a given class `cls` as actions.
 
     Args:
         cls (Type[T]): The class from which to create a Tool, integrating its methods as actions.
```

### Comparing `toolfuse-0.1.20/PKG-INFO` & `toolfuse-0.1.21/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolfuse
-Version: 0.1.20
+Version: 0.1.21
 Summary: Tools for AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

