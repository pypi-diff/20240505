# Comparing `tmp/pyretailscience-0.3.0.tar.gz` & `tmp/pyretailscience-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyretailscience-0.3.0.tar", max compression
+gzip compressed data, was "pyretailscience-0.3.1.tar", max compression
```

## Comparing `pyretailscience-0.3.0.tar` & `pyretailscience-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3860 2024-04-26 11:18:31.449879 pyretailscience-0.3.0/LICENSE
--rw-r--r--   0        0        0     2701 2024-04-26 11:18:31.449879 pyretailscience-0.3.0/README.md
--rw-r--r--   0        0        0     1056 2024-04-26 11:19:40.609992 pyretailscience-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/__init__.py
--rw-r--r--   0        0        0    15090 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/customer.py
--rw-r--r--   0        0        0        0 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/data/__init__.py
--rw-r--r--   0        0        0     1165 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/data/cli.py
--rw-r--r--   0        0        0    17441 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/data/contracts.py
--rw-r--r--   0        0        0    16021 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/data/simulation.py
--rw-r--r--   0        0        0    12493 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/range_planning.py
--rw-r--r--   0        0        0     9192 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/segmentation.py
--rw-r--r--   0        0        0     3528 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/standard_graphs.py
--rw-r--r--   0        0        0     2488 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/style/graph_utils.py
--rw-r--r--   0        0        0     9316 2024-04-26 11:18:31.457879 pyretailscience-0.3.0/pyretailscience/style/tailwind.py
--rw-r--r--   0        0        0     3707 1970-01-01 00:00:00.000000 pyretailscience-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3860 2024-05-05 14:29:57.465611 pyretailscience-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2701 2024-05-05 14:29:57.465611 pyretailscience-0.3.1/README.md
+-rw-r--r--   0        0        0     1056 2024-05-05 14:31:03.313428 pyretailscience-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/__init__.py
+-rw-r--r--   0        0        0    15090 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/customer.py
+-rw-r--r--   0        0        0        0 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/data/__init__.py
+-rw-r--r--   0        0        0     1165 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/data/cli.py
+-rw-r--r--   0        0        0    17162 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/data/contracts.py
+-rw-r--r--   0        0        0    16021 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/data/simulation.py
+-rw-r--r--   0        0        0    12898 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/range_planning.py
+-rw-r--r--   0        0        0     9192 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/segmentation.py
+-rw-r--r--   0        0        0     3528 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/standard_graphs.py
+-rw-r--r--   0        0        0     2488 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/style/graph_utils.py
+-rw-r--r--   0        0        0     9316 2024-05-05 14:29:57.473611 pyretailscience-0.3.1/pyretailscience/style/tailwind.py
+-rw-r--r--   0        0        0     3707 1970-01-01 00:00:00.000000 pyretailscience-0.3.1/PKG-INFO
```

### Comparing `pyretailscience-0.3.0/LICENSE` & `pyretailscience-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.3.0/README.md` & `pyretailscience-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.3.0/pyproject.toml` & `pyretailscience-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyretailscience"
-version = "0.3.0"
+version = "0.3.1"
 description = "Retail Data Science Tools"
 authors = ["Murray Vanwyk <2493311+mvanwyk@users.noreply.github.com>"]
 readme = "README.md"
 license = "Elastic-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `pyretailscience-0.3.0/pyretailscience/customer.py` & `pyretailscience-0.3.1/pyretailscience/customer.py`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.3.0/pyretailscience/data/cli.py` & `pyretailscience-0.3.1/pyretailscience/data/cli.py`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.3.0/pyretailscience/data/contracts.py` & `pyretailscience-0.3.1/pyretailscience/data/contracts.py`

 * *Files 18% similar despite different names*

