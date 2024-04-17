# Comparing `tmp/svinsight-0.2.7.tar.gz` & `tmp/svinsight-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svinsight-0.2.7.tar", last modified: Fri Apr 12 19:06:53 2024, max compression
+gzip compressed data, was "svinsight-0.2.8.tar", last modified: Wed Apr 17 20:29:12 2024, max compression
```

## Comparing `svinsight-0.2.7.tar` & `svinsight-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-12 19:06:53.496403 svinsight-0.2.7/
--rw-r--r--   0 matthewpreisser   (501) staff       (20)     1073 2024-04-12 14:13:08.000000 svinsight-0.2.7/LICENSE
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      751 2024-04-12 19:06:53.496180 svinsight-0.2.7/PKG-INFO
--rw-r--r--   0 matthewpreisser   (501) staff       (20)       93 2024-04-10 20:46:54.000000 svinsight-0.2.7/README.md
-drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-12 19:06:53.493473 svinsight-0.2.7/SVInsight/
--rw-r--r--   0 matthewpreisser   (501) staff       (20)       39 2024-04-12 19:05:30.000000 svinsight-0.2.7/SVInsight/__init__.py
--rw-r--r--   0 matthewpreisser   (501) staff       (20)    17061 2024-04-10 20:33:03.000000 svinsight-0.2.7/SVInsight/census_variables.py
--rw-r--r--   0 matthewpreisser   (501) staff       (20)    57504 2024-04-12 19:00:20.000000 svinsight-0.2.7/SVInsight/svi.py
-drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-12 19:06:53.495945 svinsight-0.2.7/SVInsight.egg-info/
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      751 2024-04-12 19:06:53.000000 svinsight-0.2.7/SVInsight.egg-info/PKG-INFO
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      462 2024-04-12 19:06:53.000000 svinsight-0.2.7/SVInsight.egg-info/SOURCES.txt
--rw-r--r--   0 matthewpreisser   (501) staff       (20)        1 2024-04-12 19:06:53.000000 svinsight-0.2.7/SVInsight.egg-info/dependency_links.txt
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      118 2024-04-12 19:06:53.000000 svinsight-0.2.7/SVInsight.egg-info/requires.txt
--rw-r--r--   0 matthewpreisser   (501) staff       (20)       10 2024-04-12 19:06:53.000000 svinsight-0.2.7/SVInsight.egg-info/top_level.txt
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      733 2024-04-12 19:05:30.000000 svinsight-0.2.7/pyproject.toml
--rw-r--r--   0 matthewpreisser   (501) staff       (20)       38 2024-04-12 19:06:53.496446 svinsight-0.2.7/setup.cfg
--rw-r--r--   0 matthewpreisser   (501) staff       (20)      782 2024-04-12 19:05:28.000000 svinsight-0.2.7/setup.py
-drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-12 19:06:53.495694 svinsight-0.2.7/tests/
--rw-r--r--   0 matthewpreisser   (501) staff       (20)       73 2024-04-12 15:53:21.000000 svinsight-0.2.7/tests/test_svinsight.py
+drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-17 20:29:12.527010 svinsight-0.2.8/
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)     1073 2024-04-12 14:13:08.000000 svinsight-0.2.8/LICENSE
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)      783 2024-04-17 20:29:12.526720 svinsight-0.2.8/PKG-INFO
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)      208 2024-04-15 14:32:42.000000 svinsight-0.2.8/README.md
+drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-17 20:29:12.524908 svinsight-0.2.8/SVInsight/
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)       57 2024-04-17 20:16:27.000000 svinsight-0.2.8/SVInsight/__init__.py
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)    17061 2024-04-15 15:22:19.000000 svinsight-0.2.8/SVInsight/census_variables.py
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)    59348 2024-04-17 19:36:33.000000 svinsight-0.2.8/SVInsight/svi.py
+drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-17 20:29:12.526498 svinsight-0.2.8/SVInsight.egg-info/
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)      783 2024-04-17 20:29:12.000000 svinsight-0.2.8/SVInsight.egg-info/PKG-INFO
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)      462 2024-04-17 20:29:12.000000 svinsight-0.2.8/SVInsight.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)        1 2024-04-17 20:29:12.000000 svinsight-0.2.8/SVInsight.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)      135 2024-04-17 20:29:12.000000 svinsight-0.2.8/SVInsight.egg-info/requires.txt
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)       10 2024-04-17 20:29:12.000000 svinsight-0.2.8/SVInsight.egg-info/top_level.txt
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)      757 2024-04-17 20:29:09.000000 svinsight-0.2.8/pyproject.toml
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)       38 2024-04-17 20:29:12.527068 svinsight-0.2.8/setup.cfg
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)      828 2024-04-17 20:28:31.000000 svinsight-0.2.8/setup.py
+drwxr-xr-x   0 matthewpreisser   (501) staff       (20)        0 2024-04-17 20:29:12.526371 svinsight-0.2.8/tests/
+-rw-r--r--   0 matthewpreisser   (501) staff       (20)     6769 2024-04-17 19:36:33.000000 svinsight-0.2.8/tests/test_svinsight.py
```

### Comparing `svinsight-0.2.7/LICENSE` & `svinsight-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `svinsight-0.2.7/PKG-INFO` & `svinsight-0.2.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: SVInsight
-Version: 0.2.7
+Version: 0.2.8
 Summary: Create social vulnerabilty index
 Home-page: https://github.com/mdp0023/SVInsight/
 Author: M. Preisser, P. Passalacqua, R. P. Bixler
 Author-email: Matthew Preisser <mattpreisser@gmail.com>
 Project-URL: Homepage, https://example.com
 Project-URL: Documentation, https://readthedocs.org
 Keywords: SVI
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: census==0.8.21
-Requires-Dist: factor_analyzer==0.5.1
-Requires-Dist: geopandas==0.14.2
-Requires-Dist: numpy==1.26.4
-Requires-Dist: pandas==2.2.2
-Requires-Dist: PyYAML==6.0.1
-Requires-Dist: scikit_learn==1.3.0
+Requires-Dist: census>=0.8.21
+Requires-Dist: factor_analyzer>=0.5.1
+Requires-Dist: geopandas>=0.14.2
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: pandas>=2.2.2
+Requires-Dist: PyYAML>=6.0.1
+Requires-Dist: scikit_learn>=1.3.0
+Requires-Dist: openpyxl>=3.0.10
```

