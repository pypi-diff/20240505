# Comparing `tmp/shellcrafter-1.1.2.tar.gz` & `tmp/shellcrafter-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellcrafter-1.1.2.tar", last modified: Sun Apr 28 12:33:39 2024, max compression
+gzip compressed data, was "shellcrafter-1.1.3.tar", last modified: Sun May  5 01:32:42 2024, max compression
```

## Comparing `shellcrafter-1.1.2.tar` & `shellcrafter-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:33:39.181477 shellcrafter-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-28 12:33:39.177477 shellcrafter-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:33:39.181477 shellcrafter-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:33:39.177477 shellcrafter-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:33:39.177477 shellcrafter-1.1.2/src/shellcrafter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/src/shellcrafter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/src/shellcrafter/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13367 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/src/shellcrafter/find_gadgets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11174 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/src/shellcrafter/keyst_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/src/shellcrafter/peutils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10063 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/src/shellcrafter/shellcode_procedure_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:33:39.177477 shellcrafter-1.1.2/src/shellcrafter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-28 12:33:39.000000 shellcrafter-1.1.2/src/shellcrafter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-28 12:33:39.000000 shellcrafter-1.1.2/src/shellcrafter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:33:39.000000 shellcrafter-1.1.2/src/shellcrafter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-28 12:33:39.000000 shellcrafter-1.1.2/src/shellcrafter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-28 12:33:39.000000 shellcrafter-1.1.2/src/shellcrafter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 12:33:39.000000 shellcrafter-1.1.2/src/shellcrafter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:32:42.544788 shellcrafter-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-05 01:32:42.544788 shellcrafter-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 01:32:42.544788 shellcrafter-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:32:42.540789 shellcrafter-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:32:42.540789 shellcrafter-1.1.3/src/shellcrafter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/src/shellcrafter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/src/shellcrafter/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13367 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/src/shellcrafter/find_gadgets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11174 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/src/shellcrafter/keyst_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8714 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/src/shellcrafter/peutils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10063 2024-05-05 01:32:31.000000 shellcrafter-1.1.3/src/shellcrafter/shellcode_procedure_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 01:32:42.544788 shellcrafter-1.1.3/src/shellcrafter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-05 01:32:42.000000 shellcrafter-1.1.3/src/shellcrafter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-05 01:32:42.000000 shellcrafter-1.1.3/src/shellcrafter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 01:32:42.000000 shellcrafter-1.1.3/src/shellcrafter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 01:32:42.000000 shellcrafter-1.1.3/src/shellcrafter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-05 01:32:42.000000 shellcrafter-1.1.3/src/shellcrafter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-05 01:32:42.000000 shellcrafter-1.1.3/src/shellcrafter.egg-info/top_level.txt
```

### Comparing `shellcrafter-1.1.2/PKG-INFO` & `shellcrafter-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellcrafter
-Version: 1.1.2
+Version: 1.1.3
 Summary: A package containing scripts for developing and generating shellcode
 Home-page: https://github.com/totekuh/shellcrafter
 Author: totekuh
 Author-email: totekuh@protonmail.com
 Project-URL: Bug Reports, https://github.com/totekuh/shellcrafter/issues
 Project-URL: Source, https://github.com/totekuh/shellcrafter
 Description-Content-Type: text/markdown
```

### Comparing `shellcrafter-1.1.2/README.md` & `shellcrafter-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.1.2/setup.py` & `shellcrafter-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-version = "1.1.2"
+version = "1.1.3"
 
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 REPO_URL = 'https://github.com/totekuh/shellcrafter'
```

### Comparing `shellcrafter-1.1.2/src/shellcrafter/cli.py` & `shellcrafter-1.1.3/src/shellcrafter/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -164,25 +164,36 @@
     shellcode_compiler = ShellcodeCompiler(arch=arch)
     shellcode_assembled, count = shellcode_compiler.assemble_instructions(
         instructions=get_instructions(instructions, instructions_file))
     print_shellcode(shellcode_assembled, var_name=var_name, interval=interval, output_format=output_format)
 
 
 @shellcode_app.command("run", help="Executes the compiled shellcode on the detected platform.")
-def run_shellcode_command(instructions: str = Option(None, "--instructions", "-i"),
-                          instructions_file: str = Option(None, "--instructions-file", "-if"),
-                          interactive: bool = Option(False, "--interactive"),
-                          arch: str = Option(X86_ARCH, "--arch")):
+def run_shellcode_command(instructions: str = Option(None, "--instructions", "-i", help="Inline assembly instructions to compile and run."),
+                          instructions_file: str = Option(None, "--instructions-file", "-if", help="File containing assembly instructions to compile and run."),
+                          bin_file: str = Option(None, "--bin", help="File containing raw binary shellcode to run directly."),
+                          interactive: bool = Option(False, "--interactive", help="Run shellcode in interactive mode."),
+                          arch: str = Option(X86_ARCH, "--arch", help="Architecture of the shellcode (default x86).")):
+    inputs = sum([bool(instructions), bool(instructions_file), bool(bin_file)])
+    if inputs != 1:
+        print("Error: Please specify only one of --instructions, --instructions-file, or --bin.")
+        raise Exit(code=1)
     shellcode_runner = ShellcodeRunner(arch=arch)
-    shellcode_compiler = ShellcodeCompiler(arch=arch)
-
-    shellcode_assembled, count = shellcode_compiler.assemble_instructions(
-        instructions=get_instructions(instructions, instructions_file))
 
