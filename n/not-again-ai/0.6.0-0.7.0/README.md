# Comparing `tmp/not_again_ai-0.6.0.tar.gz` & `tmp/not_again_ai-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not_again_ai-0.6.0.tar", max compression
+gzip compressed data, was "not_again_ai-0.7.0.tar", max compression
```

## Comparing `not_again_ai-0.6.0.tar` & `not_again_ai-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,29 @@
--rw-r--r--   0        0        0     1071 2024-01-28 17:31:42.037063 not_again_ai-0.6.0/LICENSE
--rw-r--r--   0        0        0    14407 2024-04-20 17:53:46.881490 not_again_ai-0.6.0/README.md
--rw-r--r--   0        0        0     4145 2024-04-20 19:07:12.112393 not_again_ai-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.6.0/src/not_again_ai/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 01:25:46.292824 not_again_ai-0.6.0/src/not_again_ai/base/__init__.py
--rw-r--r--   0        0        0      344 2023-10-22 01:25:46.292824 not_again_ai-0.6.0/src/not_again_ai/base/file_system.py
--rw-r--r--   0        0        0     3448 2023-10-22 01:25:46.292824 not_again_ai-0.6.0/src/not_again_ai/base/parallel.py
--rw-r--r--   0        0        0      451 2024-04-20 17:53:46.881490 not_again_ai-0.6.0/src/not_again_ai/llm/__init__.py
--rw-r--r--   0        0        0     8528 2024-04-20 18:00:17.873978 not_again_ai-0.6.0/src/not_again_ai/llm/chat_completion.py
--rw-r--r--   0        0        0     3424 2024-02-04 00:26:08.346905 not_again_ai-0.6.0/src/not_again_ai/llm/context_management.py
--rw-r--r--   0        0        0     2500 2024-01-29 00:33:04.305624 not_again_ai-0.6.0/src/not_again_ai/llm/embeddings.py
--rw-r--r--   0        0        0     2470 2024-01-28 00:29:53.278594 not_again_ai-0.6.0/src/not_again_ai/llm/openai_client.py
--rw-r--r--   0        0        0     7094 2024-04-20 19:17:25.528556 not_again_ai-0.6.0/src/not_again_ai/llm/prompts.py
--rw-r--r--   0        0        0     4301 2024-04-20 19:20:27.986968 not_again_ai-0.6.0/src/not_again_ai/llm/tokens.py
--rw-r--r--   0        0        0       93 2022-11-20 15:38:49.234719 not_again_ai-0.6.0/src/not_again_ai/py.typed
--rw-r--r--   0        0        0      466 2024-04-20 17:53:46.881490 not_again_ai-0.6.0/src/not_again_ai/statistics/__init__.py
--rw-r--r--   0        0        0     4429 2024-01-28 00:06:13.617140 not_again_ai-0.6.0/src/not_again_ai/statistics/dependence.py
--rw-r--r--   0        0        0      447 2024-04-20 17:53:46.881490 not_again_ai-0.6.0/src/not_again_ai/viz/__init__.py
--rw-r--r--   0        0        0     3382 2023-11-19 21:07:35.038071 not_again_ai-0.6.0/src/not_again_ai/viz/barplots.py
--rw-r--r--   0        0        0     4354 2023-10-22 01:25:46.292824 not_again_ai-0.6.0/src/not_again_ai/viz/distributions.py
--rw-r--r--   0        0        0     2290 2023-10-22 01:25:46.292824 not_again_ai-0.6.0/src/not_again_ai/viz/scatterplot.py
--rw-r--r--   0        0        0     5212 2024-01-27 23:36:54.323725 not_again_ai-0.6.0/src/not_again_ai/viz/time_series.py
--rw-r--r--   0        0        0      238 2022-11-20 15:38:49.234719 not_again_ai-0.6.0/src/not_again_ai/viz/utils.py
--rw-r--r--   0        0        0    15966 1970-01-01 00:00:00.000000 not_again_ai-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-01-28 17:31:42.037063 not_again_ai-0.7.0/LICENSE
+-rw-r--r--   0        0        0    12588 2024-05-05 20:32:34.349097 not_again_ai-0.7.0/README.md
+-rw-r--r--   0        0        0     4258 2024-05-05 20:20:05.431962 not_again_ai-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.7.0/src/not_again_ai/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 01:25:46.292824 not_again_ai-0.7.0/src/not_again_ai/base/__init__.py
+-rw-r--r--   0        0        0      949 2024-05-05 19:23:23.729901 not_again_ai-0.7.0/src/not_again_ai/base/file_system.py
+-rw-r--r--   0        0        0     3448 2023-10-22 01:25:46.292824 not_again_ai-0.7.0/src/not_again_ai/base/parallel.py
+-rw-r--r--   0        0        0      451 2024-04-20 17:53:46.881490 not_again_ai-0.7.0/src/not_again_ai/llm/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 23:24:18.378976 not_again_ai-0.7.0/src/not_again_ai/llm/ollama/__init__.py
+-rw-r--r--   0        0        0     3682 2024-05-05 15:31:46.904124 not_again_ai-0.7.0/src/not_again_ai/llm/ollama/chat_completion.py
+-rw-r--r--   0        0        0      765 2024-05-05 17:54:10.555899 not_again_ai-0.7.0/src/not_again_ai/llm/ollama/ollama_client.py
+-rw-r--r--   0        0        0     2900 2024-05-05 15:41:24.299807 not_again_ai-0.7.0/src/not_again_ai/llm/ollama/service.py
+-rw-r--r--   0        0        0        0 2024-05-05 15:59:08.566121 not_again_ai-0.7.0/src/not_again_ai/llm/openai/__init__.py
+-rw-r--r--   0        0        0     8623 2024-05-05 16:51:37.036182 not_again_ai-0.7.0/src/not_again_ai/llm/openai/chat_completion.py
+-rw-r--r--   0        0        0     3431 2024-05-05 16:01:20.819891 not_again_ai-0.7.0/src/not_again_ai/llm/openai/context_management.py
+-rw-r--r--   0        0        0     2500 2024-01-29 00:33:04.305624 not_again_ai-0.7.0/src/not_again_ai/llm/openai/embeddings.py
+-rw-r--r--   0        0        0     2470 2024-01-28 00:29:53.278594 not_again_ai-0.7.0/src/not_again_ai/llm/openai/openai_client.py
+-rw-r--r--   0        0        0     7094 2024-04-20 19:17:25.528556 not_again_ai-0.7.0/src/not_again_ai/llm/openai/prompts.py
+-rw-r--r--   0        0        0     4301 2024-04-20 19:20:27.986968 not_again_ai-0.7.0/src/not_again_ai/llm/openai/tokens.py
+-rw-r--r--   0        0        0       93 2022-11-20 15:38:49.234719 not_again_ai-0.7.0/src/not_again_ai/py.typed
+-rw-r--r--   0        0        0      466 2024-04-20 17:53:46.881490 not_again_ai-0.7.0/src/not_again_ai/statistics/__init__.py
+-rw-r--r--   0        0        0     4429 2024-01-28 00:06:13.617140 not_again_ai-0.7.0/src/not_again_ai/statistics/dependence.py
+-rw-r--r--   0        0        0      447 2024-04-20 17:53:46.881490 not_again_ai-0.7.0/src/not_again_ai/viz/__init__.py
+-rw-r--r--   0        0        0     3382 2023-11-19 21:07:35.038071 not_again_ai-0.7.0/src/not_again_ai/viz/barplots.py
+-rw-r--r--   0        0        0     4354 2023-10-22 01:25:46.292824 not_again_ai-0.7.0/src/not_again_ai/viz/distributions.py
+-rw-r--r--   0        0        0     2290 2023-10-22 01:25:46.292824 not_again_ai-0.7.0/src/not_again_ai/viz/scatterplot.py
+-rw-r--r--   0        0        0     5212 2024-01-27 23:36:54.323725 not_again_ai-0.7.0/src/not_again_ai/viz/time_series.py
+-rw-r--r--   0        0        0      238 2022-11-20 15:38:49.234719 not_again_ai-0.7.0/src/not_again_ai/viz/utils.py
+-rw-r--r--   0        0        0    14203 1970-01-01 00:00:00.000000 not_again_ai-0.7.0/PKG-INFO
```

### Comparing `not_again_ai-0.6.0/LICENSE` & `not_again_ai-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.6.0/README.md` & `not_again_ai-0.7.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -9,104 +9,48 @@
 [github-actions-badge]: https://github.com/johnthagen/python-blueprint/workflows/python/badge.svg
 [poetry-badge]: https://img.shields.io/badge/packaging-poetry-cyan.svg
 [nox-badge]: https://img.shields.io/badge/%F0%9F%A6%8A-Nox-D85E00.svg
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [ruff-badge]: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
 [mypy-badge]: https://www.mypy-lang.org/static/mypy_badge.svg
 