```diff
@@ -79,14 +79,59 @@
                 "element_count": len(self),
                 "missing_count": nulls.sum().sum(),
                 "missing_percent": nulls.mean().mean(),
             },
         }
 
 
+def build_expected_columns(columns: list[str]) -> list[ExpectationConfiguration]:
+    """A helper function that builds a list of expectations for the columns to exist.
+
+    Args:
+        columns (list[str]): A list of columns to build the expectations for.
+
+    Returns:
+        list[ExpectationConfiguration]: A list of expectations for the columns to exist.
+    """
+    return [
+        ExpectationConfiguration(expectation_type="expect_column_to_exist", kwargs={"column": column})
+        for column in columns
+    ]
+
+
+def build_expected_unique_columns(columns: list[str]) -> list[ExpectationConfiguration]:
+    """A helper function that builds a list of expectations for the columns to have unique values.
+
+    Args:
+        columns (list[str]): A list of columns to build the expectations for.
+
+    Returns:
+        list[ExpectationConfiguration]: A list of expectations for the columns to have unique values.
+    """
+    return [
+        ExpectationConfiguration(expectation_type="expect_column_values_to_be_unique", kwargs={"column": column})
+        for column in columns
+    ]
+
+
+def build_non_null_columns(columns: list[list[str]]) -> list[ExpectationConfiguration]:
+    """A helper function that builds a list of expectations for the columns to have no null values.
+
+    Args:
+        columns (list[list[str]]): A list of columns to build the expectations for.
+
+    Returns:
+        list[ExpectationConfiguration]: A list of expectations for the columns to have no null values.
+    """
+    return [
+        ExpectationConfiguration(expectation_type="expect_column_values_to_not_be_null", kwargs={"column": column})
+        for column in columns
+    ]
+
+
 class ContractBase(abc.ABC):
     """Base class for data contracts. It contains the basic and extended expectations for the data, as well as the
     validation state and the result of the last validation. It also contains a method to validate the data.
 
     Attributes:
         basic_expectations (list[ExpectationConfiguration]): A list of basic expectations for the data.
         extended_expectations (list[ExpectationConfiguration]): A list of extended expectations for the data.
@@ -176,73 +221,37 @@
             2029-12-31, and that the transaction_id, transaction_datetime, customer_id, and store_id columns have unique
             combinations.
         validation_state (EValidationState): The validation state of the data.
         expectations_run (EExpectationSet | None): The expectation set that was run in the last validation.
         validation_result (dict): The result of the last validation.
     """
 
-    basic_expectations = [
-        ExpectationConfiguration(
-            expectation_type="expect_column_to_exist",
-            kwargs={"column": "transaction_id"},
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_column_to_exist",
-            kwargs={"column": "transaction_datetime"},
-        ),
-        ExpectationConfiguration(expectation_type="expect_column_to_exist", kwargs={"column": "customer_id"}),
-        ExpectationConfiguration(expectation_type="expect_column_to_exist", kwargs={"column": "total_price"}),
-        ExpectationConfiguration(expectation_type="expect_column_to_exist", kwargs={"column": "store_id"}),
-    ]
-
-    extended_expectations = [
-        ExpectationConfiguration(
-            expectation_type="expect_column_values_to_be_unique",
-            kwargs={"column": "transaction_id"},
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_compound_columns_to_be_unique",
-            kwargs={
-                "column_list": [
-                    "transaction_id",
-                    "transaction_datetime",
-                    "customer_id",
-                    "store_id",
-                ]
-            },
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_column_values_to_be_between",
-            kwargs={
-                "column": "transaction_datetime",
-                "min_value": "1970-01-01",
-                "max_value": "2029-12-31",
-            },
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_column_values_to_not_be_null",
-            kwargs={"column": "transaction_id"},
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_column_values_to_not_be_null",
-            kwargs={"column": "transaction_datetime"},
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_column_values_to_not_be_null",
-            kwargs={"column": "customer_id"},
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_column_values_to_not_be_null",
-            kwargs={"column": "total_price"},
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_column_values_to_not_be_null",
-            kwargs={"column": "store_id"},
-        ),
-    ]
+    basic_expectations = build_expected_columns(
+        ["transaction_id", "transaction_datetime", "customer_id", "total_price", "store_id"]
+    )
+
+    extended_expectations = (
+        build_expected_unique_columns(
+            [
+                "transaction_id",
+                ["transaction_datetime", "customer_id", "total_price", "store_id"],
+            ]
+        )
+        + [
+            ExpectationConfiguration(
+                expectation_type="expect_column_values_to_be_between",
+                kwargs={
+                    "column": "transaction_datetime",
+                    "min_value": "1970-01-01",
+                    "max_value": "2029-12-31",
+                },
+            )
+        ]
+        + build_non_null_columns(["transaction_id", "transaction_datetime", "customer_id", "total_price", "store_id"])
+    )
 
 
 class TransactionItemLevelContract(ContractBase):
     """Data contract for the transaction item level data. It contains the basic and extended expectations for the data,
     as well as the validation state and the result of the last validation. It also contains a method to validate the
     data.
 
@@ -259,31 +268,27 @@
         validation_result (dict): The result of the last validation.
 
     Args:
         df (pd.DataFrame): The DataFrame to be validated. If category or brand columns are present, it adds expectations
             that these columns are not null.
     """
 
-    basic_expectations = [
-        ExpectationConfiguration(
-            expectation_type="expect_column_to_exist",
-            kwargs={"column": "transaction_id"},
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_column_to_exist",
-            kwargs={"column": "transaction_datetime"},
-        ),
-        ExpectationConfiguration(expectation_type="expect_column_to_exist", kwargs={"column": "customer_id"}),
-        ExpectationConfiguration(expectation_type="expect_column_to_exist", kwargs={"column": "total_price"}),
-        ExpectationConfiguration(expectation_type="expect_column_to_exist", kwargs={"column": "store_id"}),
-        ExpectationConfiguration(expectation_type="expect_column_to_exist", kwargs={"column": "product_id"}),
-        ExpectationConfiguration(expectation_type="expect_column_to_exist", kwargs={"column": "product_name"}),
-        ExpectationConfiguration(expectation_type="expect_column_to_exist", kwargs={"column": "unit_price"}),
-        ExpectationConfiguration(expectation_type="expect_column_to_exist", kwargs={"column": "quantity"}),
-    ]
+    basic_expectations = build_expected_columns(
+        [
+            "transaction_id",
+            "transaction_datetime",
+            "customer_id",
+            "total_price",
+            "store_id",
+            "product_id",
+            "product_name",
+            "unit_price",
+            "quantity",
+        ]
+    )
 
     extended_expectations = [
         ExpectationConfiguration(
             expectation_type="expect_compound_columns_to_be_unique",
             kwargs={
                 "column_list": [
                     "transaction_id",
@@ -293,52 +298,26 @@
                 ]
             },
         ),
         ExpectationConfiguration(
             expectation_type="expect_transaction_product_quantity_sign_to_be_unique",
             kwargs={},
         ),
-        # Null expectations
-        ExpectationConfiguration(
-            expectation_type="expect_column_values_to_not_be_null",
-            kwargs={"column": "transaction_id"},
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_column_values_to_not_be_null",
-            kwargs={"column": "transaction_datetime"},
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_column_values_to_not_be_null",
-            kwargs={"column": "customer_id"},
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_column_values_to_not_be_null",
-            kwargs={"column": "total_price"},
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_column_values_to_not_be_null",
-            kwargs={"column": "store_id"},
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_column_values_to_not_be_null",
-            kwargs={"column": "product_id"},
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_column_values_to_not_be_null",
-            kwargs={"column": "product_name"},
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_column_values_to_not_be_null",
-            kwargs={"column": "unit_price"},
-        ),
-        ExpectationConfiguration(
-            expectation_type="expect_column_values_to_not_be_null",
-            kwargs={"column": "quantity"},
-        ),
-    ]
+    ] + build_non_null_columns(
+        [
+            "transaction_id",
+            "transaction_datetime",
+            "customer_id",
+            "store_id",
+            "product_id",
+            "product_name",
+            "unit_price",
+            "quantity",
+        ]
+    )
 
     def __init__(self, df: pd.DataFrame) -> None:
         # If category or brand columns are present, add expectations for them
         category_pattern = re.compile(r"category_\d+_(id|name)")
         category_matches = [s for s in df.columns if category_pattern.match(s)]
         for match in category_matches:
             self.extended_expectations.append(
@@ -389,7 +368,41 @@
             kwargs={"column": "customer_id"},
         ),
         ExpectationConfiguration(
             expectation_type="expect_column_values_to_not_be_null",
             kwargs={"column": "customer_id"},
         ),
     ]
+
+
+class CustomContract(ContractBase):
+    """A helper class to construct contracts for specific use cases.
+
+    Args:
+        df (pd.DataFrame): The input DataFrame.
+        basic_expectations (list[ExpectationConfiguration] | None, optional): A list of basic expectation
+            configurations. Defaults to None. At least one basic or extended expectation must be supplied.
+        extended_expectations (list[ExpectationConfiguration] | None, optional): A list of extended expectation
+            configurations. Defaults to None. At least one basic or extended expectation must be supplied.
+
+    Raises:
+        ValueError: If both basic_expectations and extended_expectations are None.
+
+    Attributes:
+        basic_expectations (list[ExpectationConfiguration]): A list of basic expectation configurations.
+        extended_expectations (list[ExpectationConfiguration]): A list of extended expectation configurations.
+
+    """
+
+    def __init__(
+        self,
+        df: pd.DataFrame,
+        basic_expectations: list[ExpectationConfiguration] | None = None,
+        extended_expectations: list[ExpectationConfiguration] | None = None,
+    ) -> None:
+        if basic_expectations is None and extended_expectations is None:
+            raise ValueError("At least one of basic_expectations or extended_expectations must be provided.")
+
+        self.basic_expectations = basic_expectations or []
+        self.extended_expectations = extended_expectations or []
+
+        super().__init__(df)
```

