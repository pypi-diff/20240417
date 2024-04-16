# Comparing `tmp/keypoint-moseq-0.4.5.tar.gz` & `tmp/keypoint-moseq-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypoint-moseq-0.4.5.tar", last modified: Wed Feb 28 15:12:13 2024, max compression
+gzip compressed data, was "keypoint-moseq-0.4.6.tar", last modified: Tue Apr 16 22:08:31 2024, max compression
```

## Comparing `keypoint-moseq-0.4.5.tar` & `keypoint-moseq-0.4.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-02-28 15:12:13.274155 keypoint-moseq-0.4.5/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8091 2023-12-12 01:46:33.000000 keypoint-moseq-0.4.5/LICENSE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.4.5/NOTICE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2024-02-28 15:12:13.274293 keypoint-moseq-0.4.5/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1435 2023-11-06 19:39:05.000000 keypoint-moseq-0.4.5/README.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-02-28 15:12:13.275667 keypoint-moseq-0.4.5/keypoint_moseq/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      525 2024-02-23 04:35:35.000000 keypoint-moseq-0.4.5/keypoint_moseq/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2024-02-28 15:12:13.275795 keypoint-moseq-0.4.5/keypoint_moseq/_version.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    54089 2023-12-29 03:01:06.000000 keypoint-moseq-0.4.5/keypoint_moseq/analysis.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17753 2024-01-17 19:32:27.000000 keypoint-moseq-0.4.5/keypoint_moseq/calibration.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    22688 2023-12-15 15:22:11.000000 keypoint-moseq-0.4.5/keypoint_moseq/fitting.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    49181 2024-02-28 15:12:08.000000 keypoint-moseq-0.4.5/keypoint_moseq/io.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    12124 2024-02-19 06:20:32.000000 keypoint-moseq-0.4.5/keypoint_moseq/tools.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    39241 2023-11-07 19:17:29.000000 keypoint-moseq-0.4.5/keypoint_moseq/util.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    88677 2024-02-04 01:38:35.000000 keypoint-moseq-0.4.5/keypoint_moseq/viz.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-02-28 15:12:13.273842 keypoint-moseq-0.4.5/keypoint_moseq.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2024-02-28 15:12:13.000000 keypoint-moseq-0.4.5/keypoint_moseq.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)      479 2024-02-28 15:12:13.000000 keypoint-moseq-0.4.5/keypoint_moseq.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2024-02-28 15:12:13.000000 keypoint-moseq-0.4.5/keypoint_moseq.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      247 2024-02-28 15:12:13.000000 keypoint-moseq-0.4.5/keypoint_moseq.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2024-02-28 15:12:13.000000 keypoint-moseq-0.4.5/keypoint_moseq.egg-info/top_level.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      836 2024-02-28 15:12:13.275263 keypoint-moseq-0.4.5/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      247 2023-08-21 15:48:12.000000 keypoint-moseq-0.4.5/setup.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    84134 2023-08-21 15:48:12.000000 keypoint-moseq-0.4.5/versioneer.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-16 22:08:31.665519 keypoint-moseq-0.4.6/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8091 2023-12-12 01:46:33.000000 keypoint-moseq-0.4.6/LICENSE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.4.6/NOTICE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2024-04-16 22:08:31.665660 keypoint-moseq-0.4.6/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1435 2023-11-06 19:39:05.000000 keypoint-moseq-0.4.6/README.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-16 22:08:31.666631 keypoint-moseq-0.4.6/keypoint_moseq/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      525 2024-02-23 04:35:35.000000 keypoint-moseq-0.4.6/keypoint_moseq/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2024-04-16 22:08:31.666744 keypoint-moseq-0.4.6/keypoint_moseq/_version.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    55645 2024-04-16 22:08:28.000000 keypoint-moseq-0.4.6/keypoint_moseq/analysis.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    18130 2024-04-15 22:09:44.000000 keypoint-moseq-0.4.6/keypoint_moseq/calibration.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    22692 2024-04-16 22:08:28.000000 keypoint-moseq-0.4.6/keypoint_moseq/fitting.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    49181 2024-04-04 18:16:19.000000 keypoint-moseq-0.4.6/keypoint_moseq/io.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    12124 2024-02-19 06:20:32.000000 keypoint-moseq-0.4.6/keypoint_moseq/tools.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    40685 2024-04-16 22:08:28.000000 keypoint-moseq-0.4.6/keypoint_moseq/util.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    89506 2024-04-16 22:08:28.000000 keypoint-moseq-0.4.6/keypoint_moseq/viz.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-16 22:08:31.665139 keypoint-moseq-0.4.6/keypoint_moseq.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2024-04-16 22:08:31.000000 keypoint-moseq-0.4.6/keypoint_moseq.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      479 2024-04-16 22:08:31.000000 keypoint-moseq-0.4.6/keypoint_moseq.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2024-04-16 22:08:31.000000 keypoint-moseq-0.4.6/keypoint_moseq.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      247 2024-04-16 22:08:31.000000 keypoint-moseq-0.4.6/keypoint_moseq.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2024-04-16 22:08:31.000000 keypoint-moseq-0.4.6/keypoint_moseq.egg-info/top_level.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      836 2024-04-16 22:08:31.666337 keypoint-moseq-0.4.6/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      247 2023-08-21 15:48:12.000000 keypoint-moseq-0.4.6/setup.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    84134 2023-08-21 15:48:12.000000 keypoint-moseq-0.4.6/versioneer.py
```

### Comparing `keypoint-moseq-0.4.5/LICENSE.md` & `keypoint-moseq-0.4.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.4.5/NOTICE.md` & `keypoint-moseq-0.4.6/NOTICE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.4.5/README.md` & `keypoint-moseq-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.4.5/keypoint_moseq/__init__.py` & `keypoint-moseq-0.4.6/keypoint_moseq/__init__.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.4.5/keypoint_moseq/analysis.py` & `keypoint-moseq-0.4.6/keypoint_moseq/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,19 +40,19 @@
         list of syllable names
     """
     labels = {ix: f"{ix}" for ix in syllable_ixs}
     syll_info_path = os.path.join(project_dir, model_name, "syll_info.csv")
     if os.path.exists(syll_info_path):
         syll_info_df = pd.read_csv(syll_info_path, index_col=False).fillna("")
 
-    for ix in syllable_ixs:
-        if len(syll_info_df[syll_info_df.syllable == ix].label.values[0]) > 0:
-            labels[
-                ix
-            ] = f"{ix} ({syll_info_df[syll_info_df.syllable == ix].label.values[0]})"
+        for ix in syllable_ixs:
+            if len(syll_info_df[syll_info_df.syllable == ix].label.values[0]) > 0:
+                labels[ix] = (
+                    f"{ix} ({syll_info_df[syll_info_df.syllable == ix].label.values[0]})"
+                )
     names = [labels[ix] for ix in syllable_ixs]
     return names
 
 
 def generate_index(project_dir, model_name, index_filepath):
     """Generate index file as a csv.
 