### Comparing `svinsight-0.2.7/SVInsight/census_variables.py` & `svinsight-0.2.8/SVInsight/census_variables.py`

 * *Files identical despite different names*

### Comparing `svinsight-0.2.7/SVInsight/svi.py` & `svinsight-0.2.8/SVInsight/svi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 
 import os 
 import csv
 import copy
 import shutil
 import zipfile
 import numpy as np
+import requests
 import pandas as pd
 from ftplib import FTP
+import ftputil
 import geopandas as gpd
 from census import Census
 import concurrent.futures
 from concurrent.futures import ThreadPoolExecutor
 from sklearn.preprocessing import MinMaxScaler
 from factor_analyzer import FactorAnalyzer
 import yaml
@@ -28,15 +30,15 @@
 
 
 
 class SVInsight:
     """A class to calculate a Social Vulnerability Index."""
 
     @staticmethod
-    def validate_value(value, valid_options, value_name):
+    def _validate_value(value, valid_options, value_name):
         """
         Validates a value against a list of valid options.
 
         Args:
             value (Any): The value to be validated.
             valid_options (List[Any]): A list of valid options.
             value_name (str): The name of the value being validated.
@@ -48,15 +50,15 @@
             None
         """
         if value not in valid_options:
             options_str = ', '.join(valid_options)
             raise ValueError(f"Invalid {value_name}. Must be one of: {options_str}.")
         
     @staticmethod
-    def validate_format(value, type, value_name):
+    def _validate_format(value, type, value_name):
         """
         Validates the format of a given value.
 
         Parameters:
         value (any): The value to be validated.
         type (type): The expected type of the value.
         value_name (str): The name of the value being validated.
@@ -67,49 +69,51 @@
         Returns:
         None
         """
         if not isinstance(value, type):
             raise TypeError(f"Invalid {value_name}. Must be type {type}.")
 
     @staticmethod
-    def geoid_format(geoids):
+    def _geoid_format(geoids):
         """
         Validates the format of a list of GEOIDs.
 
         Args:
             geoids (list): A list of GEOIDs to be validated. Each GEOID must be length 2 or 5.
 
         Raises:
             ValueError: If the GEOIDs are not all of the same length, either 2 or 5.
 
         Returns:
             None
         """
