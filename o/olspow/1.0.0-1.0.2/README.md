# Comparing `tmp/olspow-1.0.0.tar.gz` & `tmp/olspow-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olspow-1.0.0.tar", last modified: Tue Feb 20 04:53:25 2024, max compression
+gzip compressed data, was "olspow-1.0.2.tar", last modified: Wed Apr 17 06:13:41 2024, max compression
```

## Comparing `olspow-1.0.0.tar` & `olspow-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-02-20 04:53:25.784798 olspow-1.0.0/
--rw-rw-r--   0 ben       (1000) ben       (1000)     1074 2024-01-21 01:57:57.000000 olspow-1.0.0/LICENSE
--rw-r--r--   0 ben       (1000) ben       (1000)     5513 2024-02-20 04:53:25.784798 olspow-1.0.0/PKG-INFO
--rw-rw-r--   0 ben       (1000) ben       (1000)     4858 2024-02-13 03:39:44.000000 olspow-1.0.0/README.md
--rw-rw-r--   0 ben       (1000) ben       (1000)      734 2024-02-19 21:15:22.000000 olspow-1.0.0/pyproject.toml
--rw-rw-r--   0 ben       (1000) ben       (1000)       38 2024-02-20 04:53:25.784798 olspow-1.0.0/setup.cfg
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-02-20 04:53:25.780798 olspow-1.0.0/src/
--rw-rw-r--   0 ben       (1000) ben       (1000)       76 2024-02-19 21:15:18.000000 olspow-1.0.0/src/__init__.py
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2024-02-20 04:53:25.784798 olspow-1.0.0/src/olspow.egg-info/
--rw-r--r--   0 ben       (1000) ben       (1000)     5513 2024-02-20 04:53:25.000000 olspow-1.0.0/src/olspow.egg-info/PKG-INFO
--rw-rw-r--   0 ben       (1000) ben       (1000)      231 2024-02-20 04:53:25.000000 olspow-1.0.0/src/olspow.egg-info/SOURCES.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)        1 2024-02-20 04:53:25.000000 olspow-1.0.0/src/olspow.egg-info/dependency_links.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       40 2024-02-20 04:53:25.000000 olspow-1.0.0/src/olspow.egg-info/requires.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       16 2024-02-20 04:53:25.000000 olspow-1.0.0/src/olspow.egg-info/top_level.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)    32427 2024-02-20 04:47:55.000000 olspow-1.0.0/src/olspow.py
+drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 06:13:41.787058 olspow-1.0.2/
+-rw-r--r--   0 benjaminknight   (502) staff       (20)     1074 2024-01-30 22:10:55.000000 olspow-1.0.2/LICENSE
+-rw-r--r--   0 benjaminknight   (502) staff       (20)     5513 2024-04-17 06:13:41.786636 olspow-1.0.2/PKG-INFO
+-rw-r--r--   0 benjaminknight   (502) staff       (20)     4858 2024-04-16 03:57:58.000000 olspow-1.0.2/README.md
+-rw-r--r--   0 benjaminknight   (502) staff       (20)      734 2024-04-16 04:05:15.000000 olspow-1.0.2/pyproject.toml
+-rw-r--r--   0 benjaminknight   (502) staff       (20)       38 2024-04-17 06:13:41.787144 olspow-1.0.2/setup.cfg
+drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 06:13:41.783994 olspow-1.0.2/src/
+-rw-r--r--   0 benjaminknight   (502) staff       (20)       76 2024-04-16 04:05:09.000000 olspow-1.0.2/src/__init__.py
+drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 06:13:41.786045 olspow-1.0.2/src/olspow.egg-info/
+-rw-r--r--   0 benjaminknight   (502) staff       (20)     5513 2024-04-17 06:13:41.000000 olspow-1.0.2/src/olspow.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminknight   (502) staff       (20)      231 2024-04-17 06:13:41.000000 olspow-1.0.2/src/olspow.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminknight   (502) staff       (20)        1 2024-04-17 06:13:41.000000 olspow-1.0.2/src/olspow.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminknight   (502) staff       (20)       40 2024-04-17 06:13:41.000000 olspow-1.0.2/src/olspow.egg-info/requires.txt
+-rw-r--r--   0 benjaminknight   (502) staff       (20)       16 2024-04-17 06:13:41.000000 olspow-1.0.2/src/olspow.egg-info/top_level.txt
+-rw-r--r--   0 benjaminknight   (502) staff       (20)    32802 2024-04-17 05:35:09.000000 olspow-1.0.2/src/olspow.py
```

### Comparing `olspow-1.0.0/LICENSE` & `olspow-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `olspow-1.0.0/PKG-INFO` & `olspow-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olspow
-Version: 1.0.0
+Version: 1.0.2
 Summary: Python package for conducting power analysis given ratio metrics, clustered data, and covariate adjustment.
 Author-email: "Benjamin S. Knight" <knight.benjamin@gmail.com>
 Project-URL: Homepage, https://github.com/b-knight/olspow
 Project-URL: Issues, https://github.com/b-knight/olspow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `olspow-1.0.0/README.md` & `olspow-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `olspow-1.0.0/pyproject.toml` & `olspow-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "olspow"
-version = "1.0.0"
+version = "1.0.2"
 authors = [
   { name="Benjamin S. Knight", email="knight.benjamin@gmail.com" },
 ]
 description = "Python package for conducting power analysis given ratio metrics, clustered data, and covariate adjustment."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `olspow-1.0.0/src/olspow.egg-info/PKG-INFO` & `olspow-1.0.2/src/olspow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olspow
