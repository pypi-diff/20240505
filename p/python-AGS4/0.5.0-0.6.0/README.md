# Comparing `tmp/python_ags4-0.5.0.tar.gz` & `tmp/python_ags4-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ags4-0.5.0.tar", max compression
+gzip compressed data, was "python_ags4-0.6.0.tar", max compression
```

## Comparing `python_ags4-0.5.0.tar` & `python_ags4-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     7652 2023-11-24 01:07:48.992474 python_ags4-0.5.0/COPYING.LESSER
--rw-r--r--   0        0        0    35149 2021-07-07 04:29:06.783702 python_ags4-0.5.0/LICENSE
--rw-r--r--   0        0        0     6981 2024-01-28 16:28:32.867040 python_ags4-0.5.0/README.md
--rw-r--r--   0        0        0      754 2024-01-28 16:28:32.899040 python_ags4-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    50522 2024-01-28 16:28:32.899040 python_ags4-0.5.0/python_ags4/AGS4.py
--rw-r--r--   0        0        0   276189 2023-11-24 01:07:49.028464 python_ags4-0.5.0/python_ags4/Standard_dictionary_v4_0_3.ags
--rw-r--r--   0        0        0   276942 2023-11-24 01:07:49.032463 python_ags4-0.5.0/python_ags4/Standard_dictionary_v4_0_4.ags
--rw-r--r--   0        0        0   377728 2024-01-28 16:28:32.903040 python_ags4-0.5.0/python_ags4/Standard_dictionary_v4_1.ags
--rw-r--r--   0        0        0   382078 2024-01-28 16:28:32.903040 python_ags4-0.5.0/python_ags4/Standard_dictionary_v4_1_1.ags
--rw-r--r--   0        0        0      138 2024-01-28 16:28:32.903040 python_ags4-0.5.0/python_ags4/__init__.py
--rw-r--r--   0        0        0    15722 2024-01-28 16:28:32.903040 python_ags4-0.5.0/python_ags4/ags4_cli.py
--rw-r--r--   0        0        0    70346 2024-01-28 16:28:32.903040 python_ags4-0.5.0/python_ags4/check.py
--rw-r--r--   0        0        0      426 2023-12-17 06:06:12.788627 python_ags4-0.5.0/python_ags4/data/__init__.py
--rw-r--r--   0        0        0     3253 2023-12-17 06:06:12.788627 python_ags4-0.5.0/python_ags4/data/test_data.ags
--rw-r--r--   0        0        0     7916 1970-01-01 00:00:00.000000 python_ags4-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-11-24 01:07:48.992474 python_ags4-0.6.0/COPYING.LESSER
+-rw-r--r--   0        0        0    35149 2021-07-07 04:29:06.783702 python_ags4-0.6.0/LICENSE
+-rw-r--r--   0        0        0     6981 2024-05-05 05:48:17.010666 python_ags4-0.6.0/README.md
+-rw-r--r--   0        0        0      778 2024-05-05 05:35:24.491576 python_ags4-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    47655 2024-05-05 05:35:24.491576 python_ags4-0.6.0/python_ags4/AGS4.py
+-rw-r--r--   0        0        0   276189 2023-11-24 01:07:49.028464 python_ags4-0.6.0/python_ags4/Standard_dictionary_v4_0_3.ags
+-rw-r--r--   0        0        0   276942 2023-11-24 01:07:49.032463 python_ags4-0.6.0/python_ags4/Standard_dictionary_v4_0_4.ags
+-rw-r--r--   0        0        0   377728 2024-01-28 18:01:51.739430 python_ags4-0.6.0/python_ags4/Standard_dictionary_v4_1.ags
+-rw-r--r--   0        0        0   382078 2024-01-28 18:01:51.739430 python_ags4-0.6.0/python_ags4/Standard_dictionary_v4_1_1.ags
+-rw-r--r--   0        0        0      138 2024-01-28 18:01:51.739430 python_ags4-0.6.0/python_ags4/__init__.py
+-rw-r--r--   0        0        0    16716 2024-05-05 05:35:24.491576 python_ags4-0.6.0/python_ags4/ags4_cli.py
+-rw-r--r--   0        0        0    69508 2024-05-05 05:35:24.491576 python_ags4-0.6.0/python_ags4/check.py
+-rw-r--r--   0        0        0      426 2023-12-17 06:06:12.788627 python_ags4-0.6.0/python_ags4/data/__init__.py
+-rw-r--r--   0        0        0     3253 2023-12-17 06:06:12.788627 python_ags4-0.6.0/python_ags4/data/test_data.ags
+-rw-r--r--   0        0        0     7917 1970-01-01 00:00:00.000000 python_ags4-0.6.0/PKG-INFO
```

### Comparing `python_ags4-0.5.0/COPYING.LESSER` & `python_ags4-0.6.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `python_ags4-0.5.0/LICENSE` & `python_ags4-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ags4-0.5.0/README.md` & `python_ags4-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `python_ags4-0.5.0/pyproject.toml` & `python_ags4-0.6.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [tool.poetry]
 name = "python-AGS4"
-version = "0.5.0"
+version = "0.6.0"
 description = "A library to read, write, and check AGS4 files using Pandas DataFrames"
 authors = ["Asitha Senanayake <asitha_sena@yahoo.com>"]
 license = "LGPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/asitha-sena/python-AGS4"
 repository = "https://gitlab.com/ags-data-format-wg/ags-python-library"
 include = ["COPYING.LESSER"]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-pandas = "^2.0"
