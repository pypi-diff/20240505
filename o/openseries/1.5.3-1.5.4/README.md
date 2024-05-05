# Comparing `tmp/openseries-1.5.3.tar.gz` & `tmp/openseries-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openseries-1.5.3.tar", max compression
+gzip compressed data, was "openseries-1.5.4.tar", max compression
```

## Comparing `openseries-1.5.3.tar` & `openseries-1.5.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1521 2024-05-01 19:28:47.534606 openseries-1.5.3/LICENSE.md
--rw-r--r--   0        0        0    42009 2024-05-01 19:28:47.534606 openseries-1.5.3/README.md
--rw-r--r--   0        0        0       41 2024-05-01 19:28:47.534606 openseries-1.5.3/openseries/__init__.py
--rw-r--r--   0        0        0    72469 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/_common_model.py
--rw-r--r--   0        0        0     3300 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/_risk.py
--rw-r--r--   0        0        0    12378 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/datefixer.py
--rw-r--r--   0        0        0    74019 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/frame.py
--rw-r--r--   0        0        0     1808 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/load_plotly.py
--rw-r--r--   0        0        0      178 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/plotly_captor_logo.json
--rw-r--r--   0        0        0     1429 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/plotly_layouts.json
--rw-r--r--   0        0        0    28313 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/series.py
--rw-r--r--   0        0        0    13905 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/simulation.py
--rw-r--r--   0        0        0     7597 2024-05-01 19:28:47.538606 openseries-1.5.3/openseries/types.py
--rw-r--r--   0        0        0     2665 2024-05-01 19:28:47.538606 openseries-1.5.3/pyproject.toml
--rw-r--r--   0        0        0    43579 1970-01-01 00:00:00.000000 openseries-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1521 2024-05-05 17:48:03.342128 openseries-1.5.4/LICENSE.md
+-rw-r--r--   0        0        0    42652 2024-05-05 17:48:03.346128 openseries-1.5.4/README.md
+-rw-r--r--   0        0        0       41 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/__init__.py
+-rw-r--r--   0        0        0    74705 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/_common_model.py
+-rw-r--r--   0        0        0     3300 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/_risk.py
+-rw-r--r--   0        0        0    12378 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/datefixer.py
+-rw-r--r--   0        0        0    74019 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/frame.py
+-rw-r--r--   0        0        0     1856 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/load_plotly.py
+-rw-r--r--   0        0        0      178 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/plotly_captor_logo.json
+-rw-r--r--   0        0        0     1429 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/plotly_layouts.json
+-rw-r--r--   0        0        0    28313 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/series.py
+-rw-r--r--   0        0        0    13905 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/simulation.py
+-rw-r--r--   0        0        0     7643 2024-05-05 17:48:03.346128 openseries-1.5.4/openseries/types.py
+-rw-r--r--   0        0        0     2665 2024-05-05 17:48:03.346128 openseries-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0    44222 1970-01-01 00:00:00.000000 openseries-1.5.4/PKG-INFO
```

### Comparing `openseries-1.5.3/LICENSE.md` & `openseries-1.5.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openseries-1.5.3/README.md` & `openseries-1.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [![GitHub Action Test Suite](https://github.com/CaptorAB/openseries/actions/workflows/test.yml/badge.svg)](https://github.com/CaptorAB/openseries/actions/workflows/test.yml)
 [![Coverage](https://cdn.jsdelivr.net/gh/CaptorAB/openseries@master/coverage.svg)](https://github.com/CaptorAB/openseries/actions/workflows/test.yml)
 [![Styling, Linting & Type checks](https://github.com/CaptorAB/openseries/actions/workflows/check.yml/badge.svg)](https://github.com/CaptorAB/openseries/actions/workflows/check.yml)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://beta.ruff.rs/docs/)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
-`openseries` is a project with tools to analyse financial timeseries of a single
+This is a project with tools to analyze financial timeseries of a single
 asset or a group of assets. It is solely made for daily or less frequent data.
 
 <span style="font-size:2em;">[CHANGELOG](https://github.com/CaptorAB/openseries/blob/master/CHANGELOG.md)</span>
 
 
 ## Basic Usage
 
@@ -289,14 +289,15 @@
 | `arithmetic_ret`        | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Annualized arithmetic mean of returns](https://www.investopedia.com/terms/a/arithmeticmean.asp).                                                                                                                       |
 | `geo_ret`               | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Compound Annual Growth Rate(CAGR)](https://www.investopedia.com/terms/c/cagr.asp), a specific implementation of geometric mean.                                                                                        |
 | `value_ret`             | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Simple return from first to last observation.                                                                                                                                                                           |
 | `vol`                   | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Annualized [volatility](https://www.investopedia.com/terms/v/volatility.asp). Pandas .std() is the equivalent of stdev.s([...]) in MS excel.                                                                            |
 | `downside_deviation`    | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Downside deviation](https://www.investopedia.com/terms/d/downside-deviation.asp) is the volatility of all negative return observations. Minimum Accepted Return (MAR) set to zero.                                     |
 | `ret_vol_ratio`         | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Ratio of arithmetic mean return and annualized volatility. It is the [Sharpe Ratio](https://www.investopedia.com/terms/s/sharperatio.asp) with the riskfree rate set to zero.                                           |
 | `sortino_ratio`         | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | The [Sortino Ratio](https://www.investopedia.com/terms/s/sortinoratio.asp) is the arithmetic mean return divided by the downside deviation. This attribute assumes that the riskfree rate and the MAR are both zero.    |
+| `omega_ratio`           | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | The [Omega Ratio](https://en.wikipedia.org/wiki/Omega_ratio) compares returns above a certain target level (MAR) to the total downside risk below MAR.                                                                  |
 | `var_down`              | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Downside 95% [Value At Risk](https://www.investopedia.com/terms/v/var.asp), "VaR". The equivalent of percentile.inc([...], 1-level) over returns in MS Excel. For other confidence levels use the corresponding method. |
 | `cvar_down`             | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Downside 95% [Conditional Value At Risk](https://www.investopedia.com/terms/c/conditional_value_at_risk.asp), "CVaR". For other confidence levels use the corresponding method.                                         |
 | `worst`                 | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Most negative percentage change of a single observation.                                                                                                                                                                |
 | `worst_month`           | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Most negative month.                                                                                                                                                                                                    |
 | `max_drawdown`          | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Maximum drawdown](https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp).                                                                                                                                      |
 | `max_drawdown_cal_year` | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Max drawdown in a single calendar year.                                                                                                                                                                                 |
 | `positive_share`        | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | The share of percentage changes that are positive.                                                                                                                                                                      |
@@ -315,14 +316,15 @@
 | `arithmetic_ret_func`     | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Annualized arithmetic mean of returns](https://www.investopedia.com/terms/a/arithmeticmean.asp).                                                                                                                                                              |
 | `geo_ret_func`            | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Compound Annual Growth Rate(CAGR)](https://www.investopedia.com/terms/c/cagr.asp), a specific implementation of geometric mean.                                                                                                                               |
 | `value_ret_func`          | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Simple return from first to last observation.                                                                                                                                                                                                                  |
 | `vol_func`                | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Annualized [volatility](https://www.investopedia.com/terms/v/volatility.asp). Pandas .std() is the equivalent of stdev.s([...]) in MS excel.                                                                                                                   |
 | `downside_deviation_func` | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Downside deviation](https://www.investopedia.com/terms/d/downside-deviation.asp) is the volatility of all negative return observations. MAR and riskfree rate can be set.                                                                                     |
 | `ret_vol_ratio_func`      | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Ratio of arithmetic mean return and annualized volatility. It is the [Sharpe Ratio](https://www.investopedia.com/terms/s/sharperatio.asp) with the riskfree rate set to zero. A riskfree rate can be set as a float or a series chosen for the frame function. |
 | `sortino_ratio_func`      | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | The [Sortino Ratio](https://www.investopedia.com/terms/s/sortinoratio.asp) is the arithmetic mean return divided by the downside deviation. A riskfree rate can be set as a float or a series chosen for the frame function. MAR is set to zero.               |
+| `omega_ratio_func`        | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | The [Omega Ratio](https://en.wikipedia.org/wiki/Omega_ratio) compares returns above a certain target level (MAR) to the total downside risk below MAR.                                                                                                         |
 | `var_down_func`           | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Downside 95% [Value At Risk](https://www.investopedia.com/terms/v/var.asp), "VaR". The equivalent of percentile.inc([...], 1-level) over returns in MS Excel. Default is 95% confidence level.                                                                 |
 | `cvar_down_func`          | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Downside 95% [Conditional Value At Risk](https://www.investopedia.com/terms/c/conditional_value_at_risk.asp), "CVaR". Default is 95% confidence level.                                                                                                         |
 | `worst_func`              | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Most negative percentage change for a given number of observations (default=1).                                                                                                                                                                                |
 | `max_drawdown_func`       | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Maximum drawdown](https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp).                                                                                                                                                                             |
 | `positive_share_func`     | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | The share of percentage changes that are positive.                                                                                                                                                                                                             |
 | `vol_from_var_func`       | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Implied annualized volatility from the Downside VaR using the assumption that returns are normally distributed.                                                                                                                                                |
 | `skew_func`               | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Skew](https://www.investopedia.com/terms/s/skewness.asp) of the return distribution.                                                                                                                                                                          |
```

### Comparing `openseries-1.5.3/openseries/_common_model.py` & `openseries-1.5.4/openseries/_common_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
             .min()
         )
         if self.tsdf.shape[1] == 1:
             return float(mddc.iloc[0])
         return Series(
             data=mddc,
             index=self.tsdf.columns,
-            name="Max Drawdown in cal yr",
+            name="Max drawdown in cal yr",
             dtype="float64",
         )
 
     @property
     def geo_ret(self: Self) -> Union[float, Series[float]]:
         """
         https://www.investopedia.com/terms/c/cagr.asp.
@@ -272,14 +272,28 @@
         minimum_accepted_return: float = 0.0
         return self.sortino_ratio_func(
             riskfree_rate=riskfree_rate,
             min_accepted_return=minimum_accepted_return,
         )
 
     @property
+    def omega_ratio(self: Self) -> Union[float, Series[float]]:
+        """
+        https://en.wikipedia.org/wiki/Omega_ratio.
+
+        Returns
+        -------
+        Union[float, Pandas.Series[float]]
+            Omega ratio calculation
+
+        """
+        minimum_accepted_return: float = 0.0
+        return self.omega_ratio_func(min_accepted_return=minimum_accepted_return)
+
+    @property
     def z_score(self: Self) -> Union[float, Series[float]]:
         """
         https://www.investopedia.com/terms/z/zscore.asp.
 
         Returns
         -------
         Union[float, Pandas.Series[float]]
@@ -1675,15 +1689,15 @@
             .max()
         ).min() - 1
         if self.tsdf.shape[1] == 1:
             return float(result.iloc[0])
         return Series(
             data=result,
             index=self.tsdf.columns,
-            name="Max Drawdown",
+            name="Max drawdown",
             dtype="float64",
         )
 
     def positive_share_func(
         self: Self,
         months_from_last: Optional[int] = None,
         from_date: Optional[dt.date] = None,
@@ -1731,15 +1745,15 @@
         )
         share = pos / tot
         if self.tsdf.shape[1] == 1:
             return float(share.iloc[0])
         return Series(
             data=share,
             index=self.tsdf.columns,
-            name="Positive Share",
+            name="Positive share",
             dtype="float64",
         )
 
     def ret_vol_ratio_func(
         self: Self,
         riskfree_rate: float = 0.0,
         months_from_last: Optional[int] = None,
@@ -1865,14 +1879,68 @@
         return Series(
             data=ratio,
             index=self.tsdf.columns,
             name="Sortino ratio",
             dtype="float64",
         )
 
+    def omega_ratio_func(
+        self: Self,
+        min_accepted_return: float = 0.0,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
+    ) -> Union[float, Series[float]]:
+        """
+        Omega Ratio.
+
+        The Omega Ratio compares returns above a certain target level
+        (often referred to as the “minimum acceptable return” or “MAR”)
+        to the total downside risk below that same threshold.
+        https://en.wikipedia.org/wiki/Omega_ratio.
+
+        Parameters
+        ----------
+        min_accepted_return : float, optional
+            The annualized Minimum Accepted Return (MAR)
+        months_from_last : int, optional
+            number of months offset as positive integer. Overrides use of from_date
+            and to_date
+        from_date : datetime.date, optional
+            Specific from date
+        to_date : datetime.date, optional
+            Specific to date
+
+        Returns
+        -------
+        Union[float, Pandas.Series[float]]
+            Omega ratio calculation
+
+        """
+        earlier, later = self.calc_range(
+            months_offset=months_from_last,
+            from_dt=from_date,
+            to_dt=to_date,
+        )
+        retdf = self.tsdf.loc[cast(int, earlier) : cast(int, later)].pct_change(
+            fill_method=cast(str, None),
+        )
+        pos = retdf[retdf > min_accepted_return].sub(min_accepted_return).sum()
+        neg = retdf[retdf < min_accepted_return].sub(min_accepted_return).sum()
+        ratio = pos / -neg
+
+        if self.tsdf.shape[1] == 1:
+            return float(cast(float64, ratio.iloc[0]))
+        return Series(
+            data=ratio,
+            index=self.tsdf.columns,
+            name="Omega ratio",
+            dtype="float64",
+        )
+
     def value_ret_func(
         self: Self,
         months_from_last: Optional[int] = None,
         from_date: Optional[dt.date] = None,
         to_date: Optional[dt.date] = None,
     ) -> Union[float, Series[float]]:
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openseries-1.5.3/openseries/_risk.py` & `openseries-1.5.4/openseries/_risk.py`

 * *Files identical despite different names*

### Comparing `openseries-1.5.3/openseries/datefixer.py` & `openseries-1.5.4/openseries/datefixer.py`

 * *Files identical despite different names*

### Comparing `openseries-1.5.3/openseries/frame.py` & `openseries-1.5.4/openseries/frame.py`

 * *Files identical despite different names*

### Comparing `openseries-1.5.3/openseries/load_plotly.py` & `openseries-1.5.4/openseries/load_plotly.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 
 from json import load
 from logging import warning
 from pathlib import Path
 
 import requests
+from requests.exceptions import ConnectionError
 
 from openseries.types import CaptorLogoType, PlotlyLayoutType
 
 
 def _check_remote_file_existence(url: str) -> bool:
     """
     Check if remote file exists.
@@ -28,15 +29,15 @@
     """
     ok_code = 200
 
     try:
         response = requests.head(url, timeout=30)
         if response.status_code != ok_code:
             return False
-    except requests.exceptions.ConnectionError:
+    except ConnectionError:
         return False
     return True
 
 
 def load_plotly_dict(
     *,
     responsive: bool = True,
@@ -55,17 +56,17 @@
         A dictionary with the Plotly config and layout template
 
     """
     project_root = Path(__file__).resolve().parent.parent
     layoutfile = project_root.joinpath("openseries").joinpath("plotly_layouts.json")
     logofile = project_root.joinpath("openseries").joinpath("plotly_captor_logo.json")
 
-    with Path.open(layoutfile, encoding="utf-8") as layout_file:
+    with Path.open(layoutfile, mode="r", encoding="utf-8") as layout_file:
         fig = load(layout_file)
-    with Path.open(logofile, encoding="utf-8") as logo_file:
+    with Path.open(logofile, mode="r", encoding="utf-8") as logo_file:
         logo = load(logo_file)
 
     if _check_remote_file_existence(url=logo["source"]) is False:
         msg = f"Failed to add logo image from URL {logo['source']}"
         warning(msg)
         logo = {}
```

### Comparing `openseries-1.5.3/openseries/plotly_layouts.json` & `openseries-1.5.4/openseries/plotly_layouts.json`

 * *Files identical despite different names*

### Comparing `openseries-1.5.3/openseries/series.py` & `openseries-1.5.4/openseries/series.py`

 * *Files identical despite different names*

### Comparing `openseries-1.5.3/openseries/simulation.py` & `openseries-1.5.4/openseries/simulation.py`

 * *Files identical despite different names*

### Comparing `openseries-1.5.3/openseries/types.py` & `openseries-1.5.4/openseries/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,15 @@
         "value_ret",
         "geo_ret",
         "arithmetic_ret",
         "vol",
         "downside_deviation",
         "ret_vol_ratio",
         "sortino_ratio",
+        "omega_ratio",
         "z_score",
         "skew",
         "kurtosis",
         "positive_share",
         "var_down",
         "cvar_down",
         "vol_from_var",
@@ -272,14 +273,15 @@
         "value_ret",
         "geo_ret",
         "arithmetic_ret",
         "vol",
         "downside_deviation",
         "ret_vol_ratio",
         "sortino_ratio",
+        "omega_ratio",
         "z_score",
         "skew",
         "kurtosis",
         "positive_share",
         "var_down",
         "cvar_down",
         "vol_from_var",
```

### Comparing `openseries-1.5.3/pyproject.toml` & `openseries-1.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openseries"
-version = "1.5.3"
+version = "1.5.4"
 description = "Tools for analyzing financial timeseries."
 authors = ["Martin Karrin <martin.karrin@captor.se>"]
 repository = "https://github.com/CaptorAB/openseries"
 license = "BSD-3-Clause"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.9",
@@ -43,21 +43,21 @@
 pydantic = ">=2.5.2,<3.0.0"
 python-dateutil = ">=2.8.2,<3.0.0"
 requests = ">=2.20.0,<3.0.0"
 scipy = ">=1.11.4,<2.0.0"
 statsmodels = ">=0.14.0,<1.0.0"
 
 [tool.poetry.group.dev.dependencies]
-coverage = "^7.5.0"
+coverage = "^7.5.1"
 coverage-badge = "^1.1.1"
 mypy = "^1.10.0"
 pandas-stubs = "^2.2.1.240316"
 pre-commit = "^3.7.0"
 pytest = "^8.2.0"
-ruff = "^0.4.2"
+ruff = "^0.4.3"
 types-openpyxl = "^3.1.0.20240428"
 types-python-dateutil = "^2.9.0.20240316"
 types-requests = "^2.31.0.20240406"
 
 [build-system]
 requires = ["poetry-core>=1.8.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openseries-1.5.3/PKG-INFO` & `openseries-1.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openseries
-Version: 1.5.3
+Version: 1.5.4
 Summary: Tools for analyzing financial timeseries.
 Home-page: https://github.com/CaptorAB/openseries
 License: BSD-3-Clause
 Keywords: python,finance,fintech,data-science,timeseries,timeseries-data,timeseries-analysis,investment,investment-analysis,investing
 Author: Martin Karrin
 Author-email: martin.karrin@captor.se
 Requires-Python: >=3.9,<3.13
@@ -49,15 +49,15 @@
 [![GitHub Action Test Suite](https://github.com/CaptorAB/openseries/actions/workflows/test.yml/badge.svg)](https://github.com/CaptorAB/openseries/actions/workflows/test.yml)
 [![Coverage](https://cdn.jsdelivr.net/gh/CaptorAB/openseries@master/coverage.svg)](https://github.com/CaptorAB/openseries/actions/workflows/test.yml)
 [![Styling, Linting & Type checks](https://github.com/CaptorAB/openseries/actions/workflows/check.yml/badge.svg)](https://github.com/CaptorAB/openseries/actions/workflows/check.yml)
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://beta.ruff.rs/docs/)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
-`openseries` is a project with tools to analyse financial timeseries of a single
+This is a project with tools to analyze financial timeseries of a single
 asset or a group of assets. It is solely made for daily or less frequent data.
 
 <span style="font-size:2em;">[CHANGELOG](https://github.com/CaptorAB/openseries/blob/master/CHANGELOG.md)</span>
 
 
 ## Basic Usage
 
@@ -325,14 +325,15 @@
 | `arithmetic_ret`        | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Annualized arithmetic mean of returns](https://www.investopedia.com/terms/a/arithmeticmean.asp).                                                                                                                       |
 | `geo_ret`               | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Compound Annual Growth Rate(CAGR)](https://www.investopedia.com/terms/c/cagr.asp), a specific implementation of geometric mean.                                                                                        |
 | `value_ret`             | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Simple return from first to last observation.                                                                                                                                                                           |
 | `vol`                   | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Annualized [volatility](https://www.investopedia.com/terms/v/volatility.asp). Pandas .std() is the equivalent of stdev.s([...]) in MS excel.                                                                            |
 | `downside_deviation`    | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Downside deviation](https://www.investopedia.com/terms/d/downside-deviation.asp) is the volatility of all negative return observations. Minimum Accepted Return (MAR) set to zero.                                     |
 | `ret_vol_ratio`         | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Ratio of arithmetic mean return and annualized volatility. It is the [Sharpe Ratio](https://www.investopedia.com/terms/s/sharperatio.asp) with the riskfree rate set to zero.                                           |
 | `sortino_ratio`         | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | The [Sortino Ratio](https://www.investopedia.com/terms/s/sortinoratio.asp) is the arithmetic mean return divided by the downside deviation. This attribute assumes that the riskfree rate and the MAR are both zero.    |
+| `omega_ratio`           | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | The [Omega Ratio](https://en.wikipedia.org/wiki/Omega_ratio) compares returns above a certain target level (MAR) to the total downside risk below MAR.                                                                  |
 | `var_down`              | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Downside 95% [Value At Risk](https://www.investopedia.com/terms/v/var.asp), "VaR". The equivalent of percentile.inc([...], 1-level) over returns in MS Excel. For other confidence levels use the corresponding method. |
 | `cvar_down`             | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Downside 95% [Conditional Value At Risk](https://www.investopedia.com/terms/c/conditional_value_at_risk.asp), "CVaR". For other confidence levels use the corresponding method.                                         |
 | `worst`                 | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Most negative percentage change of a single observation.                                                                                                                                                                |
 | `worst_month`           | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Most negative month.                                                                                                                                                                                                    |
 | `max_drawdown`          | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Maximum drawdown](https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp).                                                                                                                                      |
 | `max_drawdown_cal_year` | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Max drawdown in a single calendar year.                                                                                                                                                                                 |
 | `positive_share`        | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | The share of percentage changes that are positive.                                                                                                                                                                      |
@@ -351,14 +352,15 @@
 | `arithmetic_ret_func`     | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Annualized arithmetic mean of returns](https://www.investopedia.com/terms/a/arithmeticmean.asp).                                                                                                                                                              |
 | `geo_ret_func`            | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Compound Annual Growth Rate(CAGR)](https://www.investopedia.com/terms/c/cagr.asp), a specific implementation of geometric mean.                                                                                                                               |
 | `value_ret_func`          | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Simple return from first to last observation.                                                                                                                                                                                                                  |
 | `vol_func`                | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Annualized [volatility](https://www.investopedia.com/terms/v/volatility.asp). Pandas .std() is the equivalent of stdev.s([...]) in MS excel.                                                                                                                   |
 | `downside_deviation_func` | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Downside deviation](https://www.investopedia.com/terms/d/downside-deviation.asp) is the volatility of all negative return observations. MAR and riskfree rate can be set.                                                                                     |
 | `ret_vol_ratio_func`      | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Ratio of arithmetic mean return and annualized volatility. It is the [Sharpe Ratio](https://www.investopedia.com/terms/s/sharperatio.asp) with the riskfree rate set to zero. A riskfree rate can be set as a float or a series chosen for the frame function. |
 | `sortino_ratio_func`      | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | The [Sortino Ratio](https://www.investopedia.com/terms/s/sortinoratio.asp) is the arithmetic mean return divided by the downside deviation. A riskfree rate can be set as a float or a series chosen for the frame function. MAR is set to zero.               |
+| `omega_ratio_func`        | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | The [Omega Ratio](https://en.wikipedia.org/wiki/Omega_ratio) compares returns above a certain target level (MAR) to the total downside risk below MAR.                                                                                                         |
 | `var_down_func`           | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Downside 95% [Value At Risk](https://www.investopedia.com/terms/v/var.asp), "VaR". The equivalent of percentile.inc([...], 1-level) over returns in MS Excel. Default is 95% confidence level.                                                                 |
 | `cvar_down_func`          | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Downside 95% [Conditional Value At Risk](https://www.investopedia.com/terms/c/conditional_value_at_risk.asp), "CVaR". Default is 95% confidence level.                                                                                                         |
 | `worst_func`              | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Most negative percentage change for a given number of observations (default=1).                                                                                                                                                                                |
 | `max_drawdown_func`       | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Maximum drawdown](https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp).                                                                                                                                                                             |
 | `positive_share_func`     | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | The share of percentage changes that are positive.                                                                                                                                                                                                             |
 | `vol_from_var_func`       | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | Implied annualized volatility from the Downside VaR using the assumption that returns are normally distributed.                                                                                                                                                |
 | `skew_func`               | `float`, `pandas.Series` | `OpenTimeSeries`, `OpenFrame` | [Skew](https://www.investopedia.com/terms/s/skewness.asp) of the return distribution.                                                                                                                                                                          |
```