-Version: 1.0.0
+Version: 1.0.2
 Summary: Python package for conducting power analysis given ratio metrics, clustered data, and covariate adjustment.
 Author-email: "Benjamin S. Knight" <knight.benjamin@gmail.com>
 Project-URL: Homepage, https://github.com/b-knight/olspow
 Project-URL: Issues, https://github.com/b-knight/olspow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `olspow-1.0.0/src/olspow.py` & `olspow-1.0.2/src/olspow.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,17 @@
                     "count",
                 )
             for predictor in exog:
                 agg_method[predictor] = "sum"
         data_agg_out = data.groupby(cluster).agg(agg_method)
         data_agg_out.rename(columns={cluster: "NOBS_IN_CLUSTER"}, inplace=True)
         if verbose:
-            print(f"{len(data_agg_out)} clusters were found in the data.")
+            print(
+                f"{humanize.intcomma(len(data_agg_out))} clusters were found in the data."
+            )
         return data_agg_out
 
     def _validate_sample_size(data, exog):
         """
         Validates the sample size post aggregation.
 
         Args:
@@ -393,23 +395,25 @@
         - float: The standard deviation of the double residuals.
         """
         n = len(working_df)
         dof = n - (len(exog) + 1)
         y_resid = _compute_residuals_of_response_var(is_ratio, working_df, endog, exog)
         w_resid = _compute_residuals_of_denominator(is_ratio, working_df, exog)
         theta, y_bar, w_bar = _compute_ratio_of_means(is_ratio, working_df, endog)
+        double_residuals = y_resid - theta * w_resid
         sample_std = np.sqrt(((y_resid - theta * w_resid) ** 2).sum() / dof)
         return (
             sample_std,
             dof,
             theta,
             y_bar,
             w_bar,
             y_resid,
             w_resid,
+            double_residuals,
         )
 
     def _fetch_z_statistic(input, alternative="one-sided"):
         """
         Fetches the z-statistic based on the input and alternative.
 
         Parameters:
@@ -613,14 +617,15 @@
         dof,
         assignment_ratio,
         theta,
         y_bar,
         w_bar,
         y_residuals,
         w_residuals,
+        double_residuals,
         hypothesis,
         nobs_pre_aggregation,
         nobs_post_aggregation,
         alpha_z=None,
         beta_z=None,
         mde_est=None,
         n_est=None,
@@ -662,14 +667,15 @@
             "Sample_Stdev": sample_stdev,
             "Degrees_of_Freedom": dof,
             "Theta": theta,
             "Numerator_Y_Bar": y_bar,
             "Denominator_W_Bar": w_bar,
             "Y_Bar_Residuals": y_residuals,
             "W_Bar_Residuals": w_residuals,
+            "Double_Residuals": double_residuals,
             "Estimated_MDE": mde_est,
             "Estimated_Required_Sample_Size": n_est,
             "Estimated_Power": power_est,
         }
         return diagnostics_dict
 
     _validate_number_of_inputs()
@@ -688,14 +694,15 @@
         stdev,
         degrees,
         theta_val,
         y_bar_val,
         w_bar_val,
         y_resid,
         w_resid,
+        double_residuals,
     ) = _compute_sample_stdev(is_ratio, working_df, endog, exog)
     mean_nobs_per_cluster = working_df["NOBS_IN_CLUSTER"].mean()
     if mde is None and n is not None and power is not None:
         mde, alpha_z_stat, beta_z_stat = _derive_mde(
             is_ratio_metric=is_ratio,
             sample_size=n,
             historical_stdev=stdev,
@@ -716,14 +723,15 @@
             dof=degrees,
             theta=theta_val,
             assignment_ratio=ratio,
             y_bar=y_bar_val,
             w_bar=w_bar_val,
             y_residuals=y_resid,
             w_residuals=w_resid,
+            double_residuals=double_residuals,
             hypothesis=alternative,
             nobs_pre_aggregation=nobs_pre_aggregation_val,
             nobs_post_aggregation=nobs_post_aggregation_val,
             alpha_z=alpha_z_stat,
             beta_z=beta_z_stat,
             mde_est=mde,
             n_est=n,
@@ -752,14 +760,15 @@
             dof=degrees,
             theta=theta_val,
             assignment_ratio=ratio,
             y_bar=y_bar_val,
             w_bar=w_bar_val,
             y_residuals=y_resid,
             w_residuals=w_resid,
+            double_residuals=double_residuals,
             hypothesis=alternative,
             nobs_pre_aggregation=nobs_pre_aggregation_val,
             nobs_post_aggregation=nobs_post_aggregation_val,
             alpha_z=alpha_z_stat,
             beta_z=beta_z_stat,
             mde_est=mde,
             n_est=n,
@@ -788,14 +797,15 @@
             dof=degrees,
             theta=theta_val,
             assignment_ratio=ratio,
             y_bar=y_bar_val,
             w_bar=w_bar_val,
             y_residuals=y_resid,
             w_residuals=w_resid,
+            double_residuals=double_residuals,
             hypothesis=alternative,
             nobs_pre_aggregation=nobs_pre_aggregation_val,
             nobs_post_aggregation=nobs_post_aggregation_val,
             alpha_z=alpha_z_stat,
             mde_est=mde,
             n_est=n,
             power_est=power,
```