+python = "^3.9"
+pandas = "^2.1"
 openpyxl = "^3.0"
 defusedxml = ">=0.6, <0.8"
 click = ">=7.0, <9.0"
 rich = ">=9.0, <14.0"
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.3"
-toml = "^0.10"
-
 [tool.poetry.scripts]
 ags4_cli = "python_ags4.ags4_cli:main"
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3"
+toml = "^0.10"
+isort = "^5.13.2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `python_ags4-0.5.0/python_ags4/AGS4.py` & `python_ags4-0.6.0/python_ags4/AGS4.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,16 +60,14 @@
         AGS4 files. i.e. input for 'dataframe_to_AGS4()' function)
     line_numbers : dict of int, only if get_line_numbers=True
         Dictionary with the starting line numbers of GROUP and HEADING rows.
         This is only required for checking a .ags file with 'check_file()'
         function.
     """
 
-    from rich import print as rprint
-
     if _is_file_like(filepath_or_buffer):
         f = filepath_or_buffer
         f.seek(0)
         if hasattr(f, 'encoding') and getattr(f, 'encoding', None) != encoding:
             f.reconfigure(encoding=encoding)
         close_file = False
     else:
@@ -101,15 +99,14 @@
 
                 # Raise exception if duplicate group is found as previous copy
                 # of that group will be overwritten
                 if group in data.keys():
                     msg = f"{group} group duplicated in Line {i}. Cannot parse file without overwriting data, "\
                            "therefore please combine all duplicate groups first."
 
-                    rprint(f"[red]  ERROR: {msg}[/red]")
                     logger.error(msg)
                     raise AGS4Error(msg)
 
                 else:
                     data[group] = {}
 
                 # Store GROUP line number (A default 'HEADING' entry is added to
@@ -122,15 +119,14 @@
                 # a dictionary with arrays of unequal lengths and cause a
                 # ValueError when trying to convert to a Pandas dataframe
                 if len(temp) != len(set(temp)):
 
                     if rename_duplicate_headers is False:
                         raise AGS4Error(f"HEADER row in {group} (Line {i}) has duplicate entries")
 
-                    rprint(f"[yellow]  WARNING: HEADER row in [bold]{group}[/bold] (Line {i}) has duplicate entries.[/yellow]")
                     logger.warning(f"HEADER row in {group} (Line {i}) has duplicate entries.")
 
                     # Rename duplicate headers by appending a number
                     item_count = {}
 
                     for i, item in enumerate(temp):
                         if item not in item_count:
@@ -138,17 +134,14 @@
                         else:
                             item_count[item]['i'] = i
                             item_count[item]['count'] += 1
                             count = item_count[item]['count']
 
                             temp[i] = temp[i]+'_'+str(item_count[item]['count'])
 
-                            rprint(f'[blue]  INFO: Duplicate column {item} found and renamed as {item}_{count}.[/blue]')
-                            rprint('[blue]        Automatically renamed columns do not conform to AGS4 Rules 19a and 19b.[/blue]')
-                            rprint('[blue]        Therefore, please review the data and rename or drop duplicate columns as appropriate.[/blue]')
                             logger.info(f'Duplicate column {item} found and renamed as {item}_{count}. '
                                         'Automatically renamed columns do not conform to AGS4 Rules 19a and 19b. '
                                         'Therefore, please review the data and rename or drop duplicate columns as appropriate.')
 
                 # Store HEADING line number
                 line_numbers[group]['HEADING'] = i
 
@@ -166,15 +159,15 @@
                 # Append line number
                 if get_line_numbers is True:
                     temp.append(i)
 
                 # Check whether line has the same number of entries as the
                 # number of headings in the group. If not, print error and exit.
                 if len(temp) != len(headings[group]):
-                    rprint(f"[red]  Error: Line {i} does not have the same number of entries as the HEADING row in [bold]{group}[/bold].[/red]")
+                    logger.error(f"Line {i} does not have the same number of entries as the HEADING row in {group}.")
                     raise AGS4Error(f"Line {i} does not have the same number of entries as the HEADING row in {group}.")
 
                 for i in range(0, len(temp)):
                     data[group][headings[group][i]].append(temp[i])
 
             else:
                 continue
@@ -266,63 +259,61 @@
     encoding : str, default='utf-8'
         Encoding of text file. This can be set to 'utf-8-sig' to read files that
         begin with a byte-order-mark.
     rename_duplicate_headers: bool, default=True
         Rename duplicate headers if found. Neither AGS4 tables nor Pandas
         dataframes allow duplicate headers, therefore a number will be appended
         to duplicates to make them unique.
-    sorting_strategy : {None, dictionary', 'alphabetical', 'hierarchical'}, default=None
+    sorting_strategy : {None, 'dictionary', 'alphabetical', 'hierarchical'}, default=None
         Sort groups in the order in which they appear in the dictionary, the
         hierarchy defined in the dictionary, or alphabetically.
         WARNING: The original order of groups will be lost and cannot be
         restored when .xlsx file is converted back to .ags.
 
     Returns
     -------
     None
     """
 
     from pandas import ExcelWriter
-    from rich import print as rprint
     from openpyxl.utils import get_column_letter
 
     # Extract AGS4 file into a dictionary of dictionaries
     tables, headings = AGS4_to_dataframe(input_file, encoding=encoding,
                                          rename_duplicate_headers=rename_duplicate_headers)
 
     # Create list of tables that can be sorted
     if sorting_strategy is not None:
         sorting_desc = {'dictionary': 'according to the order of appearance in the dictionary',
                         'alphabetical': 'alphabetically',
                         'hierarchical': 'according to the hierarchy defined in the dictionary'}
         msg = f'WARNING: Worksheets in Excel file will be sorted {sorting_desc[sorting_strategy]}. The original group order will be lost.'
-        rprint(f"[yellow]{msg}[/yellow]")
         logger.warning(f"{msg}")
 
         list_of_tables = sort_groups(tables, sorting_strategy=sorting_strategy)
 
     else:
         list_of_tables = tables.keys()
 
     # Exit if there is no AGS4 tables in the input file
     if len(list_of_tables) == 0:
-        rprint('[red]  ERROR: No valid AGS4 data found in input file.[/red]')
+        logger.error('No valid AGS4 data found in input file.')
         raise AGS4Error('No valid AGS4 data found in input file.')
 
     # Write to Excel file
     with ExcelWriter(output_file, engine='openpyxl') as writer:
         for key in list_of_tables:
-            rprint(f'[green]Writing data from... [bold]{key}[/bold][/green]')
+            logger.info(f'Writing data from... {key}')
 
             # Check table size and issue warning for large files that could crash the program
             if 25000 < tables[key].shape[0] < 100000:
-                rprint(f'[blue]  INFO: {key} has {tables[key].shape[0]} rows, so it will take about a minute to export.[/blue]')
+                logger.info(f'{key} has {tables[key].shape[0]} rows, so it will take about a minute to export.')
             elif tables[key].shape[0] > 100000:
-                rprint(f'[yellow]  WARNING: {key} has {tables[key].shape[0]} rows, so it may take a few minutes to export.[/yellow]')
-                rprint('[yellow]           The program will terminate if it runs out of memory in the process.[/yellow]')
+                logger.warning(f'{key} has {tables[key].shape[0]} rows, so it may take a few minutes to export. '
+                               'The program will terminate if it runs out of memory in the process.')
 
             tables[key].to_excel(writer, sheet_name=key, index=False)
 
             # Update column widths in xlxs file to fit contents
             for i, col in enumerate(tables[key], start=1):
                 # 13 < colummn_width < 75 characters (approximately)
                 max_width = min(max(13, tables[key][col].map(len).max() + 1), 75)
@@ -358,16 +349,14 @@
         Print warnings
 
     Returns
     -------
     None
     """
 
-    from rich import print as rprint
-
     # Open file and write/append data
     with open(filepath, mode, newline='', encoding=encoding) as f:
         for key in tables:
             # First make copy of table to avoid unexpected side-effects
             df = tables[key].copy()
 
             # Take care of an edge case where quoted text is present in a field.
@@ -380,24 +369,18 @@
             for col in df.select_dtypes(include='object'):
                 # Loop through columns that contain strings, find entries with '""', and replace
                 # them with '""
                 mask = df[col].str.contains('""', na=False)
                 df.loc[mask, :] = df.loc[mask, :].apply(lambda x: x.str.replace('""', '"'))
 
             # Write table to file
-            rprint(f'[green]Writing data from... [bold]{key}[/bold][green]')
             logger.info(f'Writing data from... {key}')
             f.write('"GROUP"'+","+'"'+key+'"'+'\r\n')
 
             if key not in headings:
-                if warnings is True:
-                    rprint(f"[yellow]  WARNING: Input 'headings' dictionary does not have an entry named [bold]{key}[/bold].[/yellow]")
-                    rprint(f"[italic yellow]           All columns in the {key} table will be exported in the default order.[/italic yellow]")
-                    rprint("[italic yellow]           Please check column order and ensure AGS4 Rule 7 is still satisfied.[/italic yellow]")
-
                 logger.warning(f"Input 'headings' dictionary does not have an entry named {key}. "
                                f"All columns in the {key} table will be exported in the default order. "
                                "Please check column order and ensure AGS4 Rule 7 is still satisfied.")
 
                 df.to_csv(f, index=index, quoting=1, lineterminator='\r\n', encoding=encoding)
                 f.write("\r\n")
 
@@ -408,18 +391,14 @@
                 # headings list to export the remaining columns in the specified
                 # order.
                 # https://gitlab.com/ags-data-format-wg/ags-python-library/-/issues/69
 
                 missing_cols = set(headings[key]).difference(set(df.columns))
                 columns = [x for x in headings[key] if x not in missing_cols]
 
-                if warnings is True:
-                    rprint(f"[yellow]  WARNING: Columns {', '.join(missing_cols)} not found in the {key} table"
-                           " although they are in the headings dictionary..[/yellow]")
-
                 logger.warning(f"Columns {', '.join(missing_cols)} not found in the {key} table although they are in the headings dictionary.")
 
                 df.to_csv(f, index=index, quoting=1, columns=columns, lineterminator='\r\n', encoding=encoding)
                 f.write("\r\n")
 
             else:
                 columns = headings[key]
@@ -446,52 +425,47 @@
 
     Returns
     -------
     None
     """
 
     from pandas import read_excel
-    from rich import print as rprint
 
     # Read data from Excel file in to a dictionary of dataframes
     tables = read_excel(input_file, sheet_name=None, engine='openpyxl')
 
     # Not all worksheets in the spreadsheet may contain valid AGS4 tables, therefore
     # initiate variable to keep track of worksheets to export
     valid_tables = []
 
     for key, df in tables.items():
         # Assume that only worksheets with a 'HEADING' column contain valid AGS4 data
         if 'HEADING' in df:
             valid_tables.append(key)
         else:
-            rprint(f'[yellow]  WARNING: Worksheet [bold]{key}[/bold] dropped as it does not have a HEADING column.[/yellow]')
             logger.warning(f'Worksheet {key} dropped as it does not have a HEADING column.')
             continue
 
         # List column names that don't conform to Rule 19 (using a negative look-ahead regex)
         for col_name in df.filter(regex=r'^(?!HEADING|^[A-Z0-9]{4}_[A-Z0-9]{1,4}$)', axis='columns'):
-            rprint(f'[yellow]  WARNING: Column [bold]{col_name}[/bold] dropped as name does not conform to AGS4 Rule 19.[/yellow]')
             logger.warning(f'Column {col_name} dropped as name does not conform to AGS4 Rule 19.')
 
         # Drop columns that don't conform to Rule 19
         df = df.filter(regex=r'HEADING|^[A-Z0-9]{4}_[A-Z0-9]{1,4}$', axis='columns')
 
         # Drop rows that are not 'UNIT', 'TYPE', or 'DATA'
         df = df.loc[df.HEADING.isin(['UNIT', 'TYPE', 'DATA']), :]
 
         # Finally format numeric column if required
         if format_numeric_columns is True:
-            rprint(f'[green]Formatting columns in... [bold]{key}[/bold][/green]')
             logger.info(f'Formatting columns in... {key}')
             tables[key] = convert_to_text(df, dictionary=dictionary)
 
     # Export dictionary of DataFrames to AGS4 file
     if len(valid_tables) == 0:
-        rprint('[red]  ERROR: No valid AGS4 data found in input file. Please see warning messages above.[/red]')
         logger.warning('No valid AGS4 data found in input file. Please see warning messages above.')
     else:
         dataframe_to_AGS4({key: tables[key] for key in valid_tables}, {}, output_file, warnings=False)
 
 
 # Formatting functions #
 
@@ -558,15 +532,14 @@
     Pandas DataFrame
         A Pandas DataFrame with numeric columns converted to text and formatted
         to the correct precision. UNIT and TYPE rows will be added if that
         information is provided as an input.
     """
 
     from python_ags4 import check
-    from rich import print as rprint
 
     # Make copy of dataframe and reset index to make sure numbering
     # starts from zero
     df = dataframe.copy().reset_index(drop=True)
 
     # Check whether to use UNIT and TYPE rows in dataframe or to
     # retrieve values from the dictionary file
@@ -575,16 +548,14 @@
         if ('UNIT' in df.HEADING.values) and ('TYPE' in df.HEADING.values):
 
             for col in df.columns:
                 TYPE = df.loc[df.HEADING == 'TYPE', col].values[0]
                 df = format_numeric_column(df, col, TYPE)
 
         else:
-            rprint("[red]  ERROR: Cannot convert to text as UNIT and/or TYPE row(s) are missing.")
-            rprint("[red]         Please provide dictonary file or add UNIT & TYPE rows to input file to proceed.[/red]")
             logger.error('Cannot convert to text as UNIT and/or TYPE row(s) are missing. '
                          'Please provide dictonary file or add UNIT & TYPE rows to input file to proceed.')
             raise AGS4Error("Cannot convert to text as UNIT and/or TYPE row(s) are missing. "
                             "Please provide dictonary file or add UNIT & TYPE rows to input file to proceed.")
 
     else:
         # Read dictionary file
@@ -633,15 +604,14 @@
                     else:
                         # Add TYPE row if one is not already there
                         df.loc[-1, col] = TYPE
 
                     df = format_numeric_column(df, col, TYPE)
 
                 except IndexError:
-                    rprint(f"[yellow]  WARNING: [bold]{col}[/bold] not found in the dictionary file.[/yellow]")
                     logger.warning(f'{col} not found in the dictionary file.')
 
     return df.sort_index().reset_index(drop=True)
 
 
 def format_numeric_column(dataframe, column_name, TYPE):
     '''Format column in dataframe to specified TYPE and convert to string.
@@ -657,16 +627,14 @@
 
     Returns
     -------
     Pandas DataFrame
         Dataframe with formatted data.
     '''
 
-    from rich import print as rprint
-
     df = dataframe.copy()
     col = column_name
 
     try:
         if 'DP' in TYPE:
             i = int(TYPE.strip('DP'))
             # Apply formatting DATA rows with real numbers. NaNs will be avoided so that they will be exported
@@ -682,25 +650,23 @@
             df.loc[mask, col] = df.loc[mask, col].apply(lambda x: f"{x:.{i}E}")
 
         elif 'SF' in TYPE:
 
             # Apply formatting DATA rows with real numbers. NaNs will be avoided so that they will be exported
             # as "" rather than "nan"
             mask = (df.HEADING == "DATA") & df[col].notna()
-            df.loc[mask, [col]] = df.loc[mask, [col]].applymap(lambda x: _format_SF(x, TYPE))
+            df.loc[mask, [col]] = df.loc[mask, [col]].map(lambda x: _format_SF(x, TYPE))
 
         else:
             pass
 
     except ValueError:
-        rprint(f"[yellow]  WARNING: Numeric data in [bold]{col:<9}[/bold] not reformatted as it had one or more non-numeric entries.[/yellow]")
         logger.warning(f"Numeric data in {col:<9} not reformatted as it had one or more non-numeric entries.")
 
     except TypeError:
-        rprint(f"[yellow]  WARNING: Numeric data in [bold]{col:<9}[/bold] not reformatted as it had one or more non-numeric entries.[/yellow]")
         logger.warning(f"Numeric data in {col:<9} not reformatted as it had one or more non-numeric entries.")
 
     return df
 
 
 def _format_SF(value, TYPE):
     '''Format a value to specified number of significant figures
@@ -718,15 +684,16 @@
     if i < 0:
         return f"{round(value, i):.0f}"
 
     else:
         return f"{value:.{i}f}"
 
 
-def check_file(filepath_or_buffer, standard_AGS4_dictionary=None, rename_duplicate_headers=True, encoding='utf-8', print_output:bool=True):
+def check_file(filepath_or_buffer, standard_AGS4_dictionary=None, rename_duplicate_headers=True, encoding='utf-8',
+               print_output=True):
     """Validate AGS4 file against AGS4 rules.
 
     Parameters
     ----------
     filepath_or_buffer : strFile path (str, pathlib.Path), or StringIO.
         Path to AGS4 file or any object with a read() method (such as an open
         file or StringIO) to be checked.