@@ -822,15 +822,14 @@
     num_groups = len(group_names)
 
     # get all syllable usage data
     df_only_stats = grouped_data.drop(["group", "name"], axis=1)
     syllable_data = grouped_data.drop(["group", "name"], axis=1).values
 
     N_m, N_s = syllable_data.shape
-
     # Run KW and return H-stats
     h_all, real_ranks, X_ties = run_manual_KW_test(
         df_usage=df_only_stats,
         merged_usages_all=syllable_data,
         num_groups=num_groups,
         n_per_group=n_per_group,
         cum_group_idx=cum_group_idx,
@@ -876,15 +875,18 @@
         thresh,
         mc_method,
     )
 
     # combine Dunn's test results into single DataFrame
     df_z = pd.DataFrame(real_zs_within_group)
     df_z.index = df_z.index.set_names("syllable")
-    dunn_results_df = df_z.reset_index().melt(id_vars="syllable")
+    dunn_results_df = df_z.reset_index().melt(id_vars=[("syllable", "")])
+    dunn_results_df.rename(
+        columns={"variable_0": "group1", "variable_1": "group2"}, inplace=True
+    )
 
     # Get intersecting significant syllables between
     intersect_sig_syllables = {}
     for pair in df_pair_corrected_pvalues.columns.tolist():
         intersect_sig_syllables[pair] = np.where(
             (df_pair_corrected_pvalues[pair] < thresh) & (df_k_real.is_sig)
         )[0]
@@ -1032,15 +1034,15 @@
             complete_df, ctrl_group, exp_group, stat=stat
         )
     if colors is None:
         colors = []
     if len(colors) == 0 or len(colors) != len(groups):
         colors = sns.color_palette(n_colors=len(groups))
 
-    return ordering, groups, colors, figsize
+    return np.array(ordering), groups, colors, figsize
 
 
 def save_analysis_figure(fig, plot_name, project_dir, model_name, save_dir):
     """Save an analysis figure.
 
     The figure is saved as both a .png and .pdf, either to `save_dir` if it is
     provided, or else to `project_dir/model_name/figures`.
@@ -1084,15 +1086,15 @@
         the path to save the analysis plots
     plot_sig : bool, optional
         whether to plot the significant syllables, by default True
     thresh : float, optional
         the threshold for significance, by default 0.05
     stat : str, optional
         the statistic to plot, by default 'frequency'
-    ordering : str, optional
+    order : str, optional
         the ordering of the syllables, by default 'stat'
     groups : list, optional
         the list of groups to plot, by default None
     ctrl_group : str, optional
         the control group, by default None
     exp_group : str, optional
         the experimental group, by default None
@@ -1109,30 +1111,31 @@
         the figure object
     legend : matplotlib.legend.Legend
         the legend object
     """
 
     # get significant syllables
     sig_sylls = None
+    if groups is None:
+        groups = stats_df["group"].unique()
 
     if plot_sig and len(stats_df["group"].unique()) > 1:
         # run kruskal wallis and dunn's test
         _, _, sig_pairs = run_kruskal(stats_df, statistic=stat, thresh=thresh)
-        # plot significant syllables for control and experimental group
-        if ctrl_group is not None and exp_group is not None:
+        # plot significant syllables for control and experimental group when user specify something
+        if ctrl_group in groups and exp_group in groups:
             # check if the group pair is in the sig pairs dict
             if (ctrl_group, exp_group) in sig_pairs.keys():
                 sig_sylls = sig_pairs.get((ctrl_group, exp_group))
             # flip the order of the groups
             else:
                 sig_sylls = sig_pairs.get((exp_group, ctrl_group))
         else:
