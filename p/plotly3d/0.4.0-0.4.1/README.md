# Comparing `tmp/plotly3d-0.4.0.tar.gz` & `tmp/plotly3d-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly3d-0.4.0.tar", last modified: Sun Apr 14 14:08:59 2024, max compression
+gzip compressed data, was "plotly3d-0.4.1.tar", last modified: Tue Apr 16 20:30:31 2024, max compression
```

## Comparing `plotly3d-0.4.0.tar` & `plotly3d-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-14 14:08:59.416954 plotly3d-0.4.0/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.4.0/LICENSE
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      336 2024-04-14 14:08:59.416180 plotly3d-0.4.0/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      100 2024-04-01 03:31:03.000000 plotly3d-0.4.0/README.md
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-14 14:08:59.404695 plotly3d-0.4.0/plotly3d/
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.4.0/plotly3d/__init__.py
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     9662 2024-04-14 14:08:35.000000 plotly3d-0.4.0/plotly3d/plot.py
-drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-14 14:08:59.415423 plotly3d-0.4.0/plotly3d.egg-info/
--rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      336 2024-04-14 14:08:59.405559 plotly3d-0.4.0/plotly3d.egg-info/PKG-INFO
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-14 14:08:59.407072 plotly3d-0.4.0/plotly3d.egg-info/SOURCES.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-14 14:08:59.414564 plotly3d-0.4.0/plotly3d.egg-info/dependency_links.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       44 2024-04-14 14:08:59.415077 plotly3d-0.4.0/plotly3d.egg-info/requires.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-14 14:08:59.415511 plotly3d-0.4.0/plotly3d.egg-info/top_level.txt
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-14 14:08:59.417024 plotly3d-0.4.0/setup.cfg
--rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      425 2024-04-14 14:08:52.000000 plotly3d-0.4.0/setup.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-16 20:30:31.792157 plotly3d-0.4.1/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)     1058 2024-03-31 02:54:34.000000 plotly3d-0.4.1/LICENSE
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-16 20:30:31.791395 plotly3d-0.4.1/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      100 2024-04-01 03:31:03.000000 plotly3d-0.4.1/README.md
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-16 20:30:31.787002 plotly3d-0.4.1/plotly3d/
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-02 02:59:03.000000 plotly3d-0.4.1/plotly3d/__init__.py
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)     8257 2024-04-16 20:02:28.000000 plotly3d-0.4.1/plotly3d/plot.py
+drwxrwxr-x   0 xs272    (18671) krishnaswamy_smita (10612)        0 2024-04-16 20:30:31.790779 plotly3d-0.4.1/plotly3d.egg-info/
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      310 2024-04-16 20:30:31.788289 plotly3d-0.4.1/plotly3d.egg-info/PKG-INFO
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)      223 2024-04-16 20:30:31.788899 plotly3d-0.4.1/plotly3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        1 2024-04-16 20:30:31.789648 plotly3d-0.4.1/plotly3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       33 2024-04-16 20:30:31.790390 plotly3d-0.4.1/plotly3d.egg-info/requires.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)        9 2024-04-16 20:30:31.790830 plotly3d-0.4.1/plotly3d.egg-info/top_level.txt
+-rw-rw-r--   0 xs272    (18671) krishnaswamy_smita (10612)       38 2024-04-16 20:30:31.792230 plotly3d-0.4.1/setup.cfg
+-rw-r--r--   0 xs272    (18671) krishnaswamy_smita (10612)      404 2024-04-16 20:28:42.000000 plotly3d-0.4.1/setup.py
```

### Comparing `plotly3d-0.4.0/LICENSE` & `plotly3d-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly3d-0.4.0/plotly3d/plot.py` & `plotly3d-0.4.1/plotly3d/plot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,259 +1,207 @@
 import plotly.graph_objects as go
 from sklearn.preprocessing import MinMaxScaler
 import numpy as np
 import pandas as pd
-import matplotlib.pyplot as plt
-import matplotlib
+import os
+import plotly.express as px
+import matplotlib.cm as cm
+
 
 def scatter(points, colors=None, **kwargs):