@@ -745,21 +712,19 @@
     Returns
     -------
     dict
         Dictionary contains AGS4 error in input file.
     """
 
     from python_ags4 import check
-    from rich import print as rprint
     import traceback
 
     ags_errors = {}
 
-    if print_output:
-        logger.info(f'Opening file... {filepath_or_buffer}')
+    logger.info(f'Opening file... {filepath_or_buffer}')
 
     # Line checks
     if _is_file_like(filepath_or_buffer):
         f = filepath_or_buffer
         f.seek(0)
         if hasattr(f, 'encoding') and getattr(f, 'encoding', None) != encoding:
             f.reconfigure(encoding=encoding)
@@ -781,16 +746,16 @@
         # Reset file stream to the beginning to start AGS4 checks
         f.seek(0)
 
         # Initiate group name and headings list
         group = ''
         headings = []
 
+        logger.info('Checking lines...')
         if print_output:
-            rprint('[green]  Checking lines...[/green]')
             logger.info('Checking lines...')
 
         for i, line in enumerate(f, start=1):
 
             # Track headings to be used with group checks
             if line.strip('"').startswith("GROUP"):
                 # Reset group name and headings list at the beginning each group
@@ -830,25 +795,21 @@
                   "The validator defaults to 'utf-8' encoding as it is the most widely used encoding compatible with Unicode. "\
                   "The user can override this default if the file encoding is different but, "\
                   "it is highly recommended that the 'utf-8' encoding be used when creating AGS4 files. "\
                   "(Hint: If not 'utf-8', then the encoding is most likely to be 'windows-1252' aka 'cp1252')"
             ags_errors = check.add_error_msg(ags_errors, 'General', '', '', msg)
 
         # Import data into Pandas dataframes to run group checks
-        if print_output:
-            rprint('[green]  Loading tables...[/green]')
-            logger.info('Loading tables...')
+        logger.info('Loading tables...')
 
         f.seek(0)
         tables, headings, line_numbers = AGS4_to_dataframe(f, get_line_numbers=True, rename_duplicate_headers=rename_duplicate_headers)
 
         # Group Checks
-        if print_output:
-            rprint('[green]  Checking headings and groups...[/green]')
-            logger.info('Checking headings and groups...')
+        logger.info('Checking headings and groups...')
 
         ags_errors = check.rule_2(tables, headings, line_numbers, ags_errors=ags_errors)
         ags_errors = check.rule_2b(tables, headings, line_numbers, ags_errors=ags_errors)
         ags_errors = check.rule_8(tables, headings, line_numbers, ags_errors=ags_errors)
         ags_errors = check.rule_12(tables, headings, ags_errors=ags_errors)
         ags_errors = check.rule_13(tables, headings, line_numbers, ags_errors=ags_errors)
         ags_errors = check.rule_14(tables, headings, line_numbers, ags_errors=ags_errors)
@@ -873,17 +834,15 @@
         # Import standard dictionary file into Pandas dataframes
         tables_std_dict, _ = AGS4_to_dataframe(standard_AGS4_dictionary)
 
         # Combine standard dictionary with DICT table in input file to create an extended dictionary
         # This extended dictionary is used to check the file schema
         dictionary = check.combine_DICT_tables(tables_std_dict, tables)
 
-        if print_output:
-            rprint('[green]  Checking file schema...[/green]')
-            logger.info('Checking file schema...')
+        logger.info('Checking file schema...')
 
         ags_errors = check.rule_7_2(headings, dictionary, line_numbers, ags_errors=ags_errors)
         ags_errors = check.rule_9(headings, dictionary, line_numbers, ags_errors=ags_errors)
         ags_errors = check.rule_10a(tables, headings, dictionary, line_numbers, ags_errors=ags_errors)
         ags_errors = check.rule_10b(tables, headings, dictionary, line_numbers, ags_errors=ags_errors)
         ags_errors = check.rule_10c(tables, headings, dictionary, line_numbers, ags_errors=ags_errors)
         ags_errors = check.rule_11(tables, headings, dictionary, ags_errors=ags_errors)
@@ -898,20 +857,23 @@
         ags_errors = check.warning_16_1(tables, headings, tables_std_dict['ABBR'], ags_errors=ags_errors)
 
         # Add summary of data
         for val in check.get_data_summary(tables):
             ags_errors = check.add_error_msg(ags_errors, 'Summary of data', '', '', val)
 
     except AGS4Error as err:
-        if print_output:
-            logger.exception(err)
+        logger.exception(err)
+
+        ags_errors = check.add_error_msg(ags_errors, 'General', '-', '',
+                                         'Could not complete validation. Please fix listed errors and try again.')
+        ags_errors = check.add_error_msg(ags_errors, 'Validator Process Error', '-', '', str(err))
 
-        ags_errors = check.add_error_msg(ags_errors, 'AGS Format Rule ?', '-', '', str(err))
+    except UnboundLocalError as err:
+        logger.exception(err)
 
-    except UnboundLocalError:
         # The presence of a byte-order-mark (BOM) in the same row as first
         # "GROUP" line can cause this exception. This will be caught by line
         # checks for Rule 1 (since the BOM is not an ASCII character) and Rule 3
         # (since the BOM precedes the string "GROUP"). The BOM encoding can be
         # ignored by setting the 'encoding' argument to 'utf-8-sig'.
         f.seek(0)
 
@@ -919,25 +881,20 @@
                                                            get_line_numbers=True, rename_duplicate_headers=rename_duplicate_headers)
 
         # Add warning to error log
         msg = 'This file seems to be encoded with a byte-order-mark (BOM). It is highly recommended that the '\
               'file be saved without BOM encoding to avoid issues with other software.'
         ags_errors = check.add_error_msg(ags_errors, 'General', '', '', msg)
 
-    except Exception:
-        err = traceback.format_exc()
-        msg = 'Could not continue with group checks on file. Please review error log and fix line errors first.'
+    except Exception as err:
+        logger.exception(err)
 
-        if print_output:
-            rprint(f'[red] ERROR: {msg}[/red]')
-            rprint(f'[red]\n{err}[/red]')
-            logger.exception(msg)
-
-        ags_errors = check.add_error_msg(ags_errors, 'AGS Format Rule ?', '-', '', msg)
-        ags_errors = check.add_error_msg(ags_errors, 'AGS Format Rule ?', '-', '', err)
+        ags_errors = check.add_error_msg(ags_errors, 'General', '-', '',
+                                         'Could not complete validation. Please fix listed errors and try again.')
+        ags_errors = check.add_error_msg(ags_errors, 'Validator Process Error', '-', '', str(err))
 
     finally:
         if close_file:
             f.close()
 
         # Add metadata
         ags_errors = check.add_meta_data(filepath_or_buffer, standard_AGS4_dictionary, ags_errors=ags_errors,
@@ -962,15 +919,14 @@
         Include FYI messages in error report
 
     Returns
     -------
     None
     '''
 
-    from rich import print as rprint
     import textwrap
 
     error_count, warnings_count, fyi_count = count_errors(ags_errors)
 
     try:
         with open(output_file, 'w', newline='', encoding='utf-8') as f:
             # Write metadata
@@ -1018,14 +974,21 @@
             # Write other AGS Format error messages
             for key in [x for x in ags_errors if 'AGS Format Rule' in x]:
                 f.write(f'{key}:\r\n')
                 for entry in ags_errors[key]:
                     f.write(f'''  Line {entry['line']:<8} {entry['group'].strip('"'):<7} {entry['desc']}\r\n''')
                 f.write('\r\n')
 
+            # Write parsing and process error messages
+            for key in [x for x in ags_errors if 'Validator Process Error' in x]:
+                f.write(f'{key}:\r\n')
+                for entry in ags_errors[key]:
+                    f.write(f'''  Line {entry['line']:<8} {entry['group'].strip('"'):<7} {entry['desc']}\r\n''')
+                f.write('\r\n')
+
             # Write warning messages
             if show_warnings is True:
                 for key in [x for x in ags_errors if 'Warning' in x]:
                     f.write(f'{key}:\r\n')
                     for entry in ags_errors[key]:
                         f.write(f'''  Line {entry['line']:<8} {entry['group'].strip('"'):<7} {entry['desc']}\r\n''')
                     f.write('\r\n')
@@ -1034,19 +997,19 @@
             if show_fyi is True:
                 for key in [x for x in ags_errors if 'FYI' in x]:
                     f.write(f'{key}:\r\n')
                     for entry in ags_errors[key]:
                         f.write(f'''  Line {entry['line']:<8} {entry['group'].strip('"'):<7} {entry['desc']}\r\n''')
                     f.write('\r\n')
 
-        rprint(f'\n[yellow]Error report saved in {output_file}[/yellow]\n')
+        logger.info(f'Error report saved in {output_file}')
 
     except FileNotFoundError:
-        rprint('[red]\nERROR: Invalid output file path. Error report could not be saved.[/red]')
-        rprint('[red]       Please ensure that the specified directory exists.[/red]')
+        logger.error('Invalid output file path. Error report could not be saved. '
+                     'Please ensure that the specified directory exists.')
 
     except TypeError:
         # Nothing to do if output_file is None
         pass
 
 
 def count_errors(ags_errors):
@@ -1068,22 +1031,22 @@
     '''
 
     # Count number of entries in error log
     error_count = 0
     warnings_count = 0
     fyi_count = 0
     for key, val in ags_errors.items():
-        error_count += len(val) if 'AGS Format Rule' in key else 0
+        error_count += len(val) if ('AGS Format Rule' in key) or ('Validator Process Error' in key) else 0
         warnings_count += len(val) if 'Warning' in key else 0
         fyi_count += len(val) if 'FYI' in key else 0
 
     return error_count, warnings_count, fyi_count
 
 
-def sort_groups(tables, sorting_strategy='hierarchical'):
+def sort_groups(tables, sorting_strategy='dictionary'):
     """Sort groups/tables parsed from AGS4 file.
 
     Parameters
     ----------
     tables : dict of dataframes
         Dictionary of Pandas dataframes (output from 'AGS4_to_dataframe()')
     sorting_strategy : {'dictionary', 'alphabetical', 'hierarchical'}, default='dictionary'