-            print(
-                "No control or experimental group specified. Not plotting significant syllables."
-            )
+            # plot everything if no group pair is specified
+            sig_sylls = sig_pairs
 
     xlabel = f"Syllables sorted by {stat}"
     if order == "diff":
         xlabel += " difference"
     ordering, groups, colors, figsize = _validate_and_order_syll_stats_params(
         stats_df,
         stat=stat,
@@ -1165,18 +1168,46 @@
 
     # add syllable labels if they exist
     syll_names = get_syllable_names(project_dir, model_name, ordering)
     plt.xticks(range(len(syll_names)), syll_names, rotation=90)
 
     # if a list of significant syllables is given, mark the syllables above the x-axis
     if sig_sylls is not None:
-        markings = []
-        for s in sig_sylls:
-            markings.append(ordering.index(s))
-        plt.scatter(markings, [-0.005] * len(markings), color="r", marker="*")
+        init_y = -0.05
+        # plot all sig syllables when no reasonable control and experimental group is specified
+        if isinstance(sig_sylls, dict):
+            for key in sig_sylls.keys():
+                markings = []
+                for s in sig_sylls[key]:
+                    markings.append(np.where(ordering == s)[0])
+                if len(markings) > 0:
+                    markings = np.concatenate(markings)
+                    plt.scatter(
+                        markings, [init_y] * len(markings), color="r", marker="*"
+                    )
+                    plt.text(
+                        plt.xlim()[1],
+                        init_y,
+                        f"{key[0]} vs. {key[1]} - Total {len(sig_sylls[key])} S.S.",
+                    )
+                    init_y += -0.05
+                else:
+                    print("No significant syllables found.")
+        else:
+            markings = []
+            for s in sig_sylls:
+                if s in ordering:
+                    markings.append(np.where(ordering == s)[0])
+                else:
+                    continue
+            if len(markings) > 0:
+                markings = np.concatenate(markings)
+                plt.scatter(markings, [-0.05] * len(markings), color="r", marker="*")
+            else:
+                print("No significant syllables found.")
 
         # manually define a new patch
         patch = Line2D(
             [],
             [],
             color="red",
             marker="*",
@@ -1412,18 +1443,23 @@
         the method to normalize the transition matrix, by default 'bigram'
     figsize : tuple, optional
         the figure size, by default (12,6)
     show_syllable_names : bool, optional
         whether to show just syllable indexes (False) or syllable indexes and
         names (True)
     """
+
+    # syllable info path
+    syll_info_path = os.path.join(project_dir, model_name, "syll_info.csv")
+    # initialize syllable names
+    syll_names = [f"{ix}" for ix in syll_include]
+
     if show_syllable_names:
-        syll_names = get_syllable_names(project_dir, model_name, syll_include)
-    else:
-        syll_names = [f"{ix}" for ix in syll_include]
+        if os.path.exists(syll_info_path):
+            syll_names = get_syllable_names(project_dir, model_name, syll_include)
 
     # infer max_syllables
     max_syllables = trans_mats[0].shape[0]
 
     fig, ax = plt.subplots(1, len(group), figsize=figsize, sharex=False, sharey=True)
     title_map = dict(bigram="Bigram", columns="Incoming", rows="Outgoing")
     color_lim = max([x.max() for x in trans_mats])
```

### Comparing `keypoint-moseq-0.4.5/keypoint_moseq/calibration.py` & `keypoint-moseq-0.4.6/keypoint_moseq/calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,29 +65,35 @@
             for i in np.random.choice(len(samples_in_bin), n, replace=False):
                 sample_keys.append(samples_in_bin[i])
 
     sample_keys = [sample_keys[i] for i in np.random.permutation(len(sample_keys))]
     return sample_keys
 
 
-def load_sampled_frames(sample_keys, video_dir, video_extension=None):
+def load_sampled_frames(
+    sample_keys, video_dir, video_extension=None, downsample_rate=1
+):
     """Load sampled frames from a directory of videos.
 
     Parameters
     ----------
     sample_keys: list of tuples
         List of sampled frames as tuples with format
         (key, frame_number, bodypart)
 
     video_dir: str
         Path to directory containing videos
 
     video_extension: str, default=None
         Preferred video extension (passed to :py:func:`keypoint_moseq.util.find_matching_videos`)
 
+    downsample_rate: int, default=1
+        Downsampling rate for the video frames. Only change if keypoint detections were
+        also downsampled.
+
     Returns
     -------
     sample_keys: dict
         Dictionary mapping elements from `sample_keys` to the
         corresponding videos frames.
     """
     keys = sorted(set([k[0] for k in sample_keys]))
@@ -98,15 +104,16 @@
         sample_keys,
         desc="Loading sample frames",
         position=0,
         leave=True,
         ncols=72,
     )
     return {
-        (key, frame, bodypart): readers[key][frame] for key, frame, bodypart in pbar
+        (key, frame, bodypart): readers[key][frame * downsample_rate]
+        for key, frame, bodypart in pbar
     }
 
 
 def load_annotations(project_dir):
     """Reload saved calibration annotations.
 
     Parameters
@@ -441,14 +448,15 @@
     confidences,
     *,
     bodyparts,
     use_bodyparts,
     video_dir,
     video_extension=None,
     conf_pseudocount=0.001,
+    downsample_rate=1,
     **kwargs,
 ):
     """Perform manual annotation to calibrate the relationship between keypoint
     error and neural network confidence.
 
     This function creates a widget for interactive annotation in jupyter lab.
     Users mark correct keypoint locations for a sequence of frames, and a
@@ -499,26 +507,30 @@
         contain the videoname as a prefix.
 
     video_extension: str, default=None
         Preferred video extension (used in :py:func:`keypoint_moseq.util.find_matching_videos`)
 
     conf_pseudocount: float, default=0.001
         Pseudocount added to confidence values to avoid log(0) errors.
+
+    downsample_rate: int, default=1
+        Downsampling rate for the video frames. Only change if keypoint detections were
+        also downsampled.
     """
     dim = list(coordinates.values())[0].shape[-1]
     assert dim == 2, "Calibration is only supported for 2D keypoints."
 
     confidences = {k: v + conf_pseudocount for k, v in confidences.items()}
     sample_keys = sample_error_frames(confidences, bodyparts, use_bodyparts)
 
     annotations = load_annotations(project_dir)
     sample_keys.extend(annotations.keys())
 
     sample_images = load_sampled_frames(
-        sample_keys, video_dir, video_extension=video_extension
+        sample_keys, video_dir, video_extension, downsample_rate
     )
 
     return _noise_calibration_widget(
         project_dir,
         coordinates,
         confidences,
         sample_keys,
```

### Comparing `keypoint-moseq-0.4.5/keypoint_moseq/fitting.py` & `keypoint-moseq-0.4.6/keypoint_moseq/fitting.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,15 +284,15 @@
 
 def apply_model(
     model,
     data,
     metadata,
     project_dir=None,
     model_name=None,
-    num_iters=50,
+    num_iters=500,
     ar_only=False,
     save_results=True,
     verbose=False,
     results_path=None,
     parallel_message_passing=None,
     return_model=False,
     location_aware=False,
@@ -317,15 +317,15 @@
         Path to the project directory. Required if `save_results=True` and
         `results_path=None`.
 
     model_name : str, default=None
         Name of the model. Required if `save_results=True` and
         `results_path=None`.
 
-    num_iters : int, default=50
+    num_iters : int, default=500
         Number of iterations to run the model.
 
     ar_only : bool, default=False
         See :py:func:`keypoint_moseq.fitting.fit_model`.
 
     save_results : bool, default=True
         If True, the model outputs will be saved to disk (see
@@ -412,15 +412,15 @@
         return results
 
 
 def estimate_syllable_marginals(
     model,
     data,
     metadata,
-    burn_in_iters=50,
+    burn_in_iters=200,
     num_samples=100,
     steps_per_sample=10,
     return_samples=False,
     verbose=False,
     parallel_message_passing=None,
     location_aware=False,
     **kwargs,
@@ -436,15 +436,15 @@
     data: dict
         Data for model fitting (see :py:func:`keypoint_moseq.io.format_data`).
 
     metadata: tuple (keys, bounds)
         Recordings and start/end frames for the data (see
         :py:func:`keypoint_moseq.io.format_data`).
 
-    burn_in_iters : int, default=50
+    burn_in_iters : int, default=200
         Number of resampling iterations to run before collecting samples.
 
     num_samples : int, default=100
         Number of samples to collect for marginalization.
 
     steps_per_sample : int, default=10
         Number of resampling iterations to run between collecting samples.
```

### Comparing `keypoint-moseq-0.4.5/keypoint_moseq/io.py` & `keypoint-moseq-0.4.6/keypoint_moseq/io.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.4.5/keypoint_moseq/tools.py` & `keypoint-moseq-0.4.6/keypoint_moseq/tools.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.4.5/keypoint_moseq/util.py` & `keypoint-moseq-0.4.6/keypoint_moseq/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import jax, jax.numpy as jnp
 from scipy.ndimage import median_filter, convolve1d, gaussian_filter1d
 from sklearn.decomposition import PCA
 from sklearn.neighbors import NearestNeighbors
 from scipy.spatial.distance import pdist, squareform
 from jax_moseq.models.keypoint_slds import inverse_rigid_transform
 from jax_moseq.utils import get_frequencies, batch
+from vidio.read import OpenCVReader
 
 na = jnp.newaxis
 
 
 def np_io(fn):
     """Converts a function involving jax arrays to one that inputs and outputs
     numpy arrays."""
@@ -32,17 +33,15 @@
     Parameters
     ----------
     pca: sklearn.decomposition._pca.PCA, A fit PCA model
     f: float, Target variance fraction
     """
     cs = np.cumsum(pca.explained_variance_ratio_)
     if cs[-1] < f:
-        print(
-            f"All components together only explain {cs[-1]*100}% of variance."
-        )
+        print(f"All components together only explain {cs[-1]*100}% of variance.")
     else:
         print(
             f">={f*100}% of variance exlained by {(cs>f).nonzero()[0].min()+1} components."
         )
 
 
 def list_files_with_exts(filepath_pattern, ext_list, recursive=True):
@@ -84,17 +83,15 @@
         matches = glob.glob(filepath_pattern)
         if recursive:
             for match in list(matches):
                 matches += glob.glob(os.path.join(match, "**"), recursive=True)
 
         # filter matches by extension
         matches = [
-            match
-            for match in matches
-            if os.path.splitext(match)[1].lower() in ext_list
+            match for match in matches if os.path.splitext(match)[1].lower() in ext_list
         ]
         return matches
 
 
 def find_matching_videos(
     keys,
     video_dir,
@@ -157,17 +154,15 @@
         extensions = [".mp4", ".avi", ".mov"]
     else:
         if video_extension[0] != ".":
             video_extension = "." + video_extension
         extensions = [video_extension]
 
     videos = list_files_with_exts(video_dir, extensions, recursive=recursive)
-    videos_to_paths = {
-        os.path.splitext(os.path.basename(f))[0]: f for f in videos
-    }
+    videos_to_paths = {os.path.splitext(os.path.basename(f))[0]: f for f in videos}
 
     video_paths = []
     for key in keys:
         matches = [
             v
             for v in videos_to_paths
             if os.path.basename(key).startswith(v + recording_name_suffix)
@@ -272,17 +267,15 @@
         of shape (n_frames, [2 or 3]).
 
     headings: dict
         Dictionary mapping recording names to heading angles (in radians) as 1d
         arrays of shape (n_frames,).
     """
     if bodyparts is not None and use_bodyparts is not None:
-        coordinates = reindex_by_bodyparts(
-            coordinates, bodyparts, use_bodyparts
-        )
+        coordinates = reindex_by_bodyparts(coordinates, bodyparts, use_bodyparts)
 
     centroids, headings = {}, {}
     for key, coords in coordinates.items():
         coords = interpolate_keypoints(coords, np.isnan(coords).any(-1))
         centroids[key] = np.median(coords, axis=1)
         anterior_loc = coords[:, posterior_idxs].mean(1)
         posterior_loc = coords[:, anterior_idxs].mean(1)
@@ -309,20 +302,16 @@
         Kernel size for median filtering
 
     Returns
     -------
     filtered_centroids: dict
     filtered_headings: dict
     """
-    centroids = {
-        k: median_filter(v, (filter_size, 1)) for k, v in centroids.items()
-    }
-    headings = {
-        k: filter_angle(v, size=filter_size) for k, v in headings.items()
-    }
+    centroids = {k: median_filter(v, (filter_size, 1)) for k, v in centroids.items()}
+    headings = {k: filter_angle(v, size=filter_size) for k, v in headings.items()}
     return centroids, headings
 
 
 def get_syllable_instances(
     stateseqs,
     min_duration=3,
     pre=30,
@@ -374,23 +363,17 @@
         starts = np.insert(transitions, 0, 0)
         ends = np.append(transitions, len(stateseq))
         for s, e, syllable in zip(starts, ends, stateseq[starts]):
             if e - s >= min_duration and s >= pre and s < len(stateseq) - post:
                 syllable_instances[syllable].append((key, s, e))
 
     frequencies_filter = get_frequencies(stateseqs) >= min_frequency
-    counts_filter = (
-        np.array(list(map(len, syllable_instances))) >= min_instances
-    )
-    use_syllables = np.all(
-        [frequencies_filter, counts_filter], axis=0
-    ).nonzero()[0]
-    return {
-        syllable: syllable_instances[syllable] for syllable in use_syllables
-    }
+    counts_filter = np.array(list(map(len, syllable_instances))) >= min_instances
+    use_syllables = np.all([frequencies_filter, counts_filter], axis=0).nonzero()[0]
+    return {syllable: syllable_instances[syllable] for syllable in use_syllables}
 
 
 def get_edges(use_bodyparts, skeleton):
     """Represent the skeleton as a list of index-pairs.
 
     Parameters
     -------
@@ -413,17 +396,15 @@
             assert use_bodyparts is not None, fill(
                 "If skeleton edges are specified using bodypart names, "
                 "`use_bodyparts` must be specified"
             )
 
             for bp1, bp2 in skeleton:
                 if bp1 in use_bodyparts and bp2 in use_bodyparts:
-                    edges.append(
-                        [use_bodyparts.index(bp1), use_bodyparts.index(bp2)]
-                    )
+                    edges.append([use_bodyparts.index(bp1), use_bodyparts.index(bp2)])
     return edges
 
 
 def reindex_by_bodyparts(data, bodyparts, use_bodyparts, axis=1):
     """Use an ordered list of bodyparts to reindex keypoint coordinates.
 
     Parameters
@@ -515,33 +496,28 @@
 
     if post is None:
         trajectories = [
             coordinates[key][s - pre : e] for key, s, e in syllable_instances
         ]
         if centroids is not None and headings is not None:
             trajectories = [
-                np_io(inverse_rigid_transform)(
-                    x, centroids[key][s], headings[key][s]
-                )
+                np_io(inverse_rigid_transform)(x, centroids[key][s], headings[key][s])
                 for x, (key, s, e) in zip(trajectories, syllable_instances)
             ]
     else:
         trajectories = np.array(
-            [
-                coordinates[key][s - pre : s + post]
-                for key, s, e in syllable_instances
-            ]
+            [coordinates[key][s - pre : s + post] for key, s, e in syllable_instances]
         )
         if centroids is not None and headings is not None:
-            c = np.array(
-                [centroids[key][s] for key, s, e in syllable_instances]
-            )[:, None]
-            h = np.array(
-                [headings[key][s] for key, s, e in syllable_instances]
-            )[:, None]
+            c = np.array([centroids[key][s] for key, s, e in syllable_instances])[
+                :, None
+            ]
+            h = np.array([headings[key][s] for key, s, e in syllable_instances])[
+                :, None
+            ]
             trajectories = np_io(inverse_rigid_transform)(trajectories, c, h)
 
     return trajectories
 
 
 def sample_instances(
     syllable_instances,
@@ -604,35 +580,29 @@
     assert all([len(v) >= num_samples for v in syllable_instances.values()])
     assert n_neighbors >= num_samples
 
     if mode == "random":
         sampled_instances = {
             syllable: [
                 instances[i]
-                for i in np.random.choice(
-                    len(instances), num_samples, replace=False
-                )
+                for i in np.random.choice(len(instances), num_samples, replace=False)
             ]
             for syllable, instances in syllable_instances.items()
         }
         return sampled_instances
 
     elif mode == "density":
-        assert not (
-            coordinates is None or headings is None or centroids is None
-        ), fill(
+        assert not (coordinates is None or headings is None or centroids is None), fill(
             "`coordinates`, `headings` and `centroids` are required when "
             '`mode == "density"`'
         )
 
         for key in coordinates.keys():
             outliers = np.isnan(coordinates[key]).any(-1)
-            coordinates[key] = interpolate_keypoints(
-                coordinates[key], outliers
-            )
+            coordinates[key] = interpolate_keypoints(coordinates[key], outliers)
 
         trajectories = {
             syllable: get_instance_trajectories(
                 instances,
                 coordinates,
                 pre=pre,
                 post=post,
@@ -658,17 +628,15 @@
             nbrs = NearestNeighbors(n_neighbors=n_neighbors).fit(Xpca)
             distances, indices = nbrs.kneighbors(Xpca)
             local_density = 1 / distances.mean(1)
 
             distances, _ = all_nbrs.kneighbors(Xpca)
             global_density = 1 / distances.mean(1)
             exemplar = np.argmax(local_density / global_density)
-            samples = np.random.choice(
-                indices[exemplar], num_samples, replace=False
-            )
+            samples = np.random.choice(indices[exemplar], num_samples, replace=False)
             sampled_instances[syllable] = [
                 syllable_instances[syllable][i] for i in samples
             ]
 
         return sampled_instances
 
     else:
@@ -692,17 +660,15 @@
     -------
     x_interp: ndarray
         The interpolated values, with the same shape as fp except along the
         interpolation axis.
     """
     assert len(xp.shape) == len(x.shape) == 1
     assert fp.shape[axis] == len(xp)
-    assert (
-        len(xp) > 0
-    ), "xp must be non-empty; cannot interpolate without datapoints"
+    assert len(xp) > 0, "xp must be non-empty; cannot interpolate without datapoints"
 
     fp = np.moveaxis(fp, axis, 0)
     shape = fp.shape[1:]
     fp = fp.reshape(fp.shape[0], -1)
 
     x_interp = np.zeros((len(x), fp.shape[1]))
     for i in range(fp.shape[1]):
@@ -823,26 +789,20 @@
 
     if display_available:
 
         def colorize(val):
             color = plt.get_cmap("Reds")(val * 0.8)
             return f"background-color: rgba({int(color[0]*255)}, {int(color[1]*255)}, {int(color[2]*255)}, {color[3]})"
 
-        colored_df = df.style.applymap(colorize).set_caption(
-            "Proportion of NaNs"
-        )
+        colored_df = df.style.applymap(colorize).set_caption("Proportion of NaNs")
         display(colored_df)
         return colored_df
     else:
         print(title)
-        print(
-            tabulate(
-                df, headers="keys", tablefmt="simple_grid", showindex=True
-            )
-        )
+        print(tabulate(df, headers="keys", tablefmt="simple_grid", showindex=True))
 
 
 def check_nan_proportions(
     coordinates, bodyparts, warning_threshold=0.5, breakdown=False, **kwargs
 ):
     """Check if any bodyparts have a high proportion of NaNs.
 
@@ -868,19 +828,15 @@
         keys = sorted(coordinates.keys())
         nan_props = [np.isnan(coordinates[k]).any(-1).mean(0) for k in keys]
         _print_colored_table(keys, bodyparts, nan_props)
     else:
         all_coords = np.concatenate(list(coordinates.values()))
         nan_props = np.isnan(all_coords).any(-1).mean(0)
         if np.any(nan_props > warning_threshold):
-            bps = [
-                bp
-                for bp, p in zip(bodyparts, nan_props)
-                if p > warning_threshold
-            ]
+            bps = [bp for bp, p in zip(bodyparts, nan_props) if p > warning_threshold]
             warnings.warn(
                 "\nCoordinates for the following bodyparts are missing (set to NaN) in at least "
                 "{}% of frames:\n - {}\n\n".format(
                     warning_threshold * 100, "\n - ".join(bps)
                 )
             )
             warnings.warn(
@@ -970,17 +926,15 @@
         array of recording names and an array of (start,end) times. See
         :py:func:`jax_moseq.utils.batch` for details.
     """
     if keys is None:
         keys = sorted(coordinates.keys())
     else:
         bad_keys = set(keys) - set(coordinates.keys())
-        assert len(bad_keys) == 0, fill(
-            f"Keys {bad_keys} not found in coordinates"
-        )
+        assert len(bad_keys) == 0, fill(f"Keys {bad_keys} not found in coordinates")
 
     assert len(keys) > 0, "No recordings found"
 
     num_keypoints = [coordinates[key].shape[-2] for key in keys]
     assert len(set(num_keypoints)) == 1, fill(
         f"All recordings must have the same number of keypoints, but "
         f"found {set(num_keypoints)} keypoints across recordings."
@@ -998,47 +952,37 @@
             fill(
                 'WARNING: Recording names should not contain "/", this will cause '
                 "problems with saving/loading hdf5 files."
             )
         )
 
     if confidences is None:
-        confidences = {
-            key: np.ones_like(coordinates[key][..., 0]) for key in keys
-        }
+        confidences = {key: np.ones_like(coordinates[key][..., 0]) for key in keys}
 
     if bodyparts is not None and use_bodyparts is not None:
-        coordinates = reindex_by_bodyparts(
-            coordinates, bodyparts, use_bodyparts
-        )
-        confidences = reindex_by_bodyparts(
-            confidences, bodyparts, use_bodyparts
-        )
+        coordinates = reindex_by_bodyparts(coordinates, bodyparts, use_bodyparts)
+        confidences = reindex_by_bodyparts(confidences, bodyparts, use_bodyparts)
 
     for key in keys:
         outliers = np.isnan(coordinates[key]).any(-1)
         coordinates[key] = interpolate_keypoints(coordinates[key], outliers)
-        confidences[key] = np.where(
-            outliers, 0, np.nan_to_num(confidences[key])
-        )
+        confidences[key] = np.where(outliers, 0, np.nan_to_num(confidences[key]))
 
     if seg_length is not None:
         max_recording_length = max([coordinates[key].shape[0] for key in keys])
         seg_length = min(seg_length, max_recording_length)
 
     Y, mask, metadata = batch(coordinates, seg_length=seg_length, keys=keys)
     Y = Y.astype(float)
 
     conf = batch(confidences, seg_length=seg_length, keys=keys)[0]
     if np.min(conf) < 0:
         conf = np.maximum(conf, 0)
         warnings.warn(
-            fill(
-                "Negative confidence values are not allowed and will be set to 0."
-            )
+            fill("Negative confidence values are not allowed and will be set to 0.")
         )
     conf = conf + conf_pseudocount
 
     if added_noise_level > 0:
         Y += np.random.uniform(-added_noise_level, added_noise_level, Y.shape)
 
     data = jax.device_put({"mask": mask, "Y": Y, "conf": conf})
@@ -1101,17 +1045,15 @@
     Returns
     -------
     representative_trajectories: dict
         Dictionary mapping syllable indexes to representative trajectories
         as arrays of shape (pre+pose, n_bodyparts, [2 or 3]).
     """
     if bodyparts is not None and use_bodyparts is not None:
-        coordinates = reindex_by_bodyparts(
-            coordinates, bodyparts, use_bodyparts
-        )
+        coordinates = reindex_by_bodyparts(coordinates, bodyparts, use_bodyparts)
 
     syllables = {k: v["syllable"] for k, v in results.items()}
     centroids = {k: v["centroid"] for k, v in results.items()}
     headings = {k: v["heading"] for k, v in results.items()}
 
     min_instances = sampling_options["n_neighbors"] if density_sample else 1
     syllable_instances = get_syllable_instances(
@@ -1209,7 +1151,82 @@
         sampling_options,
     )
 
     syllable_ixs = sorted(typical_trajectories.keys())
     Xs = np.stack([typical_trajectories[s] for s in syllable_ixs])
     distances = squareform(pdist(Xs.reshape(Xs.shape[0], -1), metric))
     return distances, syllable_ixs
+
+
+def downsample_timepoints(data, downsample_rate):
+    """
+    Downsample timepoints, e.g. for of coordinates or confidences.
+
+    Parameters
+    ----------
+    data: ndarray or dict
+        Array of shape (n_frames, ...) or a dictionary with such arrays as values.
+
+    downsample_rate: int
+        The downsampling rate (e.g., `downsample_rate=2` keeps every other frame).
+
+    Returns
+    -------
+    downsampled_data: ndarray or dict
+        Downsampled array or dictionary of arrays.
+    """
+    if isinstance(data, dict):
+        return {k: downsample_timepoints(v, downsample_rate) for k, v in data.items()}
+    else:
+        return data[::downsample_rate]
+
+
+def check_video_paths(video_paths, keys):
+    """
+    Check if video paths are valid and match the keys.
+
+    Parameters
+    ----------
+    video_paths: dict
+        Dictionary mapping keys to video paths.
+
+    keys: list
+        List of keys that require a video path.
+
+    Raises
+    ------
+    ValueError
+        If any of the following are true:
+        - a video path is not provided for a key in `keys`
+        - a video isn't readable.
+        - a video path does not exist.
+    """
+    missing_keys = set(keys) - set(video_paths.keys())
+
+    nonexistent_videos = []
+    unreadable_videos = []
+    for path in video_paths.values():
+        if not os.path.exists(path):
+            nonexistent_videos.append(path)
+        else:
+            try:
+                OpenCVReader(path)[0]
+            except:
+                unreadable_videos.append(path)
+
+    error_messages = []
+
+    if len(missing_keys) > 0:
+        error_messages.append(
+            "The following keys require a video path: {}".format(missing_keys)
+        )
+    if len(nonexistent_videos) > 0:
+        error_messages.append(
+            "The following videos do not exist: {}".format(nonexistent_videos)
+        )
+    if len(unreadable_videos) > 0:
+        error_messages.append(
+            "The following videos are not readable and must be reencoded: {}".format(unreadable_videos)
+        )
+    
+    if len(error_messages) > 0:
+        raise ValueError("\n\n".join(error_messages))
```

### Comparing `keypoint-moseq-0.4.5/keypoint_moseq/viz.py` & `keypoint-moseq-0.4.6/keypoint_moseq/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -694,24 +694,27 @@
     pre,
     post,
     dot_radius,
     overlay_keypoints,
     edges,
     coordinates,
     plot_options,
+    downsample_rate,
 ):
     scale_factor = scaled_window_size / window_size
     cs = centroids[key][start - pre : start + post]
     h, c = headings[key][start], cs[pre]
     r = np.float32([[np.cos(h), np.sin(h)], [-np.sin(h), np.cos(h)]])
 
     tile = []
 
     if videos is not None:
-        frames = videos[key][start - pre : start + post]
+        frames = videos[key][
+            (start - pre) * downsample_rate : (start + post) * downsample_rate
+        ][::downsample_rate]
         c = r @ c - window_size // 2
         M = [[np.cos(h), np.sin(h), -c[0]], [-np.sin(h), np.cos(h), -c[1]]]
 
         for ii, (frame, c) in enumerate(zip(frames, cs)):
             if overlay_keypoints:
                 coords = coordinates[key][start - pre + ii]
                 frame = overlay_keypoints_on_image(
@@ -760,80 +763,82 @@
     pre=30,
     post=60,
     scaled_window_size=None,
     edges=[],
     overlay_keypoints=False,
     coordinates=None,
     plot_options={},
+    downsample_rate=1,
 ):
     """Generate a grid movie and return it as an array of frames.
 
-    Grid movies show many instances of  a syllable. Each instance contains a
-    snippet of video (and/or keypoint-overlay) centered on the animal and
-    synchronized to the onset of the syllable. A dot appears at syllable onset
-    and disappears at syllable offset.
+    Grid movies show many instances of  a syllable. Each instance contains a snippet of
+    video (and/or keypoint-overlay) centered on the animal and synchronized to the onset
+    of the syllable. A dot appears at syllable onset and disappears at syllable offset.
 
     Parameters
     ----------
     instances: list of tuples `(key, start, end)`
-        List of syllable instances to include in the grid movie, where each
-        instance is specified as a tuple with the video name, start frame and
-        end frame. The list must have length `rows*cols`. The video names must
-        also be keys in `videos`.
+        List of syllable instances to include in the grid movie, where each instance is
+        specified as a tuple with the video name, start frame and end frame. The list
+        must have length `rows*cols`. The video names must also be keys in `videos`.
 
     rows: int, cols : int
         Number of rows and columns in the grid movie grid
 
     videos: dict or None
-        Dictionary mapping video names to video readers. Frames from
-        each reader should be accessible via `__getitem__(int or slice)`. If
-        None, the the grid movie will not include video frames.
+        Dictionary mapping video names to video readers. Frames from each reader should
+        be accessible via `__getitem__(int or slice)`. If None, the the grid movie will
+        not include video frames.
 
     centroids: dict
-        Dictionary mapping video names to arrays of shape `(n_frames, 2)` with
-        the x,y coordinates of animal centroid on each frame
+        Dictionary mapping video names to arrays of shape `(n_frames, 2)` with the x,y
+        coordinates of animal centroid on each frame
 
     headings: dict
-        Dictionary mapping video names to arrays of shape `(n_frames,)` with
-        the heading of the animal on each frame (in radians)
+        Dictionary mapping video names to arrays of shape `(n_frames,)` with the heading
+        of the animal on each frame (in radians)
 
     window_size: int
-        Size of the window around the animal. This should be a multiple of 16
-        or imageio will complain.
+        Size of the window around the animal. This should be a multiple of 16 or imageio
+        will complain.
 
     dot_color: tuple of ints, default=(255,255,255)
         RGB color of the dot indicating syllable onset and offset
 
     dot_radius: int, default=4
         Radius of the dot indicating syllable onset and offset
 
     pre: int, default=30
         Number of frames before syllable onset to include in the movie
 
     post: int, default=60
         Number of frames after syllable onset to include in the movie
 
     scaled_window_size: int, default=None
-        Window size after scaling the video. If None, the no scaling is
-        performed (i.e. `scaled_window_size = window_size`)
+        Window size after scaling the video. If None, the no scaling is performed (i.e.
+        `scaled_window_size = window_size`)
 
     overlay_keypoints: bool, default=False
         If True, overlay the pose skeleton on the video frames.
 
     edges: list of tuples, default=[]
-        List of edges defining pose skeleton. Used when
-        `overlay_keypoints=True`.
+        List of edges defining pose skeleton. Used when `overlay_keypoints=True`.
 
     coordinates: dict, default=None
-        Dictionary mapping video names to arrays of shape `(n_frames, 2)`.
-        Used when `overlay_keypoints=True`.
+        Dictionary mapping video names to arrays of shape `(n_frames, 2)`. Used when
+        `overlay_keypoints=True`.
 
     plot_options: dict, default={}
-        Dictionary of options to pass to `overlay_keypoints_on_image`.
-        Used when `overlay_keypoints=True`.
+        Dictionary of options to pass to `overlay_keypoints_on_image`. Used when
+        `overlay_keypoints=True`.
+
+    downsample_rate: int, default=1
+        Downsampling rate for the video frames. Coordinates at index `i` will be
+        plotted on the video frame at index `i*downsample_rate`.
 
     Returns
     -------
     frames: array of shape `(post+pre, width, height, 3)`
         Array of frames in the grid movie where::
 
             width = rows * scaled_window_size
@@ -864,14 +869,15 @@
                 pre,
                 post,
                 dot_radius,
                 overlay_keypoints,
                 edges,
                 coordinates,
                 plot_options,
+                downsample_rate,
             )
         )
 
     tiles = np.stack(tiles).reshape(
         rows, cols, post + pre, scaled_window_size, scaled_window_size, 3
     )
     frames = np.concatenate(np.concatenate(tiles, axis=2), axis=2)
@@ -973,14 +979,15 @@
     overlay_keypoints=False,
     keypoints_only=False,
     keypoints_scale=1,
     fps=None,
     plot_options={},
     use_dims=[0, 1],
     keypoint_colormap="autumn",
+    downsample_rate=1,
     **kwargs,
 ):
     """Generate grid movies for a modeled dataset.
 
     Grid movies show many instances of a syllable and are useful in
     figuring out what behavior the syllable captures
     (see :py:func:`keypoint_moseq.viz.grid_movie`). This method
@@ -1107,14 +1114,18 @@
         Dimensions to use for plotting keypoints. Only used when
         `overlay_keypoints=True` and the keypoints are 3D.
 
     keypoint_colormap: str, default='autumn'
         Colormap used to color keypoints. Used when
         `overlay_keypoints=True`.
 
+    downsample_rate: int, default=1
+        Downsampling rate for the video frames. Coordinates at index `i` will be
+        plotted on the video frame at index `i*downsample_rate`.
+
 
     See :py:func:`keypoint_moseq.viz.grid_movie` for the remaining parameters.
 
     Returns
     -------
     sampled_instances: dict
         Dictionary mapping syllables to lists of instances shown in each in
@@ -1181,14 +1192,15 @@
         if video_paths is None:
             video_paths = find_matching_videos(
                 results.keys(),
                 video_dir,
                 as_dict=True,
                 video_extension=video_extension,
             )
+        check_video_paths(video_paths, results.keys())
         videos = {k: OpenCVReader(path) for k, path in video_paths.items()}
 
         if fps is None:
             fps = list(videos.values())[0].fps
     else:
         videos = None
 
@@ -1281,14 +1293,15 @@
             dot_color=dot_color,
             pre=pre,
             post=post,
             dot_radius=dot_radius,
             overlay_keypoints=overlay_keypoints,
             coordinates=coordinates,
             plot_options=plot_options,
+            downsample_rate=downsample_rate,
         )
 
         path = os.path.join(output_dir, f"syllable{syllable}.mp4")
         write_video_clip(frames, path, fps=fps, quality=quality)
 
     return sampled_instances
 
@@ -1903,62 +1916,67 @@
     show_frame_numbers=True,
     text_color=(255, 255, 255),
     crop_size=None,
     frames=None,
     quality=7,
     centroid_smoothing_filter=10,
     plot_options={},
+    downsample_rate=1,
 ):
     """Overlay keypoints on a video.
 
     Parameters
     ----------
     video_path: str
         Path to a video file.
 
     coordinates: ndarray of shape (num_frames, num_keypoints, 2)
         Array of keypoint coordinates.
 
     skeleton: list of tuples, default=[]
-        List of edges that define the skeleton, where each edge is a
-        pair of bodypart names or a pair of indexes.
+        List of edges that define the skeleton, where each edge is a pair of bodypart
+        names or a pair of indexes.
 
     bodyparts: list of str, default=None
-        List of bodypart names in `coordinates`. Required if
-        `skeleton` is defined using bodypart names.
+        List of bodypart names in `coordinates`. Required if `skeleton` is defined using
+        bodypart names.
 
     use_bodyparts: list of str, default=None
         Subset of bodyparts to plot. If None, all bodyparts are plotted.
 
     output_path: str, default=None
-        Path to save the video. If None, the video is saved to
-        `video_path` with the suffix `_keypoints`.
+        Path to save the video. If None, the video is saved to `video_path` with the
+        suffix `_keypoints`.
 
     show_frame_numbers: bool, default=True
         Whether to overlay the frame number in the video.
 
     text_color: tuple of int, default=(255,255,255)
         Color for the frame number overlay.
 
     crop_size: int, default=None
-        Size of the crop around the keypoints to overlay on the video.
-        If None, the entire video is used.
+        Size of the crop around the keypoints to overlay on the video. If None, the
+        entire video is used.
 
     frames: iterable of int, default=None
         Frames to overlay keypoints on. If None, all frames are used.
 
     quality: int, default=7
         Quality of the output video.
 
     centroid_smoothing_filter: int, default=10
         Amount of smoothing to determine cropping centroid.
 
     plot_options: dict, default={}
         Additional keyword arguments to pass to
         :py:func:`keypoint_moseq.viz.overlay_keypoints`.
+
+    downsample_rate: int, default=1
+        Downsampling rate for the video frames. Coordinates at index `i` will be
+        overlayed on the frame at index `i*downsample_rate`.
     """
     if output_path is None:
         output_path = os.path.splitext(video_path)[0] + "_keypoints.mp4"
         print(f"Saving video to {output_path}")
 
     if bodyparts is not None:
         if use_bodyparts is not None:
```

### Comparing `keypoint-moseq-0.4.5/setup.cfg` & `keypoint-moseq-0.4.6/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 classifiers = 
 	Programming Language :: Python :: 3
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
-python_requires = >=3.8
+python_requires = >=3.9
 install_requires = 
 	seaborn==0.13.0
 	cytoolz
 	matplotlib
 	tqdm
 	ipykernel
 	imageio[ffmpeg]
@@ -30,15 +30,15 @@
 	pynwb
 	ndx_pose
 	plotly
 	ipython_genutils
 	tabulate
 	commentjson
 	jaxtyping==0.2.14
-	jax-moseq==0.2.1
+	jax-moseq==0.2.2
 
 [options.package_data]
 * = *.md
 
 [versioneer]
 VCS = git
 style = pep440
```

### Comparing `keypoint-moseq-0.4.5/versioneer.py` & `keypoint-moseq-0.4.6/versioneer.py`

 * *Files identical despite different names*