-    # FIXME: debug force_continous!!
     """
     Plots 3D scatter plot with optional rescaling, coloring, and customization.
     
     Parameters:
     - points: Array of points to plot.
     - colors: Optional array of colors for each point.
     - scaler: Optional scaler object to rescale points. If None and rescaling is enabled, MinMaxScaler is used.
     - **kwargs: Additional optional arguments:
         - s (float): Size of the markers.
         - alpha (float): Opacity of the markers.
-        - force_continuous (bool): When True, applies a continuous colormap but discretizes it for categorical data.
+        - force_continuous (bool): Force treating colors as continuous even if they seem categorical.
         - title (str): Title of the plot.
         - filename (str): If provided, saves the plot to this file.
         - rescale (bool): If True, rescales points using the provided or default scaler.
         - fig (go.Figure): Plotly figure object to which the scatter plot will be added. If None, a new figure is created.
         - xtitle (str), ytitle (str), ztitle (str): Titles for the X, Y, and Z axes.
-        - colorscale (str): Colormap to use ('Viridis', 'Inferno', etc.).
-        - legend (bool): Whether to show legend.
     """
     is_3d = points.shape[1] == 3
     plot_func = go.Scatter3d if is_3d else go.Scatter
     scaler = kwargs.get('scaler', None)
-    s = kwargs.get('s', 6)  # Default size
-    alpha = kwargs.get('alpha', 0.8)  # Default opacity
+    s = kwargs.get('s', 1)
+    alpha = kwargs.get('alpha', 1)
     title = kwargs.get('title', 'Plot')
     filename = kwargs.get('filename', None)
     xtitle = kwargs.get('xtitle', 'X')
     ytitle = kwargs.get('ytitle', 'Y')
     ztitle = kwargs.get('ztitle', 'Z')
     force_continuous = kwargs.get('force_continuous', False)
     rescale = kwargs.get('rescale', False)
     legend = kwargs.get('legend', True)
-    colorscale = kwargs.get('colorscale', 'Viridis').capitalize()  # Ensure correct case
+    colorscale = kwargs.get('colorscale', 'Viridis')
     fig = kwargs.get('fig', go.Figure())
     points = np.asarray(points)
     colors = np.asarray(colors) if colors is not None else None
-    
     if rescale:
         if scaler is None:
             scaler = MinMaxScaler()
             scaler.fit(points)
         points_s = scaler.transform(points)
     else:
         points_s = points
 
     if colors is None:
         colors = np.zeros(points.shape[0])
         is_categorical = True
     else:
+        # Step 1: Determine Color Type
         unique_colors = np.unique(colors)
-        is_categorical = not force_continuous and (len(unique_colors) / len(colors) < 0.05)
-    
-    if force_continuous and colors is not None and is_categorical:
-        # Normalize color values for continuous colormap application
-        color_map, _ = pd.factorize(colors, sort=True)
-        color_vals = MinMaxScaler().fit_transform(color_map.reshape(-1, 1)).flatten()
-        cmap = plt.get_cmap(colorscale)
-        discrete_mapping = cmap(color_vals)  # Apply colormap
-        
-        hex_colors = [matplotlib.colors.rgb2hex(color) for color in discrete_mapping]  # Convert to hex
-
-        fig.add_trace(plot_func(
-            x=points_s[:, 0],
-            y=points_s[:, 1],
-            z=points_s[:, 2] if is_3d else None,
-            mode='markers',
-            marker=dict(size=s, color=hex_colors, opacity=alpha),
-            hoverinfo='text',
-            text=colors,  # Show original category names on hover
-        ))
+        is_categorical = (len(unique_colors) / len(colors) < 0.05) and not force_continuous # Heuristic threshold
+        # Step 2: Preprocess Points
+    if is_categorical:
+        # Step 3: Categorical Colors Plotting Strategy
+        # Map categorical color labels to integers
+        color_map, categories = pd.factorize(colors, sort=True)
+        # Create a trace for each unique color/category
+        for i, color in enumerate(categories):
+            idx = color_map == i
+            if is_3d:
+                fig.add_trace(plot_func(
+                    x=points_s[idx, 0],
+                    y=points_s[idx, 1],
+                    z=points_s[idx, 2],
+                    mode='markers',
+                    marker=dict(size=s, opacity=alpha, color=i), # Use integer mapping for color
+                    name=str(color)  # Use actual category name for legend
+                ))
+            else:
+                fig.add_trace(plot_func(
+                    x=points_s[idx, 0],
+                    y=points_s[idx, 1],
+                    mode='markers',
+                    marker=dict(size=s, opacity=alpha, color=i), # Use integer mapping for color
+                    name=str(color)  # Use actual category name for legend
+                ))
     else:
-        # Continuous or non-force_continuous categorical handling
+        # Step 3: Continuous Colors Plotting Strategy
         if is_3d:
             fig.add_trace(plot_func(
                 x=points_s[:, 0],
                 y=points_s[:, 1],
                 z=points_s[:, 2],
                 mode='markers',
-                marker=dict(size=s, color=colors, colorscale=colorscale, opacity=alpha, colorbar=dict(title='Color Scale') if not is_categorical else None),
+                marker=dict(size=s, color=colors, colorscale='Viridis', opacity=alpha, colorbar=dict(title='Color Scale')),
             ))
         else:
             fig.add_trace(plot_func(
                 x=points_s[:, 0],
                 y=points_s[:, 1],
                 mode='markers',
-                marker=dict(size=s, color=colors, colorscale=colorscale, opacity=alpha, colorbar=dict(title='Color Scale') if not is_categorical else None),
+                marker=dict(size=s, color=colors, colorscale='Viridis', opacity=alpha, colorbar=dict(title='Color Scale')),
             ))
-
-    # Layout updates
+    
+    fig.data[0].marker.colorscale = colorscale
     if is_3d:
         fig.update_layout(
             title=title,
-            scene=dict(
-                xaxis_title=xtitle,
-                yaxis_title=ytitle,
-                zaxis_title=ztitle
-            ),
+            scene=dict(xaxis_title=xtitle, yaxis_title=ytitle, zaxis_title=ztitle),
             showlegend=legend
         )
     else:
         fig.update_layout(
             title=title,
-            xaxis_title=xtitle,
-            yaxis_title=ytitle,
+            xaxis_title=xtitle, yaxis_title=ytitle,
             showlegend=legend
         )
     if filename is not None:
         fig.write_html(filename)
 
     return fig
 
 # for compatability with previous versions
 plot_3d = scatter
 scatter3d = scatter
 
-# def trajectories(trajs, s=1, alpha=1, title="3D Plot", filename=None, rescale=True, fig=None, xtitle='X', ytitle='Y', ztitle='Z', scaler=None, legend_label="Trajectories"):
-def trajectories(trajs, **kwargs):
+def trajectories(trajs, colors=None, **kwargs):
     """
-    Plots trajectories in 3D space using Plotly, with thinner gray lines without markers and reduced line opacity.
+    Plots trajectories in 3D space using Plotly, with unique colors for each category and a single legend entry per category.
 
     Parameters:
     - trajs: numpy array of shape (a, b, c), where
       a: time bins, b: trajectory index, c: space dimension (c=3 for 3D).
 
     Returns:
     - Plotly figure containing the trajectories plotted in 3D space.
     """
     is_3d = trajs.shape[2] == 3
     plot_func = go.Scatter3d if is_3d else go.Scatter
     s = kwargs.get('s', 1)
     s_end = kwargs.get('s_end', 1)
-    alpha = kwargs.get('alpha', 1)
     title = kwargs.get('title', 'Plot')
     filename = kwargs.get('filename', None)
-    rescale = kwargs.get('rescale', False)
+    rescale = kwargs.get('rescale', True)
     fig = kwargs.get('fig', go.Figure())
     xtitle = kwargs.get('xtitle', 'X')
     ytitle = kwargs.get('ytitle', 'Y')
     ztitle = kwargs.get('ztitle', 'Z')
     scaler = kwargs.get('scaler', None)
-    legend_label = kwargs.get('legend_label', 'Trajectories')
-    c = kwargs.get('c', 'gray')
-    ctip = kwargs.get('ctip', 'red')
+    # colors = kwargs.get('colors', None)
+    cmap = kwargs.get('cmap', 'tab20')
+
+    if colors is None:
+        colors = np.zeros(trajs.shape[1])
+    # color_palette = kwargs.get('color_palette', px.colors.qualitative.Plotly)  # Define a color palette
 
     trajs = np.asarray(trajs)
-    if rescale:
-        if scaler is None:
-            scaler = MinMaxScaler()
-            scaler.fit(trajs.reshape(-1, trajs.shape[2]))
-        trajs_s = scaler.transform(trajs.reshape(-1, trajs.shape[2])).reshape(trajs.shape)
-    else:
-        trajs_s = trajs
+    if rescale and scaler is None:
+        scaler = MinMaxScaler()
+        scaler.fit(trajs.reshape(-1, trajs.shape[2]))
+    trajs_s = scaler.transform(trajs.reshape(-1, trajs.shape[2])).reshape(trajs.shape) if rescale else trajs
 
-    # Number of trajectories
-    num_trajectories = trajs.shape[1]
+    color_map, categories = pd.factorize(colors, sort=True)
+    cmap = cm.get_cmap(cmap, len(categories))  # Get a colormap with as many colors as categories
     