@@ -1093,15 +1056,14 @@
     Returns
     -------
     dict
         Dictionary of Pandas dataframes (output from 'AGS4_to_dataframe()')
     """
 
     from .check import pick_standard_dictionary, combine_DICT_tables
-    from rich import print as rprint
 
     # Combine standard dictionary with DICT table in input file to create an extended dictionary
     # This extended dictionary is used to check the table order
     standard_AGS4_dictionary = pick_standard_dictionary(tables=tables)
     tables_std_dict, _ = AGS4_to_dataframe(standard_AGS4_dictionary)
     dictionary = combine_DICT_tables(tables_std_dict, tables)
 
@@ -1135,15 +1097,14 @@
     sorted_tables = {x: tables[x] for x in group_list if x in tables.keys()}
 
     # Issue warning if groups are missing after sorting and append them to the
     # end in alphabetical order
     for item in sorted(set(tables.keys()).difference(set(sorted_tables.keys()))):
         msg = f'WARNING:Table {item} appended to the end as it was either not found in the dictionary '\
               'or its parent group is not defined under DICT_PGRP.'
-        rprint(f"[yellow]{msg}[/yellow]")
         logger.warning(f"{msg}")
         sorted_tables[item] = tables[item]
 
     return sorted_tables
 
 
 def _is_file_like(obj):
```

### Comparing `python_ags4-0.5.0/python_ags4/Standard_dictionary_v4_0_3.ags` & `python_ags4-0.6.0/python_ags4/Standard_dictionary_v4_0_3.ags`

 * *Files identical despite different names*

### Comparing `python_ags4-0.5.0/python_ags4/Standard_dictionary_v4_0_4.ags` & `python_ags4-0.6.0/python_ags4/Standard_dictionary_v4_0_4.ags`

 * *Files identical despite different names*

### Comparing `python_ags4-0.5.0/python_ags4/Standard_dictionary_v4_1.ags` & `python_ags4-0.6.0/python_ags4/Standard_dictionary_v4_1.ags`

 * *Files identical despite different names*

### Comparing `python_ags4-0.5.0/python_ags4/Standard_dictionary_v4_1_1.ags` & `python_ags4-0.6.0/python_ags4/Standard_dictionary_v4_1_1.ags`

 * *Files identical despite different names*

### Comparing `python_ags4-0.5.0/python_ags4/ags4_cli.py` & `python_ags4-0.6.0/python_ags4/ags4_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,32 +17,41 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 # https://github.com/asitha-sena/python-ags4
 # https://gitlab.com/ags-data-format-wg/ags-python-library
 
 
-import sys
 import logging
+import sys
+import textwrap
+import warnings
 from logging.handlers import RotatingFileHandler
 from pathlib import Path
-import textwrap
 
 import click
 from rich.console import Console
+from rich.highlighter import NullHighlighter
+from rich.logging import RichHandler
 
-from python_ags4 import AGS4, __version__
+from . import AGS4, __version__
 
 # Add warnings filter because Pandas 2.1 produces a lot of deprecation warnings
-import warnings
 warnings.filterwarnings('ignore')
 
 # Create rich console for pretty printing
 console = Console()
 
+# Logging
+stream_handler = RichHandler(console=console, show_time=False, show_path=False,
+                             highlighter=NullHighlighter(),
+                             rich_tracebacks=True)
+logger = logging.getLogger('python_ags4')
+logger.setLevel(logging.DEBUG)
+logger.addHandler(stream_handler)
 
 @click.group()
 def main():
     '''A tool to read, write, and check AGS4 files.
     '''
     pass
 
@@ -75,23 +84,24 @@
     Windows:   ags4_cli convert c:\Temp\data.ags c:\Temp\data.xlsx
 
     Exit codes:
         0 - Conversion succeeded
         1 - Conversion failed
     '''
 
-    # Log messages if specified
+    # Log messages to file if specified
     if log_messages is True:
-        logging.basicConfig(format='{asctime}  {levelname:<8}  {module}.{funcName:<20}  {message}',
-                            style='{', datefmt='%Y-%m-%dT%H:%M:%S%z',
-                            level=logging.DEBUG,
-                            handlers=[RotatingFileHandler(filename=Path(input_file).parent/'python_ags4.log', maxBytes=100e3, backupCount=1)])
-
-    else:
-        logging.basicConfig(level=logging.CRITICAL)
+        file_handler = RotatingFileHandler(filename=Path(input_file).parent/'python_ags4.log',
+                                        maxBytes=100e3,
+                                        backupCount=1)
+        file_formatter = logging.Formatter('{asctime}  {levelname:<8}  {module}.{funcName:<20}  {message}',
+                                        style='{',
+                                        datefmt='%Y-%m-%d %H:%M:%S')
+        file_handler.setFormatter(file_formatter)
+        logger.addHandler(file_handler)
 
     try:
         if input_file.endswith('.ags') & output_file.endswith('.xlsx'):
             console.print(f'[green]Opening file... [bold]{input_file}[/bold][/green]')
             console.print(f'[green]Exporting data to... [bold]{output_file}[/bold][/green]')
             print('')
 
@@ -174,23 +184,24 @@
     INPUT_FILE   Path to .ags file to be checked
 
     Exit codes:
         0 - All checks passed
         1 - Errors found or file read error
     '''
 
-    # Log messages if specified
+    # Log messages to file if specified
     if log_messages is True:
-        logging.basicConfig(format='{asctime}  {levelname:<8}  {module}.{funcName:<20}  {message}',
-                            style='{', datefmt='%Y-%m-%dT%H:%M:%S%z',
-                            level=logging.DEBUG,
-                            handlers=[RotatingFileHandler(filename=Path(input_file).parent/'python_ags4.log', maxBytes=100e3, backupCount=1)])
-
-    else:
-        logging.basicConfig(level=logging.CRITICAL)
+        file_handler = RotatingFileHandler(filename=Path(input_file).parent/'python_ags4.log',
+                                        maxBytes=100e3,
+                                        backupCount=1)
+        file_formatter = logging.Formatter('{asctime}  {levelname:<8}  {module}.{funcName:<20}  {message}',
+                                        style='{',
+                                        datefmt='%Y-%m-%d %H:%M:%S')
+        file_handler.setFormatter(file_formatter)
+        logger.addHandler(file_handler)
 
     # Run validation
     if input_file.lower().endswith('.ags'):
         console.print(f'[green]Running [bold]python_ags4 v{__version__}[/bold][/green]')
         console.print(f'[green]Opening file... [bold]{input_file}[/bold][/green]')
         console.print('')
 
@@ -329,14 +340,21 @@
         # Write other AGS Format error messages
         for key in [x for x in ags_errors if 'AGS Format Rule' in x]:
             console.print(f'''[white underline]{key}[/white underline]:''')
             for entry in ags_errors[key]:
                 console.print(f'''  Line {entry['line']}\t [bold]{entry['group'].strip('"')}[/bold]\t {entry['desc']}''')
             console.print('')
 
+        # Write parsing and process error messages
+        for key in [x for x in ags_errors if 'Validator Process Error' in x]:
+            console.print(f'''[white underline]{key}[/white underline]:''')
+            for entry in ags_errors[key]:
+                console.print(f'''  Line {entry['line']}\t [bold]{entry['group'].strip('"')}[/bold]\t {entry['desc']}''')
+            console.print('')
+
         # Print warnings
         if show_warnings is True:
             for key in [x for x in ags_errors if 'Warning' in x]:
                 console.print(f'''[white underline]{key}[/white underline]:''')
                 for entry in ags_errors[key]:
                     console.print(f'''  Line {entry['line']}\t [bold]{entry['group'].strip('"')}[/bold]\t {entry['desc']}''')
                 console.print('')
```

### Comparing `python_ags4-0.5.0/python_ags4/check.py` & `python_ags4-0.6.0/python_ags4/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,35 +92,31 @@
     -------
     Pandas DataFrame
         Dataframe with combined DICT tables.
     """
 
     from pandas import DataFrame, concat
     from .AGS4 import AGS4Error
