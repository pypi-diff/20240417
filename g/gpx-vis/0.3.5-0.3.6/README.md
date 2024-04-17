# Comparing `tmp/gpx_vis-0.3.5.tar.gz` & `tmp/gpx_vis-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpx_vis-0.3.5.tar", last modified: Tue Apr 16 14:41:17 2024, max compression
+gzip compressed data, was "gpx_vis-0.3.6.tar", last modified: Wed Apr 17 15:59:51 2024, max compression
```

## Comparing `gpx_vis-0.3.5.tar` & `gpx_vis-0.3.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-16 14:41:17.067264 gpx_vis-0.3.5/
--rw-r--r--   0 jwt        (501) staff       (20)     1514 2024-04-05 12:16:08.000000 gpx_vis-0.3.5/LICENSE
--rw-r--r--   0 jwt        (501) staff       (20)     5178 2024-04-16 14:41:17.067036 gpx_vis-0.3.5/PKG-INFO
--rw-r--r--   0 jwt        (501) staff       (20)     4628 2024-04-16 14:29:36.000000 gpx_vis-0.3.5/README.md
--rw-r--r--   0 jwt        (501) staff       (20)      590 2024-04-16 14:40:07.000000 gpx_vis-0.3.5/pyproject.toml
--rw-r--r--   0 jwt        (501) staff       (20)       38 2024-04-16 14:41:17.067325 gpx_vis-0.3.5/setup.cfg
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-16 14:41:17.064998 gpx_vis-0.3.5/src/
--rw-r--r--   0 jwt        (501) staff       (20)      113 2024-04-07 22:23:57.000000 gpx_vis-0.3.5/src/__init__.py
-drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-16 14:41:17.066720 gpx_vis-0.3.5/src/gpx_vis.egg-info/
--rw-r--r--   0 jwt        (501) staff       (20)     5178 2024-04-16 14:41:17.000000 gpx_vis-0.3.5/src/gpx_vis.egg-info/PKG-INFO
--rw-r--r--   0 jwt        (501) staff       (20)      237 2024-04-16 14:41:17.000000 gpx_vis-0.3.5/src/gpx_vis.egg-info/SOURCES.txt
--rw-r--r--   0 jwt        (501) staff       (20)        1 2024-04-16 14:41:17.000000 gpx_vis-0.3.5/src/gpx_vis.egg-info/dependency_links.txt
--rw-r--r--   0 jwt        (501) staff       (20)       83 2024-04-16 14:41:17.000000 gpx_vis-0.3.5/src/gpx_vis.egg-info/requires.txt
--rw-r--r--   0 jwt        (501) staff       (20)       17 2024-04-16 14:41:17.000000 gpx_vis-0.3.5/src/gpx_vis.egg-info/top_level.txt
--rw-r--r--   0 jwt        (501) staff       (20)    20778 2024-04-16 13:35:51.000000 gpx_vis-0.3.5/src/gpx_vis.py
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-17 15:59:51.827624 gpx_vis-0.3.6/
+-rw-r--r--   0 jwt        (501) staff       (20)     1514 2024-04-05 12:16:08.000000 gpx_vis-0.3.6/LICENSE
+-rw-r--r--   0 jwt        (501) staff       (20)     5020 2024-04-17 15:59:51.827404 gpx_vis-0.3.6/PKG-INFO
+-rw-r--r--   0 jwt        (501) staff       (20)     4470 2024-04-17 08:37:56.000000 gpx_vis-0.3.6/README.md
+-rw-r--r--   0 jwt        (501) staff       (20)      590 2024-04-17 15:59:45.000000 gpx_vis-0.3.6/pyproject.toml
+-rw-r--r--   0 jwt        (501) staff       (20)       38 2024-04-17 15:59:51.827680 gpx_vis-0.3.6/setup.cfg
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-17 15:59:51.825581 gpx_vis-0.3.6/src/
+-rw-r--r--   0 jwt        (501) staff       (20)      113 2024-04-07 22:23:57.000000 gpx_vis-0.3.6/src/__init__.py
+drwxr-xr-x   0 jwt        (501) staff       (20)        0 2024-04-17 15:59:51.827103 gpx_vis-0.3.6/src/gpx_vis.egg-info/
+-rw-r--r--   0 jwt        (501) staff       (20)     5020 2024-04-17 15:59:51.000000 gpx_vis-0.3.6/src/gpx_vis.egg-info/PKG-INFO
+-rw-r--r--   0 jwt        (501) staff       (20)      237 2024-04-17 15:59:51.000000 gpx_vis-0.3.6/src/gpx_vis.egg-info/SOURCES.txt
+-rw-r--r--   0 jwt        (501) staff       (20)        1 2024-04-17 15:59:51.000000 gpx_vis-0.3.6/src/gpx_vis.egg-info/dependency_links.txt
+-rw-r--r--   0 jwt        (501) staff       (20)       83 2024-04-17 15:59:51.000000 gpx_vis-0.3.6/src/gpx_vis.egg-info/requires.txt
+-rw-r--r--   0 jwt        (501) staff       (20)       17 2024-04-17 15:59:51.000000 gpx_vis-0.3.6/src/gpx_vis.egg-info/top_level.txt
+-rw-r--r--   0 jwt        (501) staff       (20)    20660 2024-04-17 15:58:18.000000 gpx_vis-0.3.6/src/gpx_vis.py
```

### Comparing `gpx_vis-0.3.5/LICENSE` & `gpx_vis-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gpx_vis-0.3.5/PKG-INFO` & `gpx_vis-0.3.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpx_vis
-Version: 0.3.5
+Version: 0.3.6
 Summary: Visualising your Komoot/Strava tours
 Author-email: Jia Wei Teh <jiaweiteh.astro@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,19 +16,19 @@
 Requires-Dist: matplotlib
 Requires-Dist: vincenty
 Requires-Dist: altair
 Requires-Dist: gpxpy
 
 ### About `gpx_vis`
 