### Comparing `pyretailscience-0.3.0/pyretailscience/data/simulation.py` & `pyretailscience-0.3.1/pyretailscience/data/simulation.py`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.3.0/pyretailscience/range_planning.py` & `pyretailscience-0.3.1/pyretailscience/range_planning.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from matplotlib.axes import Axes, SubplotBase
 from scipy.cluster.hierarchy import dendrogram, linkage
 
 import pyretailscience.style.graph_utils as gu
-from pyretailscience.data.contracts import TransactionItemLevelContract
+from pyretailscience.data.contracts import CustomContract, build_expected_columns, build_non_null_columns
 from pyretailscience.style.graph_utils import GraphStyles as gs
 
 
 class CustomerDecisionHierarchy:
     def __init__(
         self,
         df: pd.DataFrame,
@@ -36,16 +36,25 @@
                 Only applicable if method is "truncated_svd". Defaults to 0.8.
             random_state (int, optional): Random seed for reproducibility. Defaults to 42.
 
         Raises:
             ValueError: If the dataframe does not comply with the TransactionItemLevelContract.
 
         """
-        if TransactionItemLevelContract(df).validate() is False:
-            raise ValueError("The dataframe does not comply with the TransactionItemLevelContract")
+        cdh_contract = CustomContract(
+            df,
+            basic_expectations=build_expected_columns(columns=["customer_id", "transaction_id", "product_name"]),
+            extended_expectations=build_non_null_columns(columns=["customer_id", "transaction_id", "product_name"]),
+        )
+
+        if cdh_contract.validate() is False:
+            raise ValueError(
+                "The dataframe requires the columns 'customer_id', 'transaction_id', and 'product_name' and they must "
+                "be non-null"
+            )
 
         self.random_state = random_state
         self.pairs_df = self._get_pairs(df, exclude_same_transaction_products)
         self.distances = self._calculate_distances(method=method, min_var_explained=min_var_explained)
 
     @staticmethod
     def _get_pairs(df: pd.DataFrame, exclude_same_transaction_products: bool) -> pd.DataFrame:
```

### Comparing `pyretailscience-0.3.0/pyretailscience/segmentation.py` & `pyretailscience-0.3.1/pyretailscience/segmentation.py`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.3.0/pyretailscience/standard_graphs.py` & `pyretailscience-0.3.1/pyretailscience/standard_graphs.py`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.3.0/pyretailscience/style/graph_utils.py` & `pyretailscience-0.3.1/pyretailscience/style/graph_utils.py`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.3.0/pyretailscience/style/tailwind.py` & `pyretailscience-0.3.1/pyretailscience/style/tailwind.py`

 * *Files identical despite different names*

### Comparing `pyretailscience-0.3.0/PKG-INFO` & `pyretailscience-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyretailscience
-Version: 0.3.0
+Version: 0.3.1
 Summary: Retail Data Science Tools
 License: Elastic-2.0
 Author: Murray Vanwyk
 Author-email: 2493311+mvanwyk@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyretailscience Version: 0.3.0 Summary: Retail Data
+Metadata-Version: 2.1 Name: pyretailscience Version: 0.3.1 Summary: Retail Data
 Science Tools License: Elastic-2.0 Author: Murray Vanwyk Author-email:
 2493311+mvanwyk@users.noreply.github.com Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
 (>=8.1.7,<9.0.0) Requires-Dist: great-expectations (>=0.18.8,<0.19.0) Requires-
 Dist: loguru (>=0.7.2,<0.8.0) Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
```