+        for geoid in geoids:
+            if  geoid is int:
+                raise ValueError('All GEOIDS must be string.')
         lengths = {len(geoid) for geoid in geoids}
         if len(lengths) > 1 or (list(lengths)[0] not in [2, 5]):
             raise ValueError("All GEOIDs must be of the same length, either 2 or 5.")
                 
 
     def __init__(self, project_name: str, file_path: str, api_key: str, geoids: list[str]):
         """
         Initialize the SVInsight class.
 
-        Parameters:
-        - project_name (str): The name of the project. Will be used in file structure and names of saved files.
-        - file_path (str): The file path where the project will be saved.
-        - api_key (str): The Census API key for accessing data.
-        - geoids (list[str]): A list of geographic identifiers. Must all be either length 2 or 5.
-        
-
-        Raises:
-        - FileNotFoundError: If the file path does not exist.
-        - ValueError: If the GEOIDs are not all of the same length, either 2 or 5.
-        - TypeError: If a value is not of the expected type.
-
-
+        :param project_name: The name of the project. Will be used in file structure and names of saved files.
+        :type project_name: str
+        :param file_path: The file path where the project will be saved.
+        :type file_path: str
+        :param api_key: The Census API key for accessing data.
+        :type api_key: str
+        :param geoids: A list of geographic identifiers. Must all be either length 2 or 5.
+        :type geoids: list[str]
+
+        :raises FileNotFoundError: If the file path does not exist.
+        :raises ValueError: If the GEOIDs are not all of the same length, either 2 or 5.
+        :raises TypeError: If a value is not of the expected type.
         """
         # Determine if file path exists
         if not os.path.exists(file_path):
             raise FileNotFoundError(f"File path '{file_path}' does not exist.")
         
         # Set variable instances (inputs)
         self.project_name = project_name
@@ -121,58 +125,61 @@
         self.low_pop_filter = 75        # boundaries to exlude 
         self.min_iterp_neighbors = 40   # minimum number of neighbors needed to interpolate holes
 
         # setup instances of Census variables
         self.all_vars_eqs, self.all_vars = setup_census_variables()
 
         # Validate Variables
-        self.validate_format(project_name, str, 'project_name')
-        self.validate_format(file_path, str, 'file_path')
-        self.validate_format(api_key, str, 'api_key')
-        self.validate_format(geoids, list, 'geoids')
-        self.geoid_format(geoids)
+        self._validate_format(project_name, str, 'project_name')
+        self._validate_format(file_path, str, 'file_path')
+        self._validate_format(api_key, str, 'api_key')
+        self._validate_format(geoids, list, 'geoids')
+        self._geoid_format(geoids)
 
         # Create file structure
         os.makedirs(self.file_path, exist_ok=True)
         folders = ['Boundaries','Variables', 'Data', 'Documentation', 'SVIs']
         for folder in folders:
             os.makedirs(os.path.join(self.file_path, folder), exist_ok=True)
             self.__dict__[folder.lower()] = os.path.join(self.file_path, folder)
 
         
     ###################################################
     # PUBLIC METHODS
     ###################################################
 
     # Method to pull block groups or tract shapefiles
-    def boundaries_data(self, boundary: str = 'bg', year: int = 2019) -> gpd.GeoDataFrame:
+    def boundaries_data(self, boundary: str = 'bg', year: int = 2019, overwrite: bool = False) -> gpd.GeoDataFrame:
         """
         Pulls block group or tract data from the Census FTP site.
 
-        Args:
-            boundary (str): The type of boundary. Defaults to 'bg'. Acceptable values are 'bg', or 'tract'.
-            year (str): The year of the data. Defaults to '2019'.
+        :param boundary: The type of boundary. Defaults to 'bg'. Acceptable values are 'bg', or 'tract'.
+        :type boundary: str
+        :param year: The year of the data. Defaults to '2019'.
+        :type year: int
+        :param overwrite: whether or not to overwrite an existing geopackage if it exists. Default is False
+        :type overwrite: bool
 
-        Returns:
-            gpd.GeoDataFrame: The boundary data as a GeoDataFrame.
+        :return: The boundary data as a GeoDataFrame.
+        :rtype: gpd.GeoDataFrame
 
-        Raises:
-            ValueError: If the boundary type is invalid, the year is not between 2010 and 2022, or geoids not properly formated.
+        :raises ValueError: If the boundary type is invalid, the year is not between 2010 and 2022, or geoids not properly formatted.
         """
         
         # Validate Variables
-        self.validate_value(boundary, ['bg', 'tract'], 'boundary')
-        self.validate_value(year, [2010, 2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022], 'year')
-        self.validate_format(boundary, str, 'boundary')
-        self.validate_format(year, int, 'year')
+        self._validate_value(boundary, ['bg', 'tract'], 'boundary')
+        self._validate_value(year, [2010, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022], 'year')
+        self._validate_format(boundary, str, 'boundary')
+        self._validate_format(year, int, 'year')
 
 
         # If shapefile already exists, pass 
-        if os.path.exists(os.path.join(self.boundaries, f"{self.project_name}_{year}_{boundary}.gpkg")):
-            pass
+        if os.path.exists(os.path.join(self.boundaries, f"{self.project_name}_{year}_{boundary}.gpkg")) and overwrite is False:
+            
+            return gpd.read_file(os.path.join(self.boundaries, f"{self.project_name}_{year}_{boundary}.gpkg"))
         else:
 
             # create final output geodataframe
             output = gpd.GeoDataFrame()
 
             # helper functions
             def _download(year, state, boundary):