-`gpx_vis` enables simple and convenient visualisation of your cycling and hiking tours, whether you're conquering mountain trails or cruising city streets.
+Transforms your .GPX files into an interactive map, whether you're conquering mountain trails or cruising city streets.
 
-You can easily transform your .GPX files into interactive and informative visualizations - just make sure your file includes data for `latitude`, `longitude`, `elevation`, and `time`, 
-and you're good to go! Whether you're using apps like <a href="https://www.komoot.com/" target="_blank">Komoot</a> and <a href="https://www.strava.com/" target="_blank">Strava</a>,
- or crafting tracks on platforms like <a href="https://gpx.studio/" target="_blank">gpx.studio</a>, `gpx_vis` has you covered.
+Whether you're using apps like <a href="https://www.komoot.com/" target="_blank">Komoot</a> and <a href="https://www.strava.com/" target="_blank">Strava</a>,
+ or crafting tracks on platforms like <a href="https://gpx.studio/" target="_blank">gpx.studio</a> - just make sure your 
+ file includes data for `latitude`, `longitude`, `elevation`, and `time`, and you're good to go!
 
 Important note: `gpx_vis` is still in its development phase, so expect more exciting features 
 and enhancements down the trail. But in the meantime, buckle up and get ready to explore your adventures! :climbing::bicyclist:
 
 
 ### Contents
 [Installation](#Install)<br>
@@ -60,72 +60,76 @@
 
 track = Track(pathname)
 ```
 
 `pathname` serves as a reference to either a single `.gpx` file or a directory.
 If a directory path is provided, all .gpx files contained within that directory
 will be merged, but retain their original metadata (e.g., different tracks remain separated).
+
 This allows users to overlay multiple tracks onto a single map, 
 providing a comprehensive summary of the data being analyzed.
 
 ## Map creation
 
 ```python
 track.create_map(filename)
 ```
 
-This generates an HTML file saved under `filename`, which contains an interactive map <a href="https://raw.githack.com/JiaWeiTeh/gpx_vis/main/example/map.html" target="_blank">(example)</a>.
-Each segment of a track corresponds to the elevation relative to user's position: blue = lower elevation, yellow = higher elevation. Users can hover over routes or click on final waypoints (flags) for additional information:
+* This generates an HTML file saved under `filename`, which contains an interactive map <a href="https://raw.githack.com/JiaWeiTeh/gpx_vis/main/example/map.html" target="_blank">(example)</a>.
+
+* Each segment of a track corresponds to the elevation relative to user's position: blue = lower elevation, yellow = higher elevation. 
+
+* Users can hover over routes or click on final waypoints (flags) for additional information:
 
-![](https://github.com/JiaWeiTeh/gpx_vis/blob/main/media/track_info.png)
+![](https://raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/track_info.png)
 
 Different backgrounds are available (selectable at lower-right corner):
 
 |Tile type             |  Example  |
 |----------------------|-----------|
-|Dark |  ![](https://github.com/JiaWeiTeh/gpx_vis/blob/main/media/ex_dark.png) |
-|Street view | ![](https://github.com/JiaWeiTeh/gpx_vis/blob/main/media/ex_openstreet.png) |
-|Plain |  ![](https://github.com/JiaWeiTeh/gpx_vis/blob/main/media/ex_plain.png) |
-|Plain (Heirarchical) |  ![](https://github.com/JiaWeiTeh/gpx_vis/blob/main/media/ex_plainheir.png) |
+|Dark |  ![](https://raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/ex_dark.png) |
+|Street view | ![](https://raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/ex_openstreet.png) |
+|Plain |  ![](https://raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/ex_plain.png) |
+|Plain (Heirarchical) |  ![](https://raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/ex_plainheir.png) |
 
 In cases where the map contains a large dataset and loading time is a concern (if one
-has been very hardworking), users have the option to include `lite = True`. By default, this option limits the 
-number of data points displayed on each route to `nlite = 50`. However, users can adjust this
-limit using the `nlite` argument, for instance,
+has been very hardworking), users have the option to include `lite = True`. 
+
+* By default, this option limits the number of data points displayed on each route to `nlite = 50`. This is adjustable using `nlite` argument:
 
 ```python
 track.create_map(filename, lite=True, nlite=100)
 ```
 
 Note that the minimum value for `nlite` is `10`.
 
 ## City overview
 
 ```python
 track.city_list
 ```
 
 Interested in the cities you passed through on your journey? This command generates a list
-of cities - sorted by country and name - that were detected along the tour route. The 
-`frequency` parameter indicates how many times each city was encountered,
-providing a rough estimate of the time spent in each city.
+of cities - sorted by country and name - that were detected along the tour route. 
+
+* The `frequency` parameter indicates how many times each city was encountered, providing a rough estimate of the time spent in each city.
 
 
 ## Additional information
 
 If you wish to plot or inspect different values, these parameters are also accessible via:
 
-`track.t`: time (UTC)<br>
-`track.x`: longitude (deg) - x values on a graph would represent the latitude.<br> 
-`track.y`: latitude (deg)<br>
-`track.z`: elevation (m)<br>
+* `track.t`: time (UTC)<br>
+* `track.x`: longitude (deg) - x values on a graph would represent the latitude.<br> 
+* `track.y`: latitude (deg)<br>
+* `track.z`: elevation (m)<br>
 
 For a more comprehensive and unprocessed dataset, you can use:
 
-`track.data`:  Returns a `pandas.DataFrame` with headers `['trackName', 'latitude', 'longitude', 'elevation', 'time']`
+`track.data`:  Returns all data in a `pandas.DataFrame` accessible format.
 
 
 ## Dependencies
 (numpy) https://numpy.org/ <br>
 (pandas) https://pandas.pydata.org/ <br>
 (altair) https://altair-viz.github.io/ <br>
 (branca) https://pypi.org/project/branca/ <br>
```

#### html2text {}

```diff
@@ -1,67 +1,66 @@
-Metadata-Version: 2.1 Name: gpx_vis Version: 0.3.5 Summary: Visualising your
+Metadata-Version: 2.1 Name: gpx_vis Version: 0.3.6 Summary: Visualising your
 Komoot/Strava tours Author-email: Jia Wei Teh
 gmail.com> Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: folium Requires-Dist:
 numpy Requires-Dist: pandas Requires-Dist: humanfriendly Requires-Dist:
 reverse_geocode Requires-Dist: matplotlib Requires-Dist: vincenty Requires-
-Dist: altair Requires-Dist: gpxpy ### About `gpx_vis` `gpx_vis` enables simple
-and convenient visualisation of your cycling and hiking tours, whether you're
-conquering mountain trails or cruising city streets. You can easily transform
-your .GPX files into interactive and informative visualizations - just make
-sure your file includes data for `latitude`, `longitude`, `elevation`, and
-`time`, and you're good to go! Whether you're using apps like _K_o_m_o_o_t and
-_S_t_r_a_v_a, or crafting tracks on platforms like _g_p_x_._s_t_u_d_i_o, `gpx_vis` has you
-covered. Important note: `gpx_vis` is still in its development phase, so expect
-more exciting features and enhancements down the trail. But in the meantime,
-buckle up and get ready to explore your adventures! :climbing::bicyclist: ###
-Contents [Installation](#Install)
+Dist: altair Requires-Dist: gpxpy ### About `gpx_vis` Transforms your .GPX
+files into an interactive map, whether you're conquering mountain trails or
+cruising city streets. Whether you're using apps like _K_o_m_o_o_t and _S_t_r_a_v_a, or
+crafting tracks on platforms like _g_p_x_._s_t_u_d_i_o - just make sure your file
+includes data for `latitude`, `longitude`, `elevation`, and `time`, and you're
+good to go! Important note: `gpx_vis` is still in its development phase, so
+expect more exciting features and enhancements down the trail. But in the
+meantime, buckle up and get ready to explore your adventures! :climbing::
+bicyclist: ### Contents [Installation](#Install)
 [How to use](#Instantiate)
 * [Map creation](#Map-creation) * [City overview](#City-overview) * [Additional
 information](#Additional-information) ## Install Installing `gpx_vis` is
 straightforward through _P_y_P_I: ```bash pip install gpx_vis ``` To update to the
 latest version (if applicable): ```bash pip install gpx_vis --upgrade ``` ##
 Instantiate ```python from gpx_vis import Track track = Track(pathname) ```
 `pathname` serves as a reference to either a single `.gpx` file or a directory.
 If a directory path is provided, all .gpx files contained within that directory
 will be merged, but retain their original metadata (e.g., different tracks
 remain separated). This allows users to overlay multiple tracks onto a single
 map, providing a comprehensive summary of the data being analyzed. ## Map
-creation ```python track.create_map(filename) ``` This generates an HTML file
-saved under `filename`, which contains an interactive map _(_e_x_a_m_p_l_e_). Each
+creation ```python track.create_map(filename) ``` * This generates an HTML file
+saved under `filename`, which contains an interactive map _(_e_x_a_m_p_l_e_). * Each
 segment of a track corresponds to the elevation relative to user's position:
-blue = lower elevation, yellow = higher elevation. Users can hover over routes
-or click on final waypoints (flags) for additional information: ![](https://
-github.com/JiaWeiTeh/gpx_vis/blob/main/media/track_info.png) Different
-backgrounds are available (selectable at lower-right corner): |Tile type |
-Example | |----------------------|-----------| |Dark | ![](https://github.com/
-JiaWeiTeh/gpx_vis/blob/main/media/ex_dark.png) | |Street view | ![](https://
-github.com/JiaWeiTeh/gpx_vis/blob/main/media/ex_openstreet.png) | |Plain | ![]
-(https://github.com/JiaWeiTeh/gpx_vis/blob/main/media/ex_plain.png) | |Plain
-(Heirarchical) | ![](https://github.com/JiaWeiTeh/gpx_vis/blob/main/media/
-ex_plainheir.png) | In cases where the map contains a large dataset and loading
-time is a concern (if one has been very hardworking), users have the option to
-include `lite = True`. By default, this option limits the number of data points
-displayed on each route to `nlite = 50`. However, users can adjust this limit
-using the `nlite` argument, for instance, ```python track.create_map(filename,
-lite=True, nlite=100) ``` Note that the minimum value for `nlite` is `10`. ##
-City overview ```python track.city_list ``` Interested in the cities you passed
-through on your journey? This command generates a list of cities - sorted by
-country and name - that were detected along the tour route. The `frequency`
-parameter indicates how many times each city was encountered, providing a rough
-estimate of the time spent in each city. ## Additional information If you wish
-to plot or inspect different values, these parameters are also accessible via:
-`track.t`: time (UTC)
-`track.x`: longitude (deg) - x values on a graph would represent the latitude.
-`track.y`: latitude (deg)
-`track.z`: elevation (m)
+blue = lower elevation, yellow = higher elevation. * Users can hover over
+routes or click on final waypoints (flags) for additional information: ![]
+(https://raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/track_info.png)
+Different backgrounds are available (selectable at lower-right corner): |Tile
+type | Example | |----------------------|-----------| |Dark | ![](https://
+raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/ex_dark.png) | |Street
+view | ![](https://raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/
+ex_openstreet.png) | |Plain | ![](https://raw.githubusercontent.com/JiaWeiTeh/
+gpx_vis/main/media/ex_plain.png) | |Plain (Heirarchical) | ![](https://
+raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/ex_plainheir.png) | In
+cases where the map contains a large dataset and loading time is a concern (if
+one has been very hardworking), users have the option to include `lite = True`.
+* By default, this option limits the number of data points displayed on each
+route to `nlite = 50`. This is adjustable using `nlite` argument: ```python
+track.create_map(filename, lite=True, nlite=100) ``` Note that the minimum
+value for `nlite` is `10`. ## City overview ```python track.city_list ```
+Interested in the cities you passed through on your journey? This command
+generates a list of cities - sorted by country and name - that were detected
+along the tour route. * The `frequency` parameter indicates how many times each
+city was encountered, providing a rough estimate of the time spent in each
+city. ## Additional information If you wish to plot or inspect different
+values, these parameters are also accessible via: * `track.t`: time (UTC)
+* `track.x`: longitude (deg) - x values on a graph would represent the
+latitude.
+* `track.y`: latitude (deg)
+* `track.z`: elevation (m)
 For a more comprehensive and unprocessed dataset, you can use: `track.data`:
-Returns a `pandas.DataFrame` with headers `['trackName', 'latitude',
-'longitude', 'elevation', 'time']` ## Dependencies (numpy) https://numpy.org/
+Returns all data in a `pandas.DataFrame` accessible format. ## Dependencies
+(numpy) https://numpy.org/
 (pandas) https://pandas.pydata.org/
 (altair) https://altair-viz.github.io/
 (branca) https://pypi.org/project/branca/
 (gpxpy) https://github.com/tkrajina/gpxpy
 (vincenty) https://pypi.org/project/vincenty/
 (folium) https://github.com/python-visualization/folium
 (humanfriendly) https://pypi.org/project/humanfriendly/
```

### Comparing `gpx_vis-0.3.5/README.md` & `gpx_vis-0.3.6/src/gpx_vis.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1 +1,143 @@
-### About `gpx_vis``gpx_vis` enables simple and convenient visualisation of your cycling and hiking tours, whether you're conquering mountain trails or cruising city streets.You can easily transform your .GPX files into interactive and informative visualizations - just make sure your file includes data for `latitude`, `longitude`, `elevation`, and `time`, and you're good to go! Whether you're using apps like <a href="https://www.komoot.com/" target="_blank">Komoot</a> and <a href="https://www.strava.com/" target="_blank">Strava</a>, or crafting tracks on platforms like <a href="https://gpx.studio/" target="_blank">gpx.studio</a>, `gpx_vis` has you covered.Important note: `gpx_vis` is still in its development phase, so expect more exciting features and enhancements down the trail. But in the meantime, buckle up and get ready to explore your adventures! :climbing::bicyclist:### Contents[Installation](#Install)<br>[How to use](#Instantiate)<br>* [Map creation](#Map-creation)* [City overview](#City-overview)* [Additional information](#Additional-information)## InstallInstalling `gpx_vis` is straightforward through <a href="https://pypi.org/project/gpx-vis/" target="_blank">PyPI</a>:```bashpip install gpx_vis```To update to the latest version (if applicable):```bashpip install gpx_vis --upgrade```## Instantiate```pythonfrom gpx_vis import Tracktrack = Track(pathname)````pathname` serves as a reference to either a single `.gpx` file or a directory.If a directory path is provided, all .gpx files contained within that directorywill be merged, but retain their original metadata (e.g., different tracks remain separated).This allows users to overlay multiple tracks onto a single map, providing a comprehensive summary of the data being analyzed.## Map creation```pythontrack.create_map(filename)```This generates an HTML file saved under `filename`, which contains an interactive map <a href="https://raw.githack.com/JiaWeiTeh/gpx_vis/main/example/map.html" target="_blank">(example)</a>.Each segment of a track corresponds to the elevation relative to user's position: blue = lower elevation, yellow = higher elevation. Users can hover over routes or click on final waypoints (flags) for additional information:![](https://github.com/JiaWeiTeh/gpx_vis/blob/main/media/track_info.png)Different backgrounds are available (selectable at lower-right corner):|Tile type             |  Example  ||----------------------|-----------||Dark |  ![](https://github.com/JiaWeiTeh/gpx_vis/blob/main/media/ex_dark.png) ||Street view | ![](https://github.com/JiaWeiTeh/gpx_vis/blob/main/media/ex_openstreet.png) ||Plain |  ![](https://github.com/JiaWeiTeh/gpx_vis/blob/main/media/ex_plain.png) ||Plain (Heirarchical) |  ![](https://github.com/JiaWeiTeh/gpx_vis/blob/main/media/ex_plainheir.png) |In cases where the map contains a large dataset and loading time is a concern (if onehas been very hardworking), users have the option to include `lite = True`. By default, this option limits the number of data points displayed on each route to `nlite = 50`. However, users can adjust thislimit using the `nlite` argument, for instance,```pythontrack.create_map(filename, lite=True, nlite=100)```Note that the minimum value for `nlite` is `10`.## City overview```pythontrack.city_list```Interested in the cities you passed through on your journey? This command generates a listof cities - sorted by country and name - that were detected along the tour route. The `frequency` parameter indicates how many times each city was encountered,providing a rough estimate of the time spent in each city.## Additional informationIf you wish to plot or inspect different values, these parameters are also accessible via:`track.t`: time (UTC)<br>`track.x`: longitude (deg) - x values on a graph would represent the latitude.<br> `track.y`: latitude (deg)<br>`track.z`: elevation (m)<br>For a more comprehensive and unprocessed dataset, you can use:`track.data`:  Returns a `pandas.DataFrame` with headers `['trackName', 'latitude', 'longitude', 'elevation', 'time']`## Dependencies(numpy) https://numpy.org/ <br>(pandas) https://pandas.pydata.org/ <br>(altair) https://altair-viz.github.io/ <br>(branca) https://pypi.org/project/branca/ <br>(gpxpy) https://github.com/tkrajina/gpxpy <br>(vincenty) https://pypi.org/project/vincenty/ <br>(folium) https://github.com/python-visualization/folium <br>(humanfriendly) https://pypi.org/project/humanfriendly/ <br>(reverse-geocode) https://pypi.org/project/reverse-geocode/ <br>
+Metadata-Version: 2.1
+Name: gpx_vis
+Version: 0.3.6
+Summary: Visualising your Komoot/Strava tours
+Author-email: Jia Wei Teh <jiaweiteh.astro@gmail.com>
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: folium
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: humanfriendly
+Requires-Dist: reverse_geocode
+Requires-Dist: matplotlib
+Requires-Dist: vincenty
+Requires-Dist: altair
+Requires-Dist: gpxpy
+
+### About `gpx_vis`
+
+Transforms your .GPX files into an interactive map, whether you're conquering mountain trails or cruising city streets.
+
+Whether you're using apps like <a href="https://www.komoot.com/" target="_blank">Komoot</a> and <a href="https://www.strava.com/" target="_blank">Strava</a>,
+ or crafting tracks on platforms like <a href="https://gpx.studio/" target="_blank">gpx.studio</a> - just make sure your 
+ file includes data for `latitude`, `longitude`, `elevation`, and `time`, and you're good to go!
+
+Important note: `gpx_vis` is still in its development phase, so expect more exciting features 
+and enhancements down the trail. But in the meantime, buckle up and get ready to explore your adventures! :climbing::bicyclist:
+
+
+### Contents
+[Installation](#Install)<br>
+[How to use](#Instantiate)<br>
+* [Map creation](#Map-creation)
+* [City overview](#City-overview)
+* [Additional information](#Additional-information)
+
+
+## Install
+
+
+Installing `gpx_vis` is straightforward through <a href="https://pypi.org/project/gpx-vis/" target="_blank">PyPI</a>:
+
+```bash
+pip install gpx_vis
+```
+
+To update to the latest version (if applicable):
+
+```bash
+pip install gpx_vis --upgrade
+```
+
+## Instantiate
+
+```python
+from gpx_vis import Track
+
+track = Track(pathname)
+```
+
+`pathname` serves as a reference to either a single `.gpx` file or a directory.
+If a directory path is provided, all .gpx files contained within that directory
+will be merged, but retain their original metadata (e.g., different tracks remain separated).
+
+This allows users to overlay multiple tracks onto a single map, 
+providing a comprehensive summary of the data being analyzed.
+
+## Map creation
+
+```python
+track.create_map(filename)
+```
+
+* This generates an HTML file saved under `filename`, which contains an interactive map <a href="https://raw.githack.com/JiaWeiTeh/gpx_vis/main/example/map.html" target="_blank">(example)</a>.
+
+* Each segment of a track corresponds to the elevation relative to user's position: blue = lower elevation, yellow = higher elevation. 
+
+* Users can hover over routes or click on final waypoints (flags) for additional information:
+
+![](https://raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/track_info.png)
+
+Different backgrounds are available (selectable at lower-right corner):
+
+|Tile type             |  Example  |
+|----------------------|-----------|
+|Dark |  ![](https://raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/ex_dark.png) |
+|Street view | ![](https://raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/ex_openstreet.png) |
+|Plain |  ![](https://raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/ex_plain.png) |
+|Plain (Heirarchical) |  ![](https://raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/ex_plainheir.png) |
+
+In cases where the map contains a large dataset and loading time is a concern (if one
+has been very hardworking), users have the option to include `lite = True`. 
+
+* By default, this option limits the number of data points displayed on each route to `nlite = 50`. This is adjustable using `nlite` argument:
+
+```python
+track.create_map(filename, lite=True, nlite=100)
+```
+
+Note that the minimum value for `nlite` is `10`.
+
+## City overview
+
+```python
+track.city_list
+```
+
+Interested in the cities you passed through on your journey? This command generates a list
+of cities - sorted by country and name - that were detected along the tour route. 
+
+* The `frequency` parameter indicates how many times each city was encountered, providing a rough estimate of the time spent in each city.
+
+
+## Additional information
+
+If you wish to plot or inspect different values, these parameters are also accessible via:
+
+* `track.t`: time (UTC)<br>
+* `track.x`: longitude (deg) - x values on a graph would represent the latitude.<br> 
+* `track.y`: latitude (deg)<br>
+* `track.z`: elevation (m)<br>
+
+For a more comprehensive and unprocessed dataset, you can use:
+
+`track.data`:  Returns all data in a `pandas.DataFrame` accessible format.
+
+
+## Dependencies
+(numpy) https://numpy.org/ <br>
+(pandas) https://pandas.pydata.org/ <br>
+(altair) https://altair-viz.github.io/ <br>
+(branca) https://pypi.org/project/branca/ <br>
+(gpxpy) https://github.com/tkrajina/gpxpy <br>
+(vincenty) https://pypi.org/project/vincenty/ <br>
+(folium) https://github.com/python-visualization/folium <br>
+(humanfriendly) https://pypi.org/project/humanfriendly/ <br>
+(reverse-geocode) https://pypi.org/project/reverse-geocode/ <br>
+
+
+
```

#### html2text {}

```diff
@@ -1,61 +1,66 @@
-### About `gpx_vis``gpx_vis` enables simple and convenient visualisation of
-your cycling and hiking tours, whether you're conquering mountain trails or
-cruising city streets.You can easily transform your .GPX files into interactive
-and informative visualizations - just make sure your file includes data for
-`latitude`, `longitude`, `elevation`, and `time`, and you're good to go!
-Whether you're using apps like _K_o_m_o_o_t and _S_t_r_a_v_a, or crafting tracks on
-platforms like _g_p_x_._s_t_u_d_i_o, `gpx_vis` has you covered.Important note: `gpx_vis`
-is still in its development phase, so expect more exciting features and
-enhancements down the trail. But in the meantime, buckle up and get ready to
-explore your adventures! :climbing::bicyclist:### Contents[Installation]
-(#Install)
+Metadata-Version: 2.1 Name: gpx_vis Version: 0.3.6 Summary: Visualising your
+Komoot/Strava tours Author-email: Jia Wei Teh
+gmail.com> Classifier: Programming Language :: Python :: 3 Classifier:
+Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: folium Requires-Dist:
+numpy Requires-Dist: pandas Requires-Dist: humanfriendly Requires-Dist:
+reverse_geocode Requires-Dist: matplotlib Requires-Dist: vincenty Requires-
+Dist: altair Requires-Dist: gpxpy ### About `gpx_vis` Transforms your .GPX
+files into an interactive map, whether you're conquering mountain trails or
+cruising city streets. Whether you're using apps like _K_o_m_o_o_t and _S_t_r_a_v_a, or
+crafting tracks on platforms like _g_p_x_._s_t_u_d_i_o - just make sure your file
+includes data for `latitude`, `longitude`, `elevation`, and `time`, and you're
+good to go! Important note: `gpx_vis` is still in its development phase, so
+expect more exciting features and enhancements down the trail. But in the
+meantime, buckle up and get ready to explore your adventures! :climbing::
+bicyclist: ### Contents [Installation](#Install)
 [How to use](#Instantiate)
-* [Map creation](#Map-creation)* [City overview](#City-overview)* [Additional
-information](#Additional-information)## InstallInstalling `gpx_vis` is
-straightforward through _P_y_P_I:```bashpip install gpx_vis```To update to the
-latest version (if applicable):```bashpip install gpx_vis --upgrade```##
-Instantiate```pythonfrom gpx_vis import Tracktrack = Track
-(pathname)````pathname` serves as a reference to either a single `.gpx` file or
-a directory.If a directory path is provided, all .gpx files contained within
-that directorywill be merged, but retain their original metadata (e.g.,
-different tracks remain separated).This allows users to overlay multiple tracks
-onto a single map, providing a comprehensive summary of the data being
-analyzed.## Map creation```pythontrack.create_map(filename)```This generates an
-HTML file saved under `filename`, which contains an interactive map
-_(_e_x_a_m_p_l_e_).Each segment of a track corresponds to the elevation relative to
-user's position: blue = lower elevation, yellow = higher elevation. Users can
-hover over routes or click on final waypoints (flags) for additional
-information:![](https://github.com/JiaWeiTeh/gpx_vis/blob/main/media/
-track_info.png)Different backgrounds are available (selectable at lower-right
-corner):|Tile type | Example ||----------------------|-----------||Dark | ![]
-(https://github.com/JiaWeiTeh/gpx_vis/blob/main/media/ex_dark.png) ||Street
-view | ![](https://github.com/JiaWeiTeh/gpx_vis/blob/main/media/
-ex_openstreet.png) ||Plain | ![](https://github.com/JiaWeiTeh/gpx_vis/blob/
-main/media/ex_plain.png) ||Plain (Heirarchical) | ![](https://github.com/
-JiaWeiTeh/gpx_vis/blob/main/media/ex_plainheir.png) |In cases where the map
-contains a large dataset and loading time is a concern (if onehas been very
-hardworking), users have the option to include `lite = True`. By default, this
-option limits the number of data points displayed on each route to `nlite =
-50`. However, users can adjust thislimit using the `nlite` argument, for
-instance,```pythontrack.create_map(filename, lite=True, nlite=100)```Note that
-the minimum value for `nlite` is `10`.## City
-overview```pythontrack.city_list```Interested in the cities you passed through
-on your journey? This command generates a listof cities - sorted by country and
-name - that were detected along the tour route. The `frequency` parameter
-indicates how many times each city was encountered,providing a rough estimate
-of the time spent in each city.## Additional informationIf you wish to plot or
-inspect different values, these parameters are also accessible via:`track.t`:
-time (UTC)
-`track.x`: longitude (deg) - x values on a graph would represent the latitude.
-`track.y`: latitude (deg)
-`track.z`: elevation (m)
-For a more comprehensive and unprocessed dataset, you can use:`track.data`:
-Returns a `pandas.DataFrame` with headers `['trackName', 'latitude',
-'longitude', 'elevation', 'time']`## Dependencies(numpy) https://numpy.org/
+* [Map creation](#Map-creation) * [City overview](#City-overview) * [Additional
+information](#Additional-information) ## Install Installing `gpx_vis` is
+straightforward through _P_y_P_I: ```bash pip install gpx_vis ``` To update to the
+latest version (if applicable): ```bash pip install gpx_vis --upgrade ``` ##
+Instantiate ```python from gpx_vis import Track track = Track(pathname) ```
+`pathname` serves as a reference to either a single `.gpx` file or a directory.
+If a directory path is provided, all .gpx files contained within that directory
+will be merged, but retain their original metadata (e.g., different tracks
+remain separated). This allows users to overlay multiple tracks onto a single
+map, providing a comprehensive summary of the data being analyzed. ## Map
+creation ```python track.create_map(filename) ``` * This generates an HTML file
+saved under `filename`, which contains an interactive map _(_e_x_a_m_p_l_e_). * Each
+segment of a track corresponds to the elevation relative to user's position:
+blue = lower elevation, yellow = higher elevation. * Users can hover over
+routes or click on final waypoints (flags) for additional information: ![]
+(https://raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/track_info.png)
+Different backgrounds are available (selectable at lower-right corner): |Tile
+type | Example | |----------------------|-----------| |Dark | ![](https://
+raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/ex_dark.png) | |Street
+view | ![](https://raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/
+ex_openstreet.png) | |Plain | ![](https://raw.githubusercontent.com/JiaWeiTeh/
+gpx_vis/main/media/ex_plain.png) | |Plain (Heirarchical) | ![](https://
+raw.githubusercontent.com/JiaWeiTeh/gpx_vis/main/media/ex_plainheir.png) | In
+cases where the map contains a large dataset and loading time is a concern (if
+one has been very hardworking), users have the option to include `lite = True`.
+* By default, this option limits the number of data points displayed on each
+route to `nlite = 50`. This is adjustable using `nlite` argument: ```python
+track.create_map(filename, lite=True, nlite=100) ``` Note that the minimum
+value for `nlite` is `10`. ## City overview ```python track.city_list ```
+Interested in the cities you passed through on your journey? This command
+generates a list of cities - sorted by country and name - that were detected
+along the tour route. * The `frequency` parameter indicates how many times each
+city was encountered, providing a rough estimate of the time spent in each
+city. ## Additional information If you wish to plot or inspect different
+values, these parameters are also accessible via: * `track.t`: time (UTC)
+* `track.x`: longitude (deg) - x values on a graph would represent the
+latitude.
+* `track.y`: latitude (deg)
+* `track.z`: elevation (m)
+For a more comprehensive and unprocessed dataset, you can use: `track.data`:
+Returns all data in a `pandas.DataFrame` accessible format. ## Dependencies
+(numpy) https://numpy.org/
 (pandas) https://pandas.pydata.org/
 (altair) https://altair-viz.github.io/
 (branca) https://pypi.org/project/branca/
 (gpxpy) https://github.com/tkrajina/gpxpy
 (vincenty) https://pypi.org/project/vincenty/
 (folium) https://github.com/python-visualization/folium
 (humanfriendly) https://pypi.org/project/humanfriendly/
```

### Comparing `gpx_vis-0.3.5/pyproject.toml` & `gpx_vis-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpx_vis"
-version = "0.3.5"
+version = "0.3.6"
 authors = [
   { name="Jia Wei Teh", email="jiaweiteh.astro@gmail.com" },
 ]
 description = "Visualising your Komoot/Strava tours"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `gpx_vis-0.3.5/src/gpx_vis.py` & `gpx_vis-0.3.6/src/gpx_vis.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,14 @@
         print('Here are the cities you passed through on your journey.')
         return sorted(unique_city_list)
     
     # =============================================================================
     # Track handling
     # =============================================================================
     
-    @staticmethod
     def idx_trksplit(self):
         """
         Index at which we enter a new track entry (if any).
         Note: x -> x[i,j], x[k+1, l]. See plt_tracks().
         """
         idx_list =  np.where(self.name[:-1] != self.name[1:])[0]
         # we provide list of indices at which tracks separate.
@@ -250,18 +249,18 @@
         main_map = folium.Map(location = map_center)
         # specify border.
         main_map.fit_bounds([map_sw, map_ne])
         
         # create group
         lineGroup = folium.FeatureGroup(name = "Your Routes")
         # plot waypoints for each end and beginning of a track
-        idx_split_list = self.idx_trksplit(self)
+        idx_split_list = self.idx_trksplit()
         # if list is empty, there is no splitting tracks
         for selected_idx in idx_split_list:
-            self._addTracksOnMap(self, lineGroup, selected_idx, lite, **kwargs)
+            self._addTracksOnMap(lineGroup, selected_idx, lite, **kwargs)
             
         # clusters
         cluster = MarkerCluster().add_to(main_map)
         # add group to map
         lineGroup.add_to(cluster)
         
         # add different backgrounds
@@ -281,15 +280,14 @@
         if not filename.endswith(".html"):
             filename += '.html'
         main_map.save(filename)
         # show time
         _timer.end()
         return print(f"File saved as {filename}.")
     
-    @staticmethod
     def _addTracksOnMap(self, group, selected_idx, lite, **kwargs):
         """
         This function adds individual tracks onto create_map().
         group: FeatureGroup this track belongs to.
         selected_idx: index range of this particular track.
         """
         ii, jj = selected_idx
@@ -307,21 +305,21 @@
         else:
             nPoints = int((jj-ii)/max_nPoints)
         
             
         track_coords = list(zip(self.y[ii:jj:nPoints], self.x[ii:jj:nPoints]))
         # information frame        
         # iframe = folium.IFrame(popupTxt)
-        elevation_graph = self._addPopupGraph(self, selected_idx)
+        elevation_graph = self._addPopupGraph(selected_idx)
         # create popup
         popup = folium.Popup(min_width=400,
                              max_width=400)
         elevation_graph.add_to(popup)
         # add tooltip
-        tooltip = self._addTooltip(self, selected_idx)
+        tooltip = self._addTooltip(selected_idx)
         # add to group
         # since elevation sometimes differ widly, perhaps it is better to use 
         # log-scale as a simple fix. (as long as there aren't zero entries)
         # Right now, I am using individual tracks for individual colorbar min/max. Can of course
         # switch to map-wide colorbar by removing [ii:jj]
         folium.ColorLine(track_coords,
                         colors = self.z[ii:jj:nPoints],
@@ -361,15 +359,14 @@
                 control=False,
                 tooltip = tooltip,
                 weight = 25, #transparent layer easier to highlight
                 highlight_function=highlight_function, 
                 ).add_to(group)
         return  
       
-    @staticmethod
     def _addPopuptxt(self, selected_idx):
         """
         Creates str-block that contains useful info.
         """
         # index range
         ii, jj = selected_idx
         # track name
@@ -398,15 +395,14 @@
         title = f'{track_name}'
         subtitle1 = f"""Start: {track_t[0].strftime('%d.%m.%Y %H:%M:%S')} (UTC), {startCity}"""
         subtitle2 = f"""End: {track_t[-1].strftime('%d.%m.%Y %H:%M:%S')} (UTC), {endCity}"""
         subtitle3 = f'Total: {dist} km, {timeElapsed}'
                  
         return title, subtitle1, subtitle2, subtitle3
     
-    @staticmethod
     def _addPopupGraph(self, selected_idx):
         """
         Creates elevation graph in Popup text.
         """
         ii, jj = selected_idx
         # create figure with Method-based Syntax.
         # https://altair-viz.github.io/user_guide/encodings/index.html
@@ -414,15 +410,15 @@
         max_nPoints = 100
         if (jj-ii) < max_nPoints:
             nPoints = 1
         else:
             nPoints = int((jj-ii)/max_nPoints)
         
         # titles
-        title, subtitle1, subtitle2, subtitle3 = self._addPopuptxt(self, selected_idx)
+        title, subtitle1, subtitle2, subtitle3 = self._addPopuptxt(selected_idx)
         # plot
         lineplot = alt.Chart(self.data[['time', 'elevation']][ii:jj:nPoints],
                                  title = alt.Title(  title, 
                                                      subtitle = [subtitle1, subtitle2, subtitle3])
                                                    )\
                             .mark_line()\
                             .encode(
@@ -440,15 +436,14 @@
                             lineplot,
                             width=300,
                             height=300,
                             )
         return elevation_graph
     
     
-    @staticmethod
     def _addTooltip(self, selected_idx):
         """
         Creates str-block that contains tooltip when mouse is hovered over the track.
         """
         ii, jj = selected_idx
         track_name = self.name[ii]
         infostr = f"Route: {track_name}"
```