-    shellcode_runner.run_shellcode(shellcode_assembled, interactive=interactive)
+    if bin_file:
+        if os.path.exists(bin_file):
+            with open(bin_file, 'rb') as file:
+                shellcode_binary = file.read()
+            shellcode_runner.run_shellcode(shellcode_binary, interactive)
+        else:
+            print(f"Error: The specified binary file does not exist: {bin_file}")
+    else:
+        shellcode_assembled, count = ShellcodeCompiler(arch).assemble_instructions(
+            get_instructions(instructions, instructions_file))
+        shellcode_runner.run_shellcode(shellcode_assembled, interactive)
 
 
 @pe_app.command(name="rva-offset-find", help="Convert RVA to file offset in a PE file.")
 def find_rva_offset_(file: str,
                      rva: str = typer.Argument(...,
                                                help='RVA to convert. Supports "0x" prefix for hexadecimal values.'),
                      section_name: Optional[str] = typer.Option(None, "--section-name", "-sn",
@@ -200,19 +211,37 @@
 
 @pe_app.command(name="bytes-display", help="Display bytes from a file starting at a specified offset.")
 def display_bytes_(file: str = typer.Argument(..., help="The path to the binary file."),
                           offset: str = typer.Option(..., help="Offset in the file to start reading bytes."),
                           length: int = typer.Option(..., help="Number of bytes to read and display.")):
     display_bytes(file=file, offset=offset, length=length)
 
-@pe_app.command(name="bytes-search", help="Search for a sequence of bytes in a file.")
+@pe_app.command(name="bytes-search", help="Search for a sequence of bytes or ASCII characters in a file.")
 def bytes_search(file: str = typer.Argument(..., help="The path to the binary file."),
-                 byte_sequence: str = typer.Option(..., help="Byte sequence to search for, e.g., '\\x41\\x42\\x43'")):
-    search_bytes(file=file, byte_sequence=byte_sequence)
+                 bytes_: Optional[str] = typer.Option(None, "--bytes", help="Byte sequence to search for, e.g., '\\x41\\x42\\x43'."),
+                 ascii: Optional[str] = typer.Option(None, "--ascii", help="ASCII text to search for, e.g., 'ABC'. Specify only one of --bytes or --ascii.")):
+    """
+    Search for a sequence of bytes or ASCII text in a file. Specify either --bytes or --ascii.
+    """
+    if bytes_ and ascii:
+        raise Exit("Error: Please specify either a byte sequence or an ASCII string, not both.")
+    if not bytes_ and not ascii:
+        raise Exit("Error: No search pattern provided. Please specify a byte sequence or an ASCII string.")
+
+    # Convert ASCII sequence to bytes if provided
+    if ascii:
+        search_sequence = ascii.encode()
+    # Convert string representation of byte sequence to actual bytes if provided
+    if bytes_:
+        try:
+            search_sequence = bytes.fromhex(bytes_.replace('\\x', ''))
+        except ValueError:
+            raise Exit("Error: Invalid byte sequence. Please ensure it's in the correct format, e.g., '\\x41\\x42'.")
 
+    search_bytes(file=file, search_sequence=search_sequence)
 
 @pe_app.command(name="eat-print", help="Parse the Export Address Table (EAT) and print it.")
 def eat_print_(file: str):
     parse_eat(file=file)
 
 @pe_app.command(name="sections-print", help="Print details of each section in the PE file.")
 def print_sections_(file: str = typer.Argument(..., help="The path to the PE file.")):
```

### Comparing `shellcrafter-1.1.2/src/shellcrafter/find_gadgets.py` & `shellcrafter-1.1.3/src/shellcrafter/find_gadgets.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.1.2/src/shellcrafter/keyst_api.py` & `shellcrafter-1.1.3/src/shellcrafter/keyst_api.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.1.2/src/shellcrafter/peutils.py` & `shellcrafter-1.1.3/src/shellcrafter/peutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pefile
 from rich.console import Console
 from rich.table import Table
 
 console = Console()
 
 
+
 def validate_file(file: str):
     if not os.path.exists(file):
         console.print(f"[-] The file {file} doesn't exist.", style="bold red")
         raise typer.Exit(code=-1)
 
 def is_valid_pe_file(file_path: str) -> bool:
     try:
@@ -164,27 +165,20 @@
     ]
     characteristics_desc = []
     for flag, desc in flags:
         if characteristics & flag:
             characteristics_desc.append(desc)
     return ", ".join(characteristics_desc)
 
-def search_bytes(file: str, byte_sequence: str):
+def search_bytes(file: str, search_sequence: bytes):
     """
     Search for a given sequence of bytes in a binary file.
     """
     validate_file(file)
 
-    # Convert string to bytes
-    try:
-        search_sequence = bytes.fromhex(byte_sequence.replace('\\x', ''))
-    except ValueError:
-        console.print(f"[-] Invalid byte sequence: {byte_sequence}", style="bold red")
-        raise typer.Exit(code=1)
-
     try:
         with open(file, 'rb') as f:
             file_content = f.read()
     except IOError as e:
         console.print(f"Error reading the file: {str(e)}", style="bold red")
         raise typer.Exit(code=1)
```

### Comparing `shellcrafter-1.1.2/src/shellcrafter/shellcode_procedure_generator.py` & `shellcrafter-1.1.3/src/shellcrafter/shellcode_procedure_generator.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.1.2/src/shellcrafter.egg-info/PKG-INFO` & `shellcrafter-1.1.3/src/shellcrafter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellcrafter
-Version: 1.1.2
+Version: 1.1.3
 Summary: A package containing scripts for developing and generating shellcode
 Home-page: https://github.com/totekuh/shellcrafter
 Author: totekuh
 Author-email: totekuh@protonmail.com
 Project-URL: Bug Reports, https://github.com/totekuh/shellcrafter/issues
 Project-URL: Source, https://github.com/totekuh/shellcrafter
 Description-Content-Type: text/markdown
```