@@ -183,44 +190,65 @@
                     year (int): The year of the shapefile.
                     state (str): The state abbreviation.
                     boundary (str): The boundary type. Must be 'bg' or 'tract'
 
                 Returns:
                     geopandas.GeoDataFrame: The boundary shapefile as a GeoDataFrame.
                 """
+               
 
                 # create filenames
                 filename = f"cb_{year}_{state}_{boundary}_500k"
                 filename_dir = os.path.join(self.boundaries, filename)
                 zipped_filename = f"{filename}.zip"
                 zipped_dir = os.path.join(self.boundaries, zipped_filename)
-
                 os.makedirs(filename_dir, exist_ok=True)
-                # Open the file locally and write it to folder
-                with open(zipped_dir, "wb") as file:
-                    ftp.retrbinary(f"RETR {zipped_filename}", file.write)
+                
+                #  # initiate FTP
+                # ftp = FTP('ftp2.census.gov')
+                # ftp.login()
+                # ftp.cwd(f'geo/tiger/GENZ{year}/shp/')
+
+                # # Open the file locally and write it to folder
+                # print('opening binary')
+                # with open(zipped_dir, "wb") as file:
+                #     ftp.retrbinary(f"RETR {zipped_filename}", file.write)
+                # print('opened binary')
+
+                # Specify the URL of the file you want to download
+                url = f"https://www2.census.gov/geo/tiger/GENZ{year}/shp/{zipped_filename}"
+
+                # Send a GET request to the URL
+                response = requests.get(url, stream=True)
+
+                # Check if the request was successful
+                if response.status_code == 200:
+                    # Open a local file with the same name as the remote file
+                    with open(zipped_dir, 'wb') as file:
+                        # Write the contents of the remote file to the local file
+                        for chunk in response.iter_content(chunk_size=1024):
+                            if chunk:
+                                file.write(chunk)
+
 
                 # Unzip the file
-                with zipfile.ZipFile(f"{zipped_dir}", 'r') as zip_ref:
-                    zip_ref.extractall(filename_dir)
+                shutil.unpack_archive(zipped_dir, filename_dir)
+                # with zipfile.ZipFile(f"{zipped_dir}", 'r') as zip_ref:
+                #     zip_ref.extractall(filename_dir)
 
                 # Read the shapefile with geopandas
                 boundary_shp = gpd.read_file(f"{filename_dir}/{filename}.shp")
 
 
                 # remove the zipped and unzipped files
                 os.remove(zipped_dir)
                 shutil.rmtree(filename_dir)
 
                 return boundary_shp
 
-            # initiate FTP
-            ftp = FTP('ftp2.census.gov')
-            ftp.login()
-            ftp.cwd(f'geo/tiger/GENZ{year}/shp/')
 
             # determine if we are pulling states or subset of counties 
             if len(self.geoids[0]) == 2:
                 for geoid in self.geoids:
                     boundary_shp = _download(year, geoid, boundary)
 
                     # Concatenate output
@@ -253,46 +281,49 @@
                     # Concatenate output and subset
                     output = pd.concat([output, subset], axis=0, join='outer')
 
             # Save the output to a new folder
             output.to_file(os.path.join(self.boundaries, f"{self.project_name}_{year}_{boundary}.gpkg"))
 
             # Quit the FTP client
-            ftp.quit()
+            #ftp.quit()
 
             return output
     
 
     # Method to pull census data and fill holes
     def census_data(self, boundary: str = 'bg', year: int = 2019, interpolate: bool = True, verbose: bool = False, overwrite: bool = False):
-        '''
+        """
         Pulls Census data for a specific boundary and year.
 
-        Parameters:
-            boundary (str): The boundary type to retrieve data for. Valid options are 'bg' (block group) and 'tract' (census tract).
-            year (int): The year of the Census data to retrieve. Valid options are from 2010 to 2022.
-            interpolate (bool, optional): Whether to interpolate missing data. Defaults to True.
-            verbose (bool, optional): Whether to display verbose output. Defaults to False.
-            overwrite (bool, optional): Whether to overwrite existing data. Defaults to False.
+        :param boundary: The boundary type to retrieve data for. Valid options are 'bg' (block group) and 'tract' (census tract).
+        :type boundary: str
+        :param year: The year of the Census data to retrieve. Valid options are from 2010 to 2022.
+        :type year: int
+        :param interpolate: Whether to interpolate missing data. Defaults to True.
+        :type interpolate: bool, optional
+        :param verbose: Whether to display verbose output. Defaults to False.
+        :type verbose: bool, optional
+        :param overwrite: Whether to overwrite existing data. Defaults to False.
+        :type overwrite: bool, optional
 