-**not-again-ai** is a collection of various functionalities that come up over and over again when developing AI projects as a Data/Applied/Research Scientist. It is designed to be simple and minimize dependencies first and foremost. This is not meant to reinvent the wheel, but instead be a home for functions that don’t belong well elsewhere. Additionally, feel free to **a)** use this as a template for your own Python package. **b)** instead of installing the package, copy and paste functions into your own projects (this is made easier with the limited amount of dependencies and the MIT license).
+**not-again-ai** is a collection of various building blocks that come up over and over again when developing AI products. The key goals of this package are to have simple, but flexible interfaces and to minimize dependencies. Feel free to **a)** use this as a template for your own Python package. **b)** instead of installing the package, copy and paste functions into your own projects (this is made possible with the limited amount of dependencies and the MIT license).
 
-**Documentation** available within the [readmes](readmes) or auto-generated at [DaveCoDev.github.io/not-again-ai/](https://DaveCoDev.github.io/not-again-ai/).
+**Documentation** available within individual **[notebooks](notebooks)**, docstrings within the source, or auto-generated at [DaveCoDev.github.io/not-again-ai/](https://DaveCoDev.github.io/not-again-ai/).
 
 # Installation
 
 Requires: Python 3.11, or 3.12
 
 Install the entire package from [PyPI](https://pypi.org/project/not-again-ai/) with: 
 
 ```bash
 $ pip install not_again_ai[llm,statistics,viz]
 ```
 
-The package is split into subpackages, so you can install only the parts you need.
+The package is split into subpackages, so you can install only the parts you need. See the **[notebooks](notebooks)** for examples.
 * **Base only**: `pip install not_again_ai`
-* **LLM only**: `pip install not_again_ai[llm]`
+* **LLM**: `pip install not_again_ai[llm]`
+    1. If you wish to use OpenAI
+        1. Go to https://platform.openai.com/settings/profile?tab=api-keys to get your API key.
+        1. (Optionally) Set the `OPENAI_API_KEY` and the `OPENAI_ORG_ID` environment variables.
+    1. If you wish to use Ollama:
+        1. follow the instructions to install ollama for your system: https://github.com/ollama/ollama
+        1. [Add Ollama as a startup service (recommended)](https://github.com/ollama/ollama/blob/main/docs/linux.md#adding-ollama-as-a-startup-service-recommended)
+        1. If you'd like to make the ollama service accessible on your local network and it is hosted on Linux, add the following to the `/etc/systemd/system/ollama.service` file:
+            ```bash
+            [Service]
+            ...
+            Environment="OLLAMA_HOST=0.0.0.0"
+            ```
+        Now ollama will be available at `http://<local_address>:11434`
 * **Statistics**: `pip install not_again_ai[statistics]`
 * **Visualization**: `pip install not_again_ai[viz]`
 
 
-# Quick Tour
-
-## Base
-[README](https://github.com/DaveCoDev/not-again-ai/blob/main/readmes/base.md)
-
-The base package includes only functions that have minimal external dependencies and are useful in a variety of situations such as parallelization and filesystem operations.
-
-## LLM (Large Language Model)
-[README](https://github.com/DaveCoDev/not-again-ai/blob/main/readmes/llm.md), [Example Notebooks](https://github.com/DaveCoDev/not-again-ai/blob/main/notebooks/llm/)
-
-Supports OpenAI chat completions and text embeddings. Includes functions for creating chat completion prompts, token management, and context management.
-
-One example: 
-```python
-client = openai_client()
-messages = [{"role": "system", "content": "You are a helpful assistant."}, {"role": "user", "content": "Hello!"}]
-response = chat_completion(messages=messages, model="gpt-3.5-turbo", max_tokens=100, client=client)["message"]
->>> "Hello! How can I help you today?"
-```
-
-## Statistics
-[README](https://github.com/DaveCoDev/not-again-ai/blob/main/readmes/statistics.md)
-
-We provide a few helpers for data analysis such as:
-
-```python
-from not_again_ai.statistics.dependence import pearson_correlation
-# quadratic dependence
->>> x = (rs.rand(500) * 4) - 2
->>> y = x**2 + (rs.randn(500) * 0.2)
->>> pearson_correlation(x, y)
-0.05
-```
-
-## Visualization
-[README](https://github.com/DaveCoDev/not-again-ai/blob/main/readmes/viz.md)
-
-We offer opinionated wrappers around seaborn to make common visualizations easier to create and customize.
-
-```python
->>> import numpy as np
->>> import pandas as pd
->>> from not_again_ai.viz.time_series import ts_lineplot
->>> from not_again_ai.viz.distributions import univariate_distplot
-
-# get some time series data
->>> rs = np.random.RandomState(365)
->>> values = rs.randn(365, 4).cumsum(axis=0)
->>> dates = pd.date_range('1 1 2021', periods=365, freq='D')
-# plot the time series and save it to a file
->>> ts_lineplot(ts_data=values, save_pathname='myplot.png', ts_x=dates, ts_names=['A', 'B', 'C', 'D'])
-
-# get a random distribution
->>> distrib = np.random.beta(a=0.5, b=0.5, size=1000)
-# plot the distribution and save it to a file
->>> univariate_distplot(
-...     data=distrib, 
-...     save_pathname='mydistribution.svg', 
-...     print_summary=False, bins=100, 
-...     title=r'Beta Distribution $\alpha=0.5, \beta=0.5$'
-... )
-```
-
-<p float="center">
-  <img src="https://raw.githubusercontent.com/DaveCoDev/not-again-ai/44c53fb7fb07234aaceea40c90d8cb74e5fa6c15/assets/distributions_test4.svg" width="404" />
-  <img src="https://raw.githubusercontent.com/DaveCoDev/not-again-ai/44c53fb7fb07234aaceea40c90d8cb74e5fa6c15/assets/ts_lineplot5.svg" width="404" /> 
-</p>
-
-
 # Development Information
 
 The following information is relevant if you would like to contribute or use this package as a template for yourself. 
 
 This package uses [Poetry](https://python-poetry.org/) to manage dependencies and
 isolated [Python virtual environments](https://docs.python.org/3/library/venv.html). To proceed, be sure to first install [pipx](https://github.com/pypa/pipx#install-pipx)
 and then [install Poetry](https://python-poetry.org/docs/#installing-with-pipx).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `not_again_ai-0.6.0/pyproject.toml` & `not_again_ai-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "not-again-ai"
-version = "0.6.0"
+version = "0.7.0"
 description = "Designed to once and for all collect all the little things that come up over and over again in AI projects and put them in one place."
 authors = ["DaveCoDev <dave.co.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/DaveCoDev/not-again-ai"
 documentation = "https://github.com/DaveCoDev/not-again-ai"
 classifiers = [
@@ -24,24 +24,25 @@
 # Some packages, such as scipy, constrain their upper bound of Python versions they support.
 # Without also constraining the upper bound here, Poetry will not select those versions and will
 # result in an old version being resolved/locked.
 python = "^3.11, <3.13"
 
 # Optional dependencies are defined here, and groupings are defined below.
 numpy = { version = "^1.26.4", optional = true }
-openai = { version = "^1.23.2", optional = true }
+ollama = { version = "^0.1.9", optional = true }
+openai = { version = "^1.25.1", optional = true }
 pandas = { version = "^2.2.2", optional = true }
 python-liquid = { version = "^1.12.1", optional = true }
 scipy = { version = "^1.13.0", optional = true }
 scikit-learn = { version = "^1.4.2", optional = true }
 seaborn = { version = "^0.13.2", optional = true }
 tiktoken = { version = "^0.6.0", optional = true }
 
 [tool.poetry.extras]
-llm = ["openai", "python-liquid", "tiktoken"]
+llm = ["ollama", "openai", "python-liquid", "tiktoken"]
 statistics = ["numpy", "scikit-learn", "scipy"]
 viz = ["numpy", "pandas", "seaborn"]
 
 [tool.poetry.dev-dependencies]
 ipykernel = "*"
 
 [tool.poetry.group.nox.dependencies]
@@ -124,11 +125,12 @@
 filterwarnings = [
     # When running tests, treat warnings as errors (e.g. -Werror).
     # See: https://docs.pytest.org/en/latest/reference/reference.html#confval-filterwarnings
     "error",
     # Add additional warning supressions as needed here. For example, if a third-party library
     # is throwing a deprecation warning that needs to be fixed upstream:
     # "ignore::DeprecationWarning:typer",
+    "ignore::pytest.PytestUnraisableExceptionWarning"
 ]
 
 [tool.coverage.run]
 branch = true
```

### Comparing `not_again_ai-0.6.0/src/not_again_ai/base/parallel.py` & `not_again_ai-0.7.0/src/not_again_ai/base/parallel.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.6.0/src/not_again_ai/llm/chat_completion.py` & `not_again_ai-0.7.0/src/not_again_ai/llm/openai/chat_completion.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from typing import Any
 
 from openai import OpenAI
 
 
 def chat_completion(
-    messages: list[dict[str, str]],
+    messages: list[dict[str, Any]],
     model: str,
     client: OpenAI,
     tools: list[dict[str, Any]] | None = None,
     tool_choice: str = "auto",
     max_tokens: int | None = None,
     temperature: float = 0.7,
     json_mode: bool = False,
@@ -29,16 +29,16 @@
         messages (list): A list of messages comprising the conversation so far.
         model (str): ID of the model to use. See the model endpoint compatibility table:
             https://platform.openai.com/docs/models/model-endpoint-compatibility
             for details on which models work with the Chat API.
         client (OpenAI): An instance of the OpenAI client.
         tools (list[dict[str, Any]], optional): A list of tools the model may generate JSON inputs for.
             Defaults to None.
-        tool_choice (str, optional): The tool choice to use. Can be "auto", "none", or a specific function name.
-            Defaults to "auto".
+        tool_choice (str, optional): The tool choice to use. Can be "auto", "required", "none", or a specific function name.
+            Note the function name cannot be any of "auto", "required", or "none". Defaults to "auto".
         max_tokens (int, optional): The maximum number of tokens to generate in the chat completion.
             Defaults to None, which automatically limits to the model's maximum context length.
         temperature (float, optional): What sampling temperature to use, between 0 and 2.
             Higher values like 0.8 will make the output more random,
             while lower values like 0.2 will make it more focused and deterministic. Defaults to 0.7.
         json_mode (bool, optional): When JSON mode is enabled, the model is constrained to only
             generate strings that parse into valid JSON object and will return a dictionary.
@@ -83,15 +83,15 @@
             "response_format": response_format,
             "n": n,
         }
     )
 
     if tools is not None:
         kwargs["tools"] = tools
-        if tool_choice not in ["none", "auto"]:
+        if tool_choice not in ["none", "auto", "required"]:
             kwargs["tool_choice"] = {"type": "function", "function": {"name": tool_choice}}
         else:
             kwargs["tool_choice"] = tool_choice
 
     if seed is not None:
         kwargs["seed"] = seed
```

### Comparing `not_again_ai-0.6.0/src/not_again_ai/llm/context_management.py` & `not_again_ai-0.7.0/src/not_again_ai/llm/openai/context_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 
-from not_again_ai.llm.tokens import num_tokens_from_messages, truncate_str
+from not_again_ai.llm.openai.tokens import num_tokens_from_messages, truncate_str
 
 
 def _inject_variable(
     messages_unformatted: list[dict[str, str]], variable_name: str, variable_text: str
 ) -> list[dict[str, str]]:
     """Injects variables into the messages using Python string formatting."""
     messages_formatted = copy.deepcopy(messages_unformatted)
```

### Comparing `not_again_ai-0.6.0/src/not_again_ai/llm/embeddings.py` & `not_again_ai-0.7.0/src/not_again_ai/llm/openai/embeddings.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.6.0/src/not_again_ai/llm/openai_client.py` & `not_again_ai-0.7.0/src/not_again_ai/llm/openai/openai_client.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.6.0/src/not_again_ai/llm/prompts.py` & `not_again_ai-0.7.0/src/not_again_ai/llm/openai/prompts.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.6.0/src/not_again_ai/llm/tokens.py` & `not_again_ai-0.7.0/src/not_again_ai/llm/openai/tokens.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.6.0/src/not_again_ai/statistics/dependence.py` & `not_again_ai-0.7.0/src/not_again_ai/statistics/dependence.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.6.0/src/not_again_ai/viz/barplots.py` & `not_again_ai-0.7.0/src/not_again_ai/viz/barplots.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.6.0/src/not_again_ai/viz/distributions.py` & `not_again_ai-0.7.0/src/not_again_ai/viz/distributions.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.6.0/src/not_again_ai/viz/scatterplot.py` & `not_again_ai-0.7.0/src/not_again_ai/viz/scatterplot.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.6.0/src/not_again_ai/viz/time_series.py` & `not_again_ai-0.7.0/src/not_again_ai/viz/time_series.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.6.0/PKG-INFO` & `not_again_ai-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not-again-ai
-Version: 0.6.0
+Version: 0.7.0
 Summary: Designed to once and for all collect all the little things that come up over and over again in AI projects and put them in one place.
 Home-page: https://github.com/DaveCoDev/not-again-ai
 License: MIT
 Author: DaveCoDev
 Author-email: dave.co.dev@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: Development Status :: 3 - Alpha
@@ -17,15 +17,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Provides-Extra: llm
 Provides-Extra: statistics
 Provides-Extra: viz
 Requires-Dist: numpy (>=1.26.4,<2.0.0) ; extra == "statistics" or extra == "viz"
-Requires-Dist: openai (>=1.23.2,<2.0.0) ; extra == "llm"
+Requires-Dist: ollama (>=0.1.9,<0.2.0) ; extra == "llm"
+Requires-Dist: openai (>=1.25.1,<2.0.0) ; extra == "llm"
 Requires-Dist: pandas (>=2.2.2,<3.0.0) ; extra == "viz"
 Requires-Dist: python-liquid (>=1.12.1,<2.0.0) ; extra == "llm"
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0) ; extra == "statistics"
 Requires-Dist: scipy (>=1.13.0,<2.0.0) ; extra == "statistics"
 Requires-Dist: seaborn (>=0.13.2,<0.14.0) ; extra == "viz"
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0) ; extra == "llm"
 Project-URL: Documentation, https://github.com/DaveCoDev/not-again-ai
@@ -43,104 +44,48 @@
 [github-actions-badge]: https://github.com/johnthagen/python-blueprint/workflows/python/badge.svg
 [poetry-badge]: https://img.shields.io/badge/packaging-poetry-cyan.svg
 [nox-badge]: https://img.shields.io/badge/%F0%9F%A6%8A-Nox-D85E00.svg
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [ruff-badge]: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
 [mypy-badge]: https://www.mypy-lang.org/static/mypy_badge.svg
 
-**not-again-ai** is a collection of various functionalities that come up over and over again when developing AI projects as a Data/Applied/Research Scientist. It is designed to be simple and minimize dependencies first and foremost. This is not meant to reinvent the wheel, but instead be a home for functions that don’t belong well elsewhere. Additionally, feel free to **a)** use this as a template for your own Python package. **b)** instead of installing the package, copy and paste functions into your own projects (this is made easier with the limited amount of dependencies and the MIT license).
+**not-again-ai** is a collection of various building blocks that come up over and over again when developing AI products. The key goals of this package are to have simple, but flexible interfaces and to minimize dependencies. Feel free to **a)** use this as a template for your own Python package. **b)** instead of installing the package, copy and paste functions into your own projects (this is made possible with the limited amount of dependencies and the MIT license).
 
-**Documentation** available within the [readmes](readmes) or auto-generated at [DaveCoDev.github.io/not-again-ai/](https://DaveCoDev.github.io/not-again-ai/).
+**Documentation** available within individual **[notebooks](notebooks)**, docstrings within the source, or auto-generated at [DaveCoDev.github.io/not-again-ai/](https://DaveCoDev.github.io/not-again-ai/).
 
 # Installation
 
 Requires: Python 3.11, or 3.12
 
 Install the entire package from [PyPI](https://pypi.org/project/not-again-ai/) with: 
 
 ```bash
 $ pip install not_again_ai[llm,statistics,viz]
 ```
 
-The package is split into subpackages, so you can install only the parts you need.
+The package is split into subpackages, so you can install only the parts you need. See the **[notebooks](notebooks)** for examples.
 * **Base only**: `pip install not_again_ai`
-* **LLM only**: `pip install not_again_ai[llm]`
+* **LLM**: `pip install not_again_ai[llm]`
+    1. If you wish to use OpenAI
+        1. Go to https://platform.openai.com/settings/profile?tab=api-keys to get your API key.
+        1. (Optionally) Set the `OPENAI_API_KEY` and the `OPENAI_ORG_ID` environment variables.
+    1. If you wish to use Ollama:
+        1. follow the instructions to install ollama for your system: https://github.com/ollama/ollama
+        1. [Add Ollama as a startup service (recommended)](https://github.com/ollama/ollama/blob/main/docs/linux.md#adding-ollama-as-a-startup-service-recommended)
+        1. If you'd like to make the ollama service accessible on your local network and it is hosted on Linux, add the following to the `/etc/systemd/system/ollama.service` file:
+            ```bash
+            [Service]
+            ...
+            Environment="OLLAMA_HOST=0.0.0.0"
+            ```
+        Now ollama will be available at `http://<local_address>:11434`
 * **Statistics**: `pip install not_again_ai[statistics]`
 * **Visualization**: `pip install not_again_ai[viz]`
 
 
-# Quick Tour
-
-## Base
-[README](https://github.com/DaveCoDev/not-again-ai/blob/main/readmes/base.md)
-
-The base package includes only functions that have minimal external dependencies and are useful in a variety of situations such as parallelization and filesystem operations.
-
-## LLM (Large Language Model)
-[README](https://github.com/DaveCoDev/not-again-ai/blob/main/readmes/llm.md), [Example Notebooks](https://github.com/DaveCoDev/not-again-ai/blob/main/notebooks/llm/)
-
-Supports OpenAI chat completions and text embeddings. Includes functions for creating chat completion prompts, token management, and context management.
-
-One example: 
-```python
-client = openai_client()
-messages = [{"role": "system", "content": "You are a helpful assistant."}, {"role": "user", "content": "Hello!"}]
-response = chat_completion(messages=messages, model="gpt-3.5-turbo", max_tokens=100, client=client)["message"]
->>> "Hello! How can I help you today?"
-```
-
-## Statistics
-[README](https://github.com/DaveCoDev/not-again-ai/blob/main/readmes/statistics.md)
-
-We provide a few helpers for data analysis such as:
-
-```python
-from not_again_ai.statistics.dependence import pearson_correlation
-# quadratic dependence
->>> x = (rs.rand(500) * 4) - 2
->>> y = x**2 + (rs.randn(500) * 0.2)
->>> pearson_correlation(x, y)
-0.05
-```
-
-## Visualization
-[README](https://github.com/DaveCoDev/not-again-ai/blob/main/readmes/viz.md)
-
-We offer opinionated wrappers around seaborn to make common visualizations easier to create and customize.
-
-```python
->>> import numpy as np
->>> import pandas as pd
->>> from not_again_ai.viz.time_series import ts_lineplot
->>> from not_again_ai.viz.distributions import univariate_distplot
-
-# get some time series data
->>> rs = np.random.RandomState(365)
->>> values = rs.randn(365, 4).cumsum(axis=0)
->>> dates = pd.date_range('1 1 2021', periods=365, freq='D')
-# plot the time series and save it to a file
->>> ts_lineplot(ts_data=values, save_pathname='myplot.png', ts_x=dates, ts_names=['A', 'B', 'C', 'D'])
-
-# get a random distribution
->>> distrib = np.random.beta(a=0.5, b=0.5, size=1000)
-# plot the distribution and save it to a file
->>> univariate_distplot(
-...     data=distrib, 
-...     save_pathname='mydistribution.svg', 
-...     print_summary=False, bins=100, 
-...     title=r'Beta Distribution $\alpha=0.5, \beta=0.5$'
-... )
-```
-
-<p float="center">
-  <img src="https://raw.githubusercontent.com/DaveCoDev/not-again-ai/44c53fb7fb07234aaceea40c90d8cb74e5fa6c15/assets/distributions_test4.svg" width="404" />
-  <img src="https://raw.githubusercontent.com/DaveCoDev/not-again-ai/44c53fb7fb07234aaceea40c90d8cb74e5fa6c15/assets/ts_lineplot5.svg" width="404" /> 
-</p>
-
-
 # Development Information
 
 The following information is relevant if you would like to contribute or use this package as a template for yourself. 
 
 This package uses [Poetry](https://python-poetry.org/) to manage dependencies and
 isolated [Python virtual environments](https://docs.python.org/3/library/venv.html). To proceed, be sure to first install [pipx](https://github.com/pypa/pipx#install-pipx)
 and then [install Poetry](https://python-poetry.org/docs/#installing-with-pipx).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