-    # Use a legendgroup and make the dummy trace for the legend entry
-    legendgroup = "trajectories"
-    # Add a dummy trace for the legend entry, enabling its visibility toggles the group
-    if is_3d:
-        fig.add_trace(plot_func(
-            x=[None],
-            y=[None],
-            z=[None],
-            mode='lines',
-            line=dict(color=c, width=s),
-            name=legend_label,
-            legendgroup=legendgroup,
-            # This is the key for toggling visibility
-            visible=True
-        ))
-    else:
-        fig.add_trace(plot_func(
-            x=[None],
-            y=[None],
-            mode='lines',
-            line=dict(color=c, width=s),
-            name=legend_label,
-            legendgroup=legendgroup,
-            # This is the key for toggling visibility
-            visible=True
-        ))
-    # Iterate over each trajectory and plot it, linked by legendgroup
-    for i in range(num_trajectories):
-        trajectory = trajs_s[:, i, :]
-        if is_3d:
-            fig.add_trace(plot_func(
-                x=trajectory[:, 0],
-                y=trajectory[:, 1],
-                z=trajectory[:, 2],
-                mode='lines',
-                line=dict(width=s, color=c),
-                opacity=alpha,
-                showlegend=False,  # Do not show these individual traces in the legend
-                legendgroup=legendgroup,  # Link visibility control to the dummy trace
-                visible=True  # Initially visible
-            ))
-        else:
+    # color_map = color_map % len(color_palette)  # Ensure we use the color palette cyclically if not enough colors
+
+    for i, color in enumerate(categories):
+        category_color = cmap(i % 20)[:3]  # Get color from colormap, repeat if more than 20 categories
+        category_color = 'rgb' + str(tuple(int(c*255) for c in category_color))  # Convert to RGB string for Plotly
+        idx = color_map == i
+        first_idx = np.where(idx)[0][0]
+        for j in np.where(idx)[0]:
+            trajectory = trajs_s[:, j, :]
+            showlegend = (j == first_idx)  # Compare indices to determine if it's the first trajectory
+            showlegend = bool(showlegend)  # Explicitly convert to Python bool
+            
+            # Add the trace for the trajectory
             fig.add_trace(plot_func(
                 x=trajectory[:, 0],
                 y=trajectory[:, 1],
-                mode='lines',
-                line=dict(width=s, color=c),
-                opacity=alpha,
-                showlegend=False,  # Do not show these individual traces in the legend
-                legendgroup=legendgroup,  # Link visibility control to the dummy trace
-                visible=True  # Initially visible
+                z=trajectory[:, 2] if is_3d else None,
+                mode= 'lines',  # Add markers only for the first trajectory
+                line=dict(width=s, color=category_color),
+                name=str(color) if showlegend else '',  # Only set the name for the first trajectory
+                showlegend=showlegend,
+                legendgroup=str(color)
             ))
-        # Add endpoint marker
-        if is_3d:
-            fig.add_trace(plot_func(
-                x=[trajectory[-1, 0]],
-                y=[trajectory[-1, 1]],
-                z=[trajectory[-1, 2]],
-                mode='markers',
-                marker=dict(size=s_end, color=ctip), # Customize color and size as needed
-                showlegend=False,
-                legendgroup=legendgroup,
-                visible=True
-            ))
-        else:
+
             fig.add_trace(plot_func(
                 x=[trajectory[-1, 0]],
                 y=[trajectory[-1, 1]],
+                z=[trajectory[-1, 2]] if is_3d else None,
                 mode='markers',
-                marker=dict(size=s_end, color=ctip), # Customize color and size as needed
+                marker=dict(size=s_end, color='black'),  # Black dot
                 showlegend=False,
-                legendgroup=legendgroup,
-                visible=True
+                legendgroup=str(color)
             ))
 
-    # Set the layout for the 3D plot
-    if is_3d:
-        fig.update_layout(
-            title=title,
-            scene=dict(
-                xaxis_title=xtitle, yaxis_title=ytitle, zaxis_title=ztitle,
-            ),
-            margin=dict(l=0, r=0, b=0, t=30)
-        )
-    else:
-        fig.update_layout(
-            title=title,
-            xaxis_title=xtitle, yaxis_title=ytitle,
-            margin=dict(l=0, r=0, b=0, t=30)
-        )
+    fig.update_layout(
+        title=title,
+        scene=dict(xaxis_title=xtitle, yaxis_title=ytitle, zaxis_title=ztitle) if is_3d else dict(),
+        margin=dict(l=0, r=0, b=0, t=30)
+    )
+
     if filename is not None:
         fig.write_html(filename)
 
-    return fig
+    return fig
```

