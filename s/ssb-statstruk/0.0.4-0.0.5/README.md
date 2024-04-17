# Comparing `tmp/ssb_statstruk-0.0.4.tar.gz` & `tmp/ssb_statstruk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_statstruk-0.0.4.tar", max compression
+gzip compressed data, was "ssb_statstruk-0.0.5.tar", max compression
```

## Comparing `ssb_statstruk-0.0.4.tar` & `ssb_statstruk-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2024-03-19 15:33:53.491309 ssb_statstruk-0.0.4/LICENSE
--rw-r--r--   0        0        0     3633 2024-03-19 15:33:53.491309 ssb_statstruk-0.0.4/README.md
--rw-r--r--   0        0        0     4216 2024-03-19 15:34:03.139183 ssb_statstruk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       86 2024-03-19 15:33:53.495308 ssb_statstruk-0.0.4/src/statstruk/__init__.py
--rw-r--r--   0        0        0      213 2024-03-19 15:33:53.495308 ssb_statstruk-0.0.4/src/statstruk/__main__.py
--rw-r--r--   0        0        0        0 2024-03-19 15:33:53.495308 ssb_statstruk-0.0.4/src/statstruk/py.typed
--rw-r--r--   0        0        0    31682 2024-03-19 15:34:03.139183 ssb_statstruk-0.0.4/src/statstruk/ratemodel.py
--rw-r--r--   0        0        0     4594 2024-03-19 15:34:03.139183 ssb_statstruk-0.0.4/src/statstruk/ssbmodel.py
--rw-r--r--   0        0        0     4693 1970-01-01 00:00:00.000000 ssb_statstruk-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-17 08:15:02.070561 ssb_statstruk-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3633 2024-04-17 08:15:02.070561 ssb_statstruk-0.0.5/README.md
+-rw-r--r--   0        0        0     4218 2024-04-17 08:15:14.810610 ssb_statstruk-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       86 2024-04-17 08:15:02.074561 ssb_statstruk-0.0.5/src/statstruk/__init__.py
+-rw-r--r--   0        0        0      213 2024-04-17 08:15:02.074561 ssb_statstruk-0.0.5/src/statstruk/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-17 08:15:02.074561 ssb_statstruk-0.0.5/src/statstruk/py.typed
+-rw-r--r--   0        0        0    32529 2024-04-17 08:15:02.074561 ssb_statstruk-0.0.5/src/statstruk/ratemodel.py
+-rw-r--r--   0        0        0     4899 2024-04-17 08:15:02.074561 ssb_statstruk-0.0.5/src/statstruk/ssbmodel.py
+-rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 ssb_statstruk-0.0.5/PKG-INFO
```

### Comparing `ssb_statstruk-0.0.4/LICENSE` & `ssb_statstruk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_statstruk-0.0.4/README.md` & `ssb_statstruk-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ssb_statstruk-0.0.4/pyproject.toml` & `ssb_statstruk-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "ssb-statstruk"
-version = "0.0.4"
+version = "0.0.5"
 description = "SSB Statstruk"
 authors = ["Susie Jentoft <coo@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/ssb-statstruk"
 repository = "https://github.com/statisticsnorway/ssb-statstruk"
 documentation = "https://statisticsnorway.github.io/ssb-statstruk"
 packages = [{ include = "statstruk", from = "src" }]
 classifiers = ["Development Status :: 4 - Beta"]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/statisticsnorway/ssb-statstruk/releases"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 click = ">=8.0.1"
 numpy = "^1.26.4"
 pandas = "^2.2.0"
 statsmodels = "^0.14.1"
 pandas-stubs = "^2.2.0.240218"
 
 [tool.poetry.group.dev.dependencies]
@@ -67,15 +67,15 @@
 show_column_numbers = true
 show_error_context = true
 
 [tool.ruff]
 force-exclude = true  # Apply excludes to pre-commit
 show-fixes = true
 src = ["src", "tests"]
-target-version = "py39"  # Minimum Python version supported
+target-version = "py310"  # Minimum Python version supported
 include = ["*.py", "*.pyi", "**/pyproject.toml", "*.ipynb"]
 extend-exclude = [
     "__pycache__",
     "old",
     "*/.ipynb_checkpoints/*",
     "noxfile.py",
     "docs/conf.py",
```

### Comparing `ssb_statstruk-0.0.4/src/statstruk/ratemodel.py` & `ssb_statstruk-0.0.5/src/statstruk/ratemodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,86 @@
 # # Code for rate estimation
 # #### To do:
 #
-# - Add in standard variance
+# - Fix for ulike strata i utvalg og pop
+# - Adjust rerunning for excludes to only rerun specific strata.
 # - Add in option for several y values.
-# - Write theory documentation with formulas in a markdown doc.
-# - Write help file/instructs documentation
 # - Homogen model option
 # - Regression model option
 
 # +
 
 
 # Import libraries
 from typing import Any
-from typing import Union
 
 import numpy as np
 import pandas as pd
 import statsmodels.formula.api as smf  # type: ignore
 
 from .ssbmodel import ssbmodel
 
 # -
 
 
 class ratemodel(ssbmodel):
     """Class for estimating statistics for business surveys using a rate model."""
 
     def __init__(
-        self, pop_data: pd.DataFrame, sample_data: pd.DataFrame, id_nr: str
+        self,
+        pop_data: pd.DataFrame,
+        sample_data: pd.DataFrame,
+        id_nr: str,
+        verbose: int = 1,
     ) -> None:
         """Initialization of ratemodel object."""
-        super().__init__(pop_data, sample_data, id_nr)
+        super().__init__(pop_data, sample_data, id_nr, verbose)
 
     def fit(
         self,
         y_var: str,
         x_var: str,
-        strata_var: Union[str, list[str]] = "",
+        strata_var: str | list[str] = "",
         control_extremes: bool = True,
-        exclude: Union[list[Union[str, int]], None] = None,
+        exclude: list[str | int] | None = None,
         exclude_auto: int = 0,
         remove_missing: bool = True,
         rbound: float = 2,
         gbound: float = 2,
+        count: int = 0,
     ) -> None:
         """Run and fit a rate model within strata.
 
         Args:
             y_var: The target variable to estimate from the survey.
             x_var: The variable to use as the explanatory variable in the model.
             strata_var: The stratification variable.
             control_extremes: Whether the model should be fitted in a way that allows for extremes value controls.
             exclude: List of ID numbers for observations to exclude.
             exclude_auto: Whether extreme values should be automatically excluded from the models. Default 0. Integer 1 indicates extreme values should be removed once and model run again.
             remove_missing: Whether to automatically remove units in the sample that are missing x or y values.
             rbound: Multiplicative value to determine the extremity of the studentized residual values.
             gbound: Multiplicative value to determine the extremity of the G values.
+            count: Integer value for the round count if using automatic exclusion of outliers.
 
         """
         # Check variables
         self._check_variable(x_var, self.pop_data, data_name="population")
         self._check_variable(x_var, self.sample_data, remove_missing=remove_missing)
         self._check_variable(y_var, self.sample_data, remove_missing=remove_missing)
 
+        # Bytte dtype hvis INt64 for x siden det fungere ikke med modellen - quick fix
+        # To DO: swap to funksjon
+        if self.pop_data[x_var].dtype == "Int64":
+            self.pop_data[x_var] = self.pop_data[x_var].astype("int64")
+        if self.sample_data[x_var].dtype == "Int64":
+            self.sample_data[x_var] = self.sample_data[x_var].astype("int64")
+        if self.sample_data[y_var].dtype == "Int64":
+            self.sample_data[y_var] = self.sample_data[y_var].astype("int64")
+
         # Check control and exclude_auto
         if (not control_extremes) & (exclude_auto > 0):
             print(
                 "You have chosen to automatically remove outliers so extreme values must be controlled. Parameter control_extremes set to True."
             )
             control_extremes = True
 
@@ -123,92 +136,48 @@
             all_values_present
         ), "Not all strata in the sample were found in the population data. Please check."
 
         # Create new strata variable for modelling in case there are excluded observations
         self.pop_data["_strata_var_mod"] = self.pop_data[strata_var_new]
         self.sample_data["_strata_var_mod"] = self.sample_data[strata_var_new]
 
-        # Add in change of strata for those excluded from model as: "surprise_strata"
-        def _update_strata(df: pd.DataFrame, exclude: list[Union[str, int]]) -> None:
-            """Update files to include a new variable for modelling including suprise strata."""
-            # Use the 'loc' method to locate the rows where ID is in the exclude list and update 'strata'
-            mask = df[self.id_nr].isin(exclude)
-            df.loc[mask, "_strata_var_mod"] = (
-                df.loc[mask, "_strata_var_mod"]
-                + "_surprise_"
-                + df.loc[mask, self.id_nr].astype(str)
-            )
-
+        # Check strata is same in sample and pop for excluded units and change if necessary
         if exclude is not None:
-            _update_strata(self.pop_data, exclude)
-            _update_strata(self.sample_data, exclude)
-
-        def _get_hat(X: Any, W: Any) -> Any:
-            """Get the hat matrix for the model."""
-            # Compute the square root of the weight matrix, W^(1/2)
-            W = np.diag(W)
-            W_sqrt = np.sqrt(W)
-
-            # Compute (X^T * W * X)^(-1)
-            XTWX_inv = np.linalg.inv(X.T @ W @ X)
-
-            # Compute the hat matrix
-            H = W_sqrt @ X @ XTWX_inv @ X.T @ W_sqrt
-
-            # Return diagonal
-            return np.diag(H)
-
-        def _get_rstud(
-            y: Any,
-            res: Any,
-            x_var: str,
-            df: pd.DataFrame,
-            hh: Any,
-            X: Any,
-            formula: str,
-        ) -> tuple[Any, Any]:
-            """Get the studentized residuals from the model."""
-            # set up vectors
-            n = len(y)
-            y = np.array(y)
-            X = np.array(X)
-            beta_ex_values = np.zeros(n)
-            R = np.zeros(n)
-
-            for i in range(n):
-                # Exclude the i-th observation
-                df_i = df.drop(index=df.iloc[i].name)
-                ww_i = 1.0 / (df_i[x_var])
-                ww_i.loc[df_i[x_var] == 0] = 1.0 / (df_i[x_var] + 1)
-                X_i = np.delete(X, i, axis=0)
-                y_i = np.delete(y, i, axis=0)
-
-                # Fit the WLS model without the i-th observation
-                model_i = smf.wls(formula, data=df_i, weights=ww_i).fit()
-                beta_ex_values[i] = model_i.params[x_var].item()
-
-                # get predicted values y_j
-                y_hat_j = model_i.predict(df_i)
-
-                # Calculate sigma
-                sigma2 = sum((y_i - y_hat_j) ** 2 / X_i) * 1.0 / (n - 2)
-
-                # Calculate and save studentized residuals
-                if (X[i] > 0) & (sigma2 > 0):
-                    R[i] = res[i] / (np.sqrt(sigma2 * X[i]) * np.sqrt(1.0 - hh[i]))
-                else:
-                    R[i] = np.nan
-
-            return (R, beta_ex_values)
+            sample_data_filtered = self.sample_data[
+                self.sample_data[self.id_nr].isin(exclude)
+            ]
+            pop_data_filtered = self.pop_data[self.pop_data[self.id_nr].isin(exclude)]
+            merged_df = pd.merge(
+                pop_data_filtered[[self.id_nr, "_strata_var_mod"]],
+                sample_data_filtered[[self.id_nr, "_strata_var_mod"]],
+                on=self.id_nr,
+                suffixes=("_pop", "_sample"),
+            )
+            update_needed = (
+                merged_df["_strata_var_mod_sample"] != merged_df["_strata_var_mod_pop"]
+            )
+            if update_needed.sum() > 0:
+                print(
+                    f"Stratum different in sample and population for excluded unit(s): {merged_df.loc[update_needed,self.id_nr].values}. The sample data strata will be used."
+                )
+                ids_to_update = merged_df.loc[update_needed, self.id_nr]
+                for i in ids_to_update:
+                    mask1 = self.pop_data[self.id_nr] == i
+                    mask2 = merged_df[self.id_nr] == i
+                    self.pop_data.loc[mask1, "_strata_var_mod"] = merged_df.loc[
+                        mask2, "_strata_var_mod_sample"
+                    ].values
+
+            # Next update for strata_var_mod to surprise strata
+            self.pop_data = self._update_strata(self.pop_data, exclude)
+            self.sample_data = self._update_strata(self.sample_data, exclude)
 
         # Set up coefficient dictionaries
         strata_results: dict["str", Any] = {}  # Each stratum as key
-        obs_data: dict["str", Any] = (
-            {}
-        )  # Each stratum as key - consider changing to virk id?
+        obs_data: dict["str", Any] = {}  # Each stratum as key
 
         # Iterate over each stratum in sample and fit model
         for stratum, group in self.sample_data.groupby("_strata_var_mod"):
             stratum_info: dict["str", Any] = {
                 "_strata_var_mod": stratum,
                 "n": len(group),  # Number of observations in the sample
                 "x_sum_sample": group[x_var].sum(),
@@ -238,15 +207,15 @@
                     {
                         "beta": model.params[x_var].item(),  # Series of coefficients
                         "sigma2": sigma2,
                     }
                 )
 
                 # Add in residuals and hat values to observation info
-                hats = _get_hat(group[[x_var]].values, weights)
+                hats = self._get_hat(group[[x_var]].values, weights)
                 obs_info.update({"resids": model.resid.values, "hat": hats})
 
                 # Check for x=0 and return message
                 if (any(group[x_var] == 0)) & (control_extremes):
                     print(
                         f"Values of zero detected in stratum {stratum!r}. These observations will not be assessed for extremeness."
                     )
@@ -269,15 +238,15 @@
                         print(
                             f"Extreme values not able to be detected in stratum: {stratum!r} due to too few observations."
                         )
                         obs_info.update(
                             {"rstud": np.nan, "G": np.nan, "beta_ex": np.nan}
                         )
                     else:
-                        rstuds = _get_rstud(
+                        rstuds = self._get_rstud(
                             y=np.array(group[y_var]),
                             res=model.resid.values,
                             x_var=x_var,
                             df=group,
                             hh=hats,
                             X=np.array(group[x_var]),
                             formula=formula,
@@ -296,42 +265,46 @@
                         f"Stratum: {stratum!r}, has only one observation and has 0 variance. Consider combing strata."
                     )
                 # Add standard info in for 1 obs strata : check for x-values = 0
                 x = group[x_var].values[0]
 
                 if x == 0:
                     print(
-                        f"Stratum {stratum!r}, has 1 observation and has a x-value of 0. This is causing a problem withestimates."
+                        f"Stratum {stratum!r}, has 1 observation and has a x-value of 0. This is causing a problem with estimates and has been adjusted to 0.01."
                     )
                     x = 0.01  ## Not quite right but quick fix for errors. Need to fix properly
                 stratum_info.update(
                     {
                         "beta": group[y_var].values[0] / x,
                         "sigma2": 0,
                     }
                 )
                 obs_info.update({"resids": [0], "hat": np.nan})
                 if control_extremes:
                     obs_info.update({"rstud": np.nan, "G": np.nan, "beta_ex": np.nan})
             strata_results[stratum] = stratum_info  # type: ignore
             obs_data[stratum] = obs_info  # type: ignore
 
+        if self.verbose == 2:
+            print("Finished fitting models. Now summarizing additional data")
+
         # Loop through population also
         for stratum, group in self.pop_data.groupby("_strata_var_mod"):
             stratum_info = {"N": len(group), "x_sum_pop": group[x_var].sum()}
             # Condition to see if strata exists. This is for cases where excludes observations are already excluded due to missing data
             if stratum in strata_results:
                 strata_results[stratum].update(stratum_info)  # type: ignore
 
         # Set results to instance
         self.strata_results = strata_results
         self.obs_data = obs_data
 
         # Check for outliers and re-run if auto exclude is on
         if exclude_auto > 0:
+            count = +1
             extremes = self.get_extremes(rbound=rbound, gbound=gbound)[
                 self.id_nr
             ].values.tolist()
             print(f"The following were extreme values and were excluded: {extremes!r}")
             if exclude is None:
                 exclude = extremes
             else:
@@ -344,16 +317,89 @@
                 strata_var=strata_var,
                 control_extremes=control_extremes,
                 exclude=exclude,
                 exclude_auto=exclude_auto,
                 remove_missing=remove_missing,
                 rbound=rbound,
                 gbound=gbound,
+                count=count,
             )
 
+    def _update_strata(
+        self, df: pd.DataFrame, exclude: list[str | int]
+    ) -> pd.DataFrame:
+        """Update files to include a new variable for modelling including suprise strata."""
+        # Use the 'loc' method to locate the rows where ID is in the exclude list and update 'strata'
+        mask = df[self.id_nr].isin(exclude)
+        df.loc[mask, "_strata_var_mod"] = (
+            df.loc[mask, "_strata_var_mod"]
+            + "_surprise_"
+            + df.loc[mask, self.id_nr].astype(str)
+        )
+        return df
+
+    def _get_hat(self, X: Any, W: Any) -> Any:
+        """Get the hat matrix for the model."""
+        # Compute the square root of the weight matrix, W^(1/2)
+        W = np.diag(W)
+        W_sqrt = np.sqrt(W)
+
+        # Compute (X^T * W * X)^(-1)
+        XTWX_inv = np.linalg.inv(X.T @ W @ X)
+
+        # Compute the hat matrix
+        H = W_sqrt @ X @ XTWX_inv @ X.T @ W_sqrt
+
+        # Return diagonal
+        return np.diag(H)
+
+    def _get_rstud(
+        self,
+        y: Any,
+        res: Any,
+        x_var: str,
+        df: pd.DataFrame,
+        hh: Any,
+        X: Any,
+        formula: str,
+    ) -> tuple[Any, Any]:
+        """Get the studentized residuals from the model."""
+        # set up vectors
+        n = len(y)
+        y = np.array(y)
+        X = np.array(X)
+        beta_ex_values = np.zeros(n)
+        R = np.zeros(n)
+
+        for i in range(n):
+            # Exclude the i-th observation
+            df_i = df.drop(index=df.iloc[i].name)
+            ww_i = 1.0 / (df_i[x_var])
+            ww_i.loc[df_i[x_var] == 0] = 1.0 / (df_i[x_var] + 1)
+            X_i = np.delete(X, i, axis=0)
+            y_i = np.delete(y, i, axis=0)
+
+            # Fit the WLS model without the i-th observation
+            model_i = smf.wls(formula, data=df_i, weights=ww_i).fit()
+            beta_ex_values[i] = model_i.params[x_var].item()
+
+            # get predicted values y_j
+            y_hat_j = model_i.predict(df_i)
+
+            # Calculate sigma
+            sigma2 = sum((y_i - y_hat_j) ** 2 / X_i) * 1.0 / (n - 2)
+
+            # Calculate and save studentized residuals
+            if (X[i] > 0) & (sigma2 > 0):
+                R[i] = res[i] / (np.sqrt(sigma2 * X[i]) * np.sqrt(1.0 - hh[i]))
+            else:
+                R[i] = np.nan
+
+        return (R, beta_ex_values)
+
     @property
     def get_coeffs(self) -> pd.DataFrame:
         """Get the model coefficients for each strata."""
         return pd.DataFrame(self.strata_results).T
 
     @property
     def get_obs(self) -> dict[str, Any]:
@@ -365,16 +411,16 @@
         # collect data for strata
         x_pop = self.strata_results[strata]["x_sum_pop"]
         x_utv = self.strata_results[strata]["x_sum_sample"]
 
         hi = self.obs_data[strata]["hat"]
         ei = self.obs_data[strata]["resids"]
 
-        if (isinstance(ei, (pd.Series, np.ndarray))) & (
-            isinstance(hi, (pd.Series, np.ndarray))
+        if (isinstance(ei, (pd.Series | np.ndarray))) & (
+            isinstance(hi, (pd.Series | np.ndarray))
         ):
             # Calculate ai
             Xr = x_pop - x_utv
             ai = Xr / x_utv
 
             # Calculate di variations
             di_1 = ei**2
@@ -489,21 +535,23 @@
         return domain_mapped.str[0]
 
     def get_estimates(
         self,
         domain: str = "",
         uncertainty_type: str = "CV",
         variance_type: str = "robust",
+        return_type: str = "unbiased",
     ) -> pd.DataFrame:
         """Get estimates for previously run model within strata or domains. Variance and CV estimates are returned for each domain.
 
         Args:
             domain: Name of the variable to use for estimation. Should be in the population data.
             uncertainty_type: Which uncertainty measures to return. Choose between 'CV' (default) for coefficient of variation, 'VAR' for variance, 'SE' for standard errors, 'CI' for confidence intervals. Multiple measures can be returned with combinations of these, for example "CV_SE" returns both the coefficient of variation and the standard error.
             variance_type: Choose from 'robust' or 'standard' estimation of variance. Currently only robust estimation is calculated for strata and aggregated strata domains estimation and standard for other domains.
+            return_type: String for which robust estimates to return. Choose 'unbiased' to return only the unbiased robust variance estimate or 'all' to return all three.
 
         Returns:
             A pd.Dataframe is returned conatining estimates and variance/coefficient of variation estimations for each domain.
 
         """
         # Check model is run
         self._check_model_run()
@@ -534,66 +582,55 @@
 
         # Add estimates
         strata_df["beta"] = pd.to_numeric(strata_df["beta"])
         strata_df[f"{self.y_var}_EST"] = pd.to_numeric(
             strata_df["beta"] * strata_df["x_sum_pop"]
         )
 
-        # Add variance
+        # Add variance standard or robust
         if variance_type == "standard":
             var1 = []
             for s in strata_df["_strata_var_mod"]:
                 var1.append(self._get_variance(s))
+
+            # Check for negative variances
+            if any(x < 0 for x in var1):
+                print("Negative variances calculated. These are being adjusted to 0.")
+                var1 = [i if i >= 0 else 0 for i in var1]
             strata_df[f"{self.y_var}_VAR"] = np.array(var1)
 
             # Aggregate to domain
             result = (
                 strata_df[[domain, "N", "n", f"{self.y_var}_EST", f"{self.y_var}_VAR"]]
                 .groupby(domain)
                 .sum()
             )
-
-            # Add in CV
-            if "CV" in uncertainty_type:
-                result[f"{self.y_var}_CV"] = (
-                    np.sqrt(result[f"{self.y_var}_VAR"])
-                    / result[f"{self.y_var}_EST"]
-                    * 100
-                )
-
-            # Add SE
-            if "SE" in uncertainty_type:
-                result[f"{self.y_var}_SE"] = np.sqrt(result[f"{self.y_var}_VAR"])
-
-            # Add in Confidence interval
-            if "CI" in uncertainty_type:
-                result[f"{self.y_var}_LB"] = result[f"{self.y_var}_EST"] - (
-                    1.96 * np.sqrt(result[f"{self.y_var}_VAR"])
-                )
-                result[f"{self.y_var}_UB"] = result[f"{self.y_var}_EST"] + (
-                    1.96 * np.sqrt(result[f"{self.y_var}_VAR"])
-                )
-
-            if "VAR" not in uncertainty_type:
-                result = result.drop([f"{self.y_var}_VAR"], axis=1)
-
         if variance_type == "robust":
             var1 = []
             var2 = []
             var3 = []
             for s in strata_df["_strata_var_mod"]:
                 var = self._get_robust(s)
                 if isinstance(var, tuple):
                     var1.append(var[0])
                     var2.append(var[1])
                     var3.append(var[2])
 
-            strata_df[f"{self.y_var}_VAR1"] = np.array(var1)
-            strata_df[f"{self.y_var}_VAR2"] = np.array(var2)
-            strata_df[f"{self.y_var}_VAR3"] = np.array(var3)
+            # Adjust negative variance to zero
+            if any(x < 0 for x in var1 + var2 + var3):
+                print("Negative variances calculated. These are being adjusted to 0.")
+            strata_df[f"{self.y_var}_VAR1"] = np.array(
+                [i if i >= 0 else 0 for i in var1]
+            )
+            strata_df[f"{self.y_var}_VAR2"] = np.array(
+                [i if i >= 0 else 0 for i in var2]
+            )
+            strata_df[f"{self.y_var}_VAR3"] = np.array(
+                [i if i >= 0 else 0 for i in var3]
+            )
 
             # Aggregate to domain
             result = (
                 strata_df[
                     [
                         domain,
                         "N",
@@ -604,64 +641,44 @@
                         f"{self.y_var}_VAR3",
                     ]
                 ]
                 .groupby(domain)
                 .sum()
             )
 
-            # Add in CV
+        # Format and add in CV, SE, CI
+        if variance_type == "standard":
+            variance_list = [""]
+        if (variance_type == "robust") & (return_type == "unbiased"):
+            variance_list = ["2"]
+        if (variance_type == "robust") & (return_type == "all"):
+            variance_list = ["1", "2", "3"]
+
+        for i in variance_list:
+
             if "CV" in uncertainty_type:
-                result[f"{self.y_var}_CV1"] = (
-                    np.sqrt(result[f"{self.y_var}_VAR1"])
-                    / result[f"{self.y_var}_EST"]
-                    * 100
-                )
-                result[f"{self.y_var}_CV2"] = (
-                    np.sqrt(result[f"{self.y_var}_VAR2"])
-                    / result[f"{self.y_var}_EST"]
-                    * 100
-                )
-                result[f"{self.y_var}_CV3"] = (
-                    np.sqrt(result[f"{self.y_var}_VAR3"])
+                result[f"{self.y_var}_CV{i}"] = (
+                    np.sqrt(result[f"{self.y_var}_VAR{i}"])
                     / result[f"{self.y_var}_EST"]
                     * 100
                 )
 
-            # Add SE
             if "SE" in uncertainty_type:
-                result[f"{self.y_var}_SE1"] = np.sqrt(result[f"{self.y_var}_VAR1"])
-                result[f"{self.y_var}_SE2"] = np.sqrt(result[f"{self.y_var}_VAR2"])
-                result[f"{self.y_var}_SE3"] = np.sqrt(result[f"{self.y_var}_VAR3"])
+                result[f"{self.y_var}_SE{i}"] = np.sqrt(result[f"{self.y_var}_VAR{i}"])
 
-            # Add in Confidence interval
             if "CI" in uncertainty_type:
-                result[f"{self.y_var}_LB1"] = result[f"{self.y_var}_EST"] - (
-                    1.96 * np.sqrt(result[f"{self.y_var}_VAR1"])
-                )
-                result[f"{self.y_var}_UB1"] = result[f"{self.y_var}_EST"] + (
-                    1.96 * np.sqrt(result[f"{self.y_var}_VAR1"])
-                )
-                result[f"{self.y_var}_LB2"] = result[f"{self.y_var}_EST"] - (
-                    1.96 * np.sqrt(result[f"{self.y_var}_VAR2"])
+                result[f"{self.y_var}_LB{i}"] = result[f"{self.y_var}_EST"] - (
+                    1.96 * np.sqrt(result[f"{self.y_var}_VAR{i}"])
                 )
-                result[f"{self.y_var}_UB2"] = result[f"{self.y_var}_EST"] + (
-                    1.96 * np.sqrt(result[f"{self.y_var}_VAR2"])
-                )
-                result[f"{self.y_var}_LB3"] = result[f"{self.y_var}_EST"] - (
-                    1.96 * np.sqrt(result[f"{self.y_var}_VAR3"])
-                )
-                result[f"{self.y_var}_UB3"] = result[f"{self.y_var}_EST"] + (
-                    1.96 * np.sqrt(result[f"{self.y_var}_VAR3"])
+                result[f"{self.y_var}_UB{i}"] = result[f"{self.y_var}_EST"] + (
+                    1.96 * np.sqrt(result[f"{self.y_var}_VAR{i}"])
                 )
 
             if "VAR" not in uncertainty_type:
-                result = result.drop(
-                    [f"{self.y_var}_VAR1", f"{self.y_var}_VAR2", f"{self.y_var}_VAR3"],
-                    axis=1,
-                )
+                result = result.drop([f"{self.y_var}_VAR{i}"], axis=1)
 
         return result
 
     def get_extremes(
         self, threshold_type: str = "both", rbound: float = 2, gbound: float = 2
     ) -> pd.DataFrame:
         """Get observations with extreme values based on their rstudized residual value or G value.
```

### Comparing `ssb_statstruk-0.0.4/src/statstruk/ssbmodel.py` & `ssb_statstruk-0.0.5/src/statstruk/ssbmodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,7 +110,13 @@
             lambda x: 1 if x in sample_ids else 0
         )
 
     def _check_model_run(self) -> None:
         """Check to ensure that model has been run before proceeding with other functions."""
         if not hasattr(self, "strata_results"):
             raise RuntimeError("Model has not been run. Please run fit() first")
+
+    def _convert_var(self, var_name: str, dataset: pd.DataFrame) -> None:
+        if dataset[var_name].dtype == "Int64":
+            dataset[var_name] = dataset[var_name].astype("int64")
+        if dataset[var_name].dtype == "Float64":
+            dataset[var_name] = dataset[var_name].astype("float64")
```

### Comparing `ssb_statstruk-0.0.4/PKG-INFO` & `ssb_statstruk-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: ssb-statstruk
-Version: 0.0.4
+Version: 0.0.5
 Summary: SSB Statstruk
 Home-page: https://github.com/statisticsnorway/ssb-statstruk
 License: MIT
 Author: Susie Jentoft
 Author-email: coo@ssb.no
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.0.1)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pandas-stubs (>=2.2.0.240218,<3.0.0.0)
```