-        Raises:
-            ValueError: If the boundary type is invalid or the year is not between 2010 and 2022.
-            FileNotFoundError: If the shapefile for the specified boundary and year does not exist.
+        :raises ValueError: If the boundary type is invalid or the year is not between 2010 and 2022.
+        :raises FileNotFoundError: If the shapefile for the specified boundary and year does not exist.
 
-        Returns:
-            None
-        '''
+        :return: None
+        :rtype: None
+        """
         # Validate Variables
-        self.validate_value(boundary, ['bg', 'tract'], 'boundary')
-        self.validate_value(year, [2010, 2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022], 'year')
-        self.validate_format(boundary, str, 'boundary')
-        self.validate_format(year, int, 'year')
+        self._validate_value(boundary, ['bg', 'tract'], 'boundary')
+        self._validate_value(year, [2010, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022], 'year')
+        self._validate_format(boundary, str, 'boundary')
+        self._validate_format(year, int, 'year')
 
         # If data already exists and overwrite is False, don't pull data 
-        if os.path.join(self.data, f"{self.project_name}_{year}_{boundary}_rawdata.gpkg") and overwrite is False:
+        if os.path.exists(os.path.join(self.data, f"{self.project_name}_{year}_{boundary}_rawdata.gpkg")) and overwrite is False:
             pass
         else:
 
             # check if shapefile exists
             if not os.path.exists(os.path.join(self.boundaries, f"{self.project_name}_{year}_{boundary}.gpkg")):
                 raise FileNotFoundError(f"{self.project_name}_{year}_{boundary}.gpkg not found. Run boundaries_data method prior to census_data.")
             else:
@@ -329,60 +360,63 @@
 
 
     # Method to inspect variable descriptions
     def var_descriptions(self, vars: list = None):
         """
         Print the descriptions of the variables.
 
-        Args:
-            vars (list): Optional. List of variables to print descriptions for. If not provided, descriptions for all variables will be printed.
+        :param vars: Optional. List of variables to print descriptions for. If not provided, descriptions for all variables will be printed.
+        :type vars: list
 
-        Raises:
-            ValueError: If any variable in `vars` is not an available variable.
+        :raises ValueError: If any variable in `vars` is not an available variable.
 
-        Returns:
-            None
+        :return: None
+        :rtype: None
         """
 
         # Raise exception if var in vars not an available variable
         if vars is not None:
             for var in vars:
-                self.validate_value(var, list(self.all_vars_eqs.keys()), var)
+                self._validate_value(var, list(self.all_vars_eqs.keys()), var)
 
         if vars is None:
             vars = list(self.all_vars_eqs.keys())
         for var in vars:
             print(f"{var}: {self.all_vars_eqs[var]['description']}")
         
 
     # Method to add a variable
     def add_variable(self, boundary: str, year: int, name:str, num: list, den: list = [1], description: str = None):
         """
         Add additional variable and collect necessary raw data. 
         
-        Args:
-            boundary (str): The boundary type for the variable. Should be either 'bg' or 'tract'.
-            year (int): The year for which the raw data is collected.
-            name (str): The name of the variable.
-            num (list): The list of numerator variables used to calculate the variable.
-            den (list): The list of denominator variables used to calculate the variable. Default is [1].
-            description (str): Optional description of the variable. Default is None.
+        :param boundary: The boundary type for the variable. Should be either 'bg' or 'tract'.
+        :type boundary: str
+        :param year: The year for which the raw data is collected.
+        :type year: int
+        :param name: The name of the variable.
+        :type name: str
+        :param num: The list of numerator variables used to calculate the variable.
+        :type num: list
+        :param den: The list of denominator variables used to calculate the variable. Default is [1].
+        :type den: list, optional
+        :param description: Optional description of the variable. Default is None.
+        :type description: str, optional
+        
+        :raises ValueError: If the variable name already exists.
+        :raises ValueError: If the boundary type is invalid or the year is not between 2010 and 2022.
+        :raises FileNotFoundError: If the raw data file doesn't exist. Run the census_data method first.
         
-        Raises:
-            ValueError: If the variable name already exists.
-             ValueError: If the boundary type is invalid or the year is not between 2010 and 2022.
-            FileNotFoundError: If the raw data file doesn't exist. Run the census_data method first.
-        
-        Returns:
-            None
+        :return: None
+        :rtype: None
         """
         
         # Validate Variables
-        self.validate_value(boundary, ['bg', 'tract'], 'boundary')
-        self.validate_value(year, [2010, 2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022], 'year')
+        self._validate_value(boundary, ['bg', 'tract'], 'boundary')
+        self._validate_value(year, [2010, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022], 'year')
         
         # if name of variable already exists, raise error
         if name in self.all_vars_eqs:
             raise ValueError(f"Variable '{name}' already exists.")
 
         # open the raw data file as a df 
         if not os.path.exists(os.path.join(self.data, f"{self.project_name}_{year}_{boundary}_rawdata.gpkg")):
@@ -430,47 +464,46 @@
             data_df = self._fill_holes(data_df, boundary, self.geoids, self.api_key, year, interpolate=True, verbose=False)
 
             data_df.to_csv(os.path.join(self.data, f"{self.project_name}_{year}_{boundary}_rawdata.csv"))
             data_df.to_file(os.path.join(self.data, f"{self.project_name}_{year}_{boundary}_rawdata.gpkg"))
 
 
     # Method to create a configuration file before calculating SVI
-    def configure_variables(self, config_file: str , exclude: list = None, include: list = None, inverse_vars = ['PERCAP' , 'QRICH', 'MDHSEVAL']):
+    def configure_variables(self, config_file: str, exclude: list = None, include: list = None, inverse_vars: list = ['PERCAP', 'QRICH', 'MDHSEVAL']):
         """
-        Configure variables and save them to a YAML file. Can either exclude variables with exclude argument, or only include specific variables with include argument. 
-
-        Args:
-            config_name (str, optional): The name of the configuration file. 
-            exclude (list, optional): A list of variable names to exclude for the configuration. Defaults to None.
-            include (list, optional): A list of variable names to only include for the configuration. Defaults to None. 
-
-        Returns:
-            None
-
-        Raises:
-            ValueError: If `exclude` and `include` arguments are both passed.
-            ValueError: If a variable in the `exclude` list is not available in `self.all_vars_eqs`.
-            ValueError: If a variable in the `include` list is not available in `self.all_vars_eqs`.
-
+        Configure variables and save them to a YAML file.
 
+        :param config_file: The name of the configuration file.
+        :type config_file: str
+        :param exclude: Optional. A list of variable names to exclude for the configuration. Defaults to None.
+        :type exclude: list, optional
+        :param include: Optional. A list of variable names to only include for the configuration. Defaults to None.
+        :type include: list, optional
+        :param inverse_vars: Optional. A list of variable names to be inverted. Defaults to ['PERCAP', 'QRICH', 'MDHSEVAL'].
+        :type inverse_vars: list, optional
+
+        :returns: None
+        :raises ValueError: If `exclude` and `include` arguments are both passed.
+        :raises ValueError: If a variable in the `exclude` list is not available in `self.all_vars_eqs`.
+        :raises ValueError: If a variable in the `include` list is not available in `self.all_vars_eqs`.
         """
         # raise error if exclude and include are both not none
         if (exclude is not None) and (include is not None):
             raise ValueError("Both exclude and include arguments cannot be passed.")
 
         output_dict = copy.deepcopy(self.all_vars_eqs)
 
         if exclude is not None:
             for key in exclude:
-                self.validate_value(key, list(self.all_vars_eqs.keys()), key)
+                self._validate_value(key, list(self.all_vars_eqs.keys()), key)
                 del output_dict[key]
         
         if include is not None:
             for key in include:
-                self.validate_value(key, list(self.all_vars_eqs.keys()), key)
+                self._validate_value(key, list(self.all_vars_eqs.keys()), key)
             for key in list(output_dict.keys()):
                 if key not in include:
                     del output_dict[key]
 
 
         with open(os.path.join(self.variables, f"{config_file}.yaml"), 'w') as file:
             yaml.dump(inverse_vars, file)
@@ -479,48 +512,49 @@
 
     
     # Method to calculate SVI -> input yaml file to determine what variables are included and how they are calculated  
     def calculate_svi(self, config_file: str, boundary: str = 'bg', year: int = 2019):
         """
         Calculate the Social Vulnerability Index (SVI) using two different methods.
 
-        Args:
-            config_file (str): The name of the configuration file (without the extension) containing the SVI variables.
-            boundary (str): The boundary type for the SVI calculation. Default is 'bg'.
-            year (int): The year for which the SVI is calculated. Default is 2019.
+        :param config_file: The name of the configuration file (without the extension) containing the SVI variables.
+        :type config_file: str
+        :param boundary: The boundary type for the SVI calculation. Default is 'bg'.
+        :type boundary: str
+        :param year: The year for which the SVI is calculated. Default is 2019.
+        :type year: int
 
-        Returns:
-            None
-        
-        Raises:
-            ValueError: If the boundary type is invalid or the year is not between 2010 and 2022,
+        :returns: None
+        :raises ValueError: If the boundary type is invalid or the year is not between 2010 and 2022,
 
         This method reads a configuration file in YAML format, loads the raw data as a dataframe,
         calculates the SVI using two different methods, and saves the results to output files.
 
-        Method 1: Iterative Factor Analysis
+        **Method 1: Iterative Factor Analysis**
+        
         - Conducts factor analysis on the input variables to identify significant components.
         - Scales the data and calculates initial loading factors.
         - Iteratively refactors the data based on the Kaiser Criterion until all significant variables are included.
         - Calculates the SVI using the scaled factors and the ratio of variance.
         - Appends the SVI variables to the output dataframe.
 
-        Method 2: Rank Method
+        **Method 2: Rank Method**
+
         - Ranks the input variables in descending order for each observation.
         - Calculates the sum of ranks for each observation.
         - Calculates the SVI using the rank sum.
         - Appends the SVI variables to the output dataframe.
 
         The output dataframe is saved as a GeoPackage file and a CSV file.
-        Additionally, intermediate results from method 1 such as significant components, loading factors, and variances
+        Additionally, intermediate results from Method 1 such as significant components, loading factors, and variances
         are saved in an Excel file for documentation purposes.
         """
         # validate inputs
-        self.validate_value(boundary, ['bg', 'tract'], 'boundary')
-        self.validate_value(year, [2010, 2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022], 'year')
+        self._validate_value(boundary, ['bg', 'tract'], 'boundary')
+        self._validate_value(year, [2010, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022], 'year')
 
         # open the configuration file
         with open(os.path.join(self.variables, f"{config_file}.yaml")) as stream:
             try:
                 docs = list(yaml.safe_load_all(stream))
             except yaml.YAMLError as exc:
                 print(exc)
@@ -613,14 +647,15 @@
 
             return sig_components, include, df_ratio_var, df_variances
 
 
         # 1. Scale data
         scaler = MinMaxScaler()
         fa_df = pd.DataFrame(data=scaler.fit_transform(fa_df), columns=fa_df.columns, index=fa_df.index)
+        
         # 2. Conduct Factor Analysis and calculate initial loading factors
         fa, n_factors, loading_factors, facs = _initalize_fa(fa_df)
         # 3. Calculate initial variances
         sig_components, include, df_ratio_var, df_variances = _calc_variance(fa, n_factors, loading_factors, facs, df_variances)
 
         num_refactors+=1
         # 4. Begin refactor loop with initial 'include' array
@@ -697,15 +732,15 @@
         rank_df['sum_rank'] = rank_df.sum(axis=1)
         output_df['RM_SVI_Rank'] = rank_df['sum_rank'].rank()
         output_df['RM_SVI_Percentile'] = rank_df['sum_rank'].rank(ascending=False, pct=True)
         
 
         # save geopackage and csv output
         output_df.to_file(os.path.join(self.svis, f"{self.project_name}_{year}_{boundary}_{config_file}_svi.gpkg"))
-        data_df.to_csv(os.path.join(self.svis, f"{self.project_name}_{year}_{boundary}_{config_file}_svi.csv"))
+        output_df.to_csv(os.path.join(self.svis, f"{self.project_name}_{year}_{boundary}_{config_file}_svi.csv"))
          
 
 
 
 
     ###################################################
     # PRIVATE METHODS (helper functions)
@@ -837,15 +872,15 @@
             for miss_col in empty_cols:
                 new_col = miss_col + '_y'
                 data_df[miss_col] = data_df[new_col]
                 data_df = data_df.drop([new_col], axis=1)
             cols_to_drop = data_df.filter(like='_y', axis=1).columns
             data_df = data_df.drop(cols_to_drop, axis=1)
 
-        if verbose is True:
+        if verbose is True and empty_cols:
              with open(empty_output_name, 'w', newline='') as file:
                 writer = csv.writer(file)
                 # Write rows to the CSV file
                 writer.writerows(empty_output)
 
         return data_df
     
@@ -923,23 +958,24 @@
 
             if index == 0:
                 # not enough info, don't interpolate
                 pass
             else:
                 # determine the number of data points below the median interval
                 cumsum_before = calc['freq'].cumsum()[index-1]
+                # determine the width of the median interval
+                width = calc['high_range'][index + 1] - calc['low_range'][index + 1] + 1
                 # determine the number of data points in the median interval
                 freq_medain = calc['freq'][index + 1]
                 # rare case if new median falls in range of values with zero frequency
                 if freq_medain == 0:
-                    freq_medain = 1
-                # determine the width of the median interval
-                width = calc['high_range'][index + 1] - calc['low_range'][index + 1] + 1
-                # calculate median
-                median = L1 + (N/2 - cumsum_before) / freq_medain * width
+                    median = L1 + (N/2 - cumsum_before)
+                else:
+                    # calculate median
+                    median = L1 + (N/2 - cumsum_before) / freq_medain * width
                 # fill in values of data frame
                 data_df.loc[fips, var] = median
                 interpolated_output.append([f'{fips}', var, 'Interpolated'])
 
 
         return data_df
   
@@ -1104,15 +1140,15 @@
                 data_df = self.__interpolate(fips,
                                              var,
                                              neighbors,
                                              holes_df,
                                              data_df, 
                                              'B25075', 
                                              'B25075_001E', 
-                                            [0, 10000, 15000, 20000, 25000, 30000,35000, 40000, 50000, 60000, 70000, 80000, 90000, 100000, 125000, 150000,  175000, 200000, 250000, 300000, 400000, 500000, 750000, 1000000, 1500000, 2000000], 
+                                            [0, 10000, 15000, 20000, 25000, 30000, 35000, 40000, 50000, 60000, 70000, 80000, 90000, 100000, 125000, 150000,  175000, 200000, 250000, 300000, 400000, 500000, 750000, 1000000, 1500000, 2000000], 
                                              [9999,14999,19999,24999,29999,34999,39999,49999,59999,69999,79999, 89999,99999,124999,149999,174999, 199999,249999,299999,399999,499999,749999,999999,1499999,1999999,2000001],
                                              interpolated_output)
 
             elif var == 'B01002_001E':
                 # Median Age
                 # variable name: MEDAGE
                 # filter value like: B01001
@@ -1184,10 +1220,7 @@
                 writer.writerows(interpolated_output)
 
             
         return data_df
     
 
 
-# Initialize an instance of SVInsight
-def project(project_name: str, file_path: str, api_key: str, geoids: list[str]):
-    return SVInsight(project_name, file_path, api_key, geoids)
```

### Comparing `svinsight-0.2.7/SVInsight.egg-info/PKG-INFO` & `svinsight-0.2.8/SVInsight.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: SVInsight
-Version: 0.2.7
+Version: 0.2.8
 Summary: Create social vulnerabilty index
 Home-page: https://github.com/mdp0023/SVInsight/
 Author: M. Preisser, P. Passalacqua, R. P. Bixler
 Author-email: Matthew Preisser <mattpreisser@gmail.com>
 Project-URL: Homepage, https://example.com
 Project-URL: Documentation, https://readthedocs.org
 Keywords: SVI
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: census==0.8.21
-Requires-Dist: factor_analyzer==0.5.1
-Requires-Dist: geopandas==0.14.2
-Requires-Dist: numpy==1.26.4
-Requires-Dist: pandas==2.2.2
-Requires-Dist: PyYAML==6.0.1
-Requires-Dist: scikit_learn==1.3.0
+Requires-Dist: census>=0.8.21
+Requires-Dist: factor_analyzer>=0.5.1
+Requires-Dist: geopandas>=0.14.2
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: pandas>=2.2.2
+Requires-Dist: PyYAML>=6.0.1
+Requires-Dist: scikit_learn>=1.3.0
+Requires-Dist: openpyxl>=3.0.10
```

### Comparing `svinsight-0.2.7/pyproject.toml` & `svinsight-0.2.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SVInsight"
-version = "0.2.7"
+version = "0.2.8"
 dependencies = [
-    "census==0.8.21",
-    "factor_analyzer==0.5.1",
-    "geopandas==0.14.2",
-    "numpy==1.26.4",
-    "pandas==2.2.2",
-    "PyYAML==6.0.1",
-    "scikit_learn==1.3.0"
+    "census>=0.8.21",
+    "factor_analyzer>=0.5.1",
+    "geopandas>=0.14.2",
+    "numpy>=1.26.4",
+    "pandas>=2.2.2",
+    "PyYAML>=6.0.1",
+    "scikit_learn>=1.3.0",
+    "openpyxl>=3.0.10"
 ]
 requires-python = ">=3.8"
 authors = [
   {name = "Matthew Preisser", email = "mattpreisser@gmail.com"},
 ]
 description = "Create social vulnerabilty index"
 readme = "README.rst"
```

### Comparing `svinsight-0.2.7/setup.py` & `svinsight-0.2.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from setuptools import setup, find_packages
+#from SVInsight import __version__ as version
 
 setup(
     name='SVInsight',
-    version='0.2.7',
+    version='0.2.8',
     license='MIT',
     description='SVInsight - A python package for calculating an exploratory social vulnerability index',
     author='M. Preisser, P. Passalacqua, R. P. Bixler',
     author_email='mattpreisser@gmail.com',
     url='https://github.com/mdp0023/SVInsight/',
     packages= find_packages(exclude=['*.tests']),
     package_data = {'' : ['*.txt', '*.npz']},
```