-    from rich import print as rprint
 
     # Initialize DataFrame to hold all dictionary entries
     master_DICT = DataFrame()
 
     for item in ags_tables:
         try:
 
             master_DICT = concat([master_DICT, item['DICT']])
 
         except KeyError:
             # KeyError if there is no DICT table in an input file
-            rprint('[yellow]  WARNING: DICT group not found in input file.[/yellow]')
             logger.warning('DICT group not found in input file.')
 
     # Check whether master_DICT is empty
     if master_DICT.shape[0] == 0:
         msg = 'No DICT groups available to proceed with checking. '\
               'Please ensure the input file has a DICT group or provide file with standard AGS4 dictionary.'
-
-        rprint(f'[red]  ERROR: {msg}[/red]')
         logger.error(msg)
 
         raise AGS4Error(msg)
 
     # Drop duplicate entries
     master_DICT.drop_duplicates(['HEADING', 'DICT_TYPE', 'DICT_GRP', 'DICT_HDNG'], keep='first', inplace=True)
 
@@ -194,47 +190,41 @@
     Returns
     -------
     str
       File path to standard dictionary
     """
 
     from pathlib import Path
-    from rich import print as rprint
 
     # Select standard dictionary based on TRAN_AGS
     try:
         if dict_version is None:
             TRAN = tables['TRAN']
             dict_version = TRAN.loc[TRAN.HEADING.eq('DATA'), 'TRAN_AGS'].values[0]
 
         if dict_version in STANDARD_DICT_FILES.keys():
             path_to_standard_dictionary = Path(__file__).parent / STANDARD_DICT_FILES[dict_version]
 
         else:
-            rprint('[yellow]  WARNING: Standard dictionary for AGS4 version specified in TRAN_AGS not available.[/yellow]')
-            rprint(f'[yellow]           Defaulting to standard dictionary v{LATEST_DICT_VERSION}.[/yellow]')
             logger.warning('Standard dictionary for AGS4 version specified in TRAN_AGS not available. '
                            f'Defaulting to standard dictionary v{LATEST_DICT_VERSION}.')
             path_to_standard_dictionary = Path(__file__).parent / STANDARD_DICT_FILES[LATEST_DICT_VERSION]
 
     except KeyError:
         # TRAN table not in file
-        rprint(f'[yellow]  WARNING: TRAN_AGS not found. Defaulting to standard dictionary v{LATEST_DICT_VERSION}.[/yellow]')
         logger.warning(f'TRAN_AGS not found. Defaulting to standard dictionary v{LATEST_DICT_VERSION}.')
         path_to_standard_dictionary = Path(__file__).parent / STANDARD_DICT_FILES[LATEST_DICT_VERSION]
 
     except IndexError:
         # No DATA rows in TRAN table
-        rprint(f'[yellow]  WARNING: TRAN_AGS not found. Defaulting to standard dictionary v{LATEST_DICT_VERSION}.[/yellow]')
         logger.warning(f'TRAN_AGS not found. Defaulting to standard dictionary v{LATEST_DICT_VERSION}.')
         path_to_standard_dictionary = Path(__file__).parent / STANDARD_DICT_FILES[LATEST_DICT_VERSION]
 
     except TypeError:
         # TRAN table not found and dict_version not valid
-        rprint(f'[yellow]  WARNING: Neither TRAN_AGS nor dict_version is valid. Defaulting to standard dictionary v{LATEST_DICT_VERSION}.[/yellow]')
         logger.warning(f'TRAN_AGS not found. Defaulting to standard dictionary v{LATEST_DICT_VERSION}.')
         path_to_standard_dictionary = Path(__file__).parent / STANDARD_DICT_FILES[LATEST_DICT_VERSION]
 
     return path_to_standard_dictionary
 
 
 def add_meta_data(filepath_or_buffer, standard_dictionary, ags_errors={}, encoding='utf-8'):
```

### Comparing `python_ags4-0.5.0/python_ags4/data/test_data.ags` & `python_ags4-0.6.0/python_ags4/data/test_data.ags`

 * *Files identical despite different names*

### Comparing `python_ags4-0.5.0/PKG-INFO` & `python_ags4-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: python-AGS4
-Version: 0.5.0
+Version: 0.6.0
 Summary: A library to read, write, and check AGS4 files using Pandas DataFrames
 Home-page: https://github.com/asitha-sena/python-AGS4
 License: LGPL-3.0
 Author: Asitha Senanayake
 Author-email: asitha_sena@yahoo.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=7.0,<9.0)
 Requires-Dist: defusedxml (>=0.6,<0.8)
 Requires-Dist: openpyxl (>=3.0,<4.0)
-Requires-Dist: pandas (>=2.0,<3.0)
+Requires-Dist: pandas (>=2.1,<3.0)
 Requires-Dist: rich (>=9.0,<14.0)
 Project-URL: Repository, https://gitlab.com/ags-data-format-wg/ags-python-library
 Description-Content-Type: text/markdown
 
 ![PyPI](https://img.shields.io/pypi/v/python-ags4?label=Current%20Release)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/python-ags4?label=Downloads%20pypi)
 ![Conda](https://img.shields.io/conda/dn/conda-forge/python-ags4?label=Downloads%20conda-forge)
```

