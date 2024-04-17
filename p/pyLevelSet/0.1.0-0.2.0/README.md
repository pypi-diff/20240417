# Comparing `tmp/pyLevelSet-0.1.0.tar.gz` & `tmp/pyLevelSet-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLevelSet-0.1.0.tar", last modified: Mon Apr 15 03:03:32 2024, max compression
+gzip compressed data, was "pyLevelSet-0.2.0.tar", last modified: Wed Apr 17 16:17:09 2024, max compression
```

## Comparing `pyLevelSet-0.1.0.tar` & `pyLevelSet-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 eleven    (1000) eleven    (1000)        0 2024-04-15 03:03:32.454770 pyLevelSet-0.1.0/
--rw-rw-r--   0 eleven    (1000) eleven    (1000)    35149 2023-07-10 08:03:07.000000 pyLevelSet-0.1.0/LICENSE
--rw-r--r--   0 eleven    (1000) eleven    (1000)     2932 2024-04-15 03:03:32.454770 pyLevelSet-0.1.0/PKG-INFO
--rw-rw-r--   0 eleven    (1000) eleven    (1000)     2207 2024-04-15 02:18:54.000000 pyLevelSet-0.1.0/README.md
-drwxrwxr-x   0 eleven    (1000) eleven    (1000)        0 2024-04-15 03:03:32.454770 pyLevelSet-0.1.0/pyLevelSet/
--rw-rw-r--   0 eleven    (1000) eleven    (1000)    32968 2024-04-14 15:59:14.000000 pyLevelSet-0.1.0/pyLevelSet/BasicShape.py
--rw-rw-r--   0 eleven    (1000) eleven    (1000)     9178 2024-04-05 12:34:32.000000 pyLevelSet-0.1.0/pyLevelSet/BuildSurfaceNode.py
--rw-rw-r--   0 eleven    (1000) eleven    (1000)    13904 2024-04-05 12:34:35.000000 pyLevelSet-0.1.0/pyLevelSet/FastMarchingMethod.py
--rw-rw-r--   0 eleven    (1000) eleven    (1000)     7279 2024-04-14 15:25:21.000000 pyLevelSet-0.1.0/pyLevelSet/LevelSetGrid.py
--rw-rw-r--   0 eleven    (1000) eleven    (1000)     2930 2024-04-05 12:34:42.000000 pyLevelSet-0.1.0/pyLevelSet/MultiSDF.py
--rw-rw-r--   0 eleven    (1000) eleven    (1000)     7892 2024-04-05 12:35:57.000000 pyLevelSet-0.1.0/pyLevelSet/SDFs.py
--rw-rw-r--   0 eleven    (1000) eleven    (1000)     5664 2024-04-05 12:34:50.000000 pyLevelSet-0.1.0/pyLevelSet/SDFs2D.py
--rw-rw-r--   0 eleven    (1000) eleven    (1000)    14573 2024-04-05 12:34:54.000000 pyLevelSet-0.1.0/pyLevelSet/SDFs3D.py
--rw-rw-r--   0 eleven    (1000) eleven    (1000)     1947 2024-04-15 01:46:33.000000 pyLevelSet-0.1.0/pyLevelSet/__init__.py
--rw-rw-r--   0 eleven    (1000) eleven    (1000)     3478 2024-02-16 14:42:15.000000 pyLevelSet-0.1.0/pyLevelSet/ease.py
--rw-rw-r--   0 eleven    (1000) eleven    (1000)     2919 2024-04-05 12:34:41.000000 pyLevelSet-0.1.0/pyLevelSet/mesh.py
--rw-rw-r--   0 eleven    (1000) eleven    (1000)     2182 2024-02-04 15:02:53.000000 pyLevelSet-0.1.0/pyLevelSet/progress.py
--rw-rw-r--   0 eleven    (1000) eleven    (1000)     4414 2024-04-05 12:34:57.000000 pyLevelSet-0.1.0/pyLevelSet/text.py
--rw-rw-r--   0 eleven    (1000) eleven    (1000)     4242 2024-04-05 12:35:43.000000 pyLevelSet-0.1.0/pyLevelSet/utils.py
--rw-rw-r--   0 eleven    (1000) eleven    (1000)     1119 2024-04-05 12:35:22.000000 pyLevelSet-0.1.0/pyLevelSet/utils23D.py
--rw-rw-r--   0 eleven    (1000) eleven    (1000)     1082 2024-04-05 12:35:15.000000 pyLevelSet-0.1.0/pyLevelSet/utils2D.py
--rw-rw-r--   0 eleven    (1000) eleven    (1000)     4282 2024-04-05 12:35:18.000000 pyLevelSet-0.1.0/pyLevelSet/utils3D.py
-drwxrwxr-x   0 eleven    (1000) eleven    (1000)        0 2024-04-15 03:03:32.454770 pyLevelSet-0.1.0/pyLevelSet.egg-info/
--rw-r--r--   0 eleven    (1000) eleven    (1000)     2932 2024-04-15 03:03:32.000000 pyLevelSet-0.1.0/pyLevelSet.egg-info/PKG-INFO
--rw-rw-r--   0 eleven    (1000) eleven    (1000)      585 2024-04-15 03:03:32.000000 pyLevelSet-0.1.0/pyLevelSet.egg-info/SOURCES.txt
--rw-rw-r--   0 eleven    (1000) eleven    (1000)        1 2024-04-15 03:03:32.000000 pyLevelSet-0.1.0/pyLevelSet.egg-info/dependency_links.txt
--rw-rw-r--   0 eleven    (1000) eleven    (1000)       57 2024-04-15 03:03:32.000000 pyLevelSet-0.1.0/pyLevelSet.egg-info/requires.txt
--rw-rw-r--   0 eleven    (1000) eleven    (1000)       11 2024-04-15 03:03:32.000000 pyLevelSet-0.1.0/pyLevelSet.egg-info/top_level.txt
--rw-rw-r--   0 eleven    (1000) eleven    (1000)       38 2024-04-15 03:03:32.454770 pyLevelSet-0.1.0/setup.cfg
--rw-rw-r--   0 eleven    (1000) eleven    (1000)     1455 2024-04-15 03:03:28.000000 pyLevelSet-0.1.0/setup.py
+drwxrwxr-x   0 eleven    (1000) eleven    (1000)        0 2024-04-17 16:17:09.841201 pyLevelSet-0.2.0/
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)    35149 2023-07-10 08:03:07.000000 pyLevelSet-0.2.0/LICENSE
+-rw-r--r--   0 eleven    (1000) eleven    (1000)     5613 2024-04-17 16:17:09.841201 pyLevelSet-0.2.0/PKG-INFO
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)     4866 2024-04-17 16:07:23.000000 pyLevelSet-0.2.0/README.md
+drwxrwxr-x   0 eleven    (1000) eleven    (1000)        0 2024-04-17 16:17:09.841201 pyLevelSet-0.2.0/pyLevelSet/
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)    33189 2024-04-17 15:44:35.000000 pyLevelSet-0.2.0/pyLevelSet/BasicShape.py
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)     9178 2024-04-15 03:16:35.000000 pyLevelSet-0.2.0/pyLevelSet/BuildSurfaceNode.py
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)    13904 2024-04-15 03:16:35.000000 pyLevelSet-0.2.0/pyLevelSet/FastMarchingMethod.py
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)     7440 2024-04-17 15:45:08.000000 pyLevelSet-0.2.0/pyLevelSet/LevelSetGrid.py
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)     2930 2024-04-15 03:16:35.000000 pyLevelSet-0.2.0/pyLevelSet/MultiSDF.py
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)     7892 2024-04-15 03:16:35.000000 pyLevelSet-0.2.0/pyLevelSet/SDFs.py
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)     5664 2024-04-15 03:16:35.000000 pyLevelSet-0.2.0/pyLevelSet/SDFs2D.py
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)    14573 2024-04-15 03:16:35.000000 pyLevelSet-0.2.0/pyLevelSet/SDFs3D.py
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)     1947 2024-04-17 16:16:04.000000 pyLevelSet-0.2.0/pyLevelSet/__init__.py
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)     3478 2024-04-15 03:16:35.000000 pyLevelSet-0.2.0/pyLevelSet/ease.py
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)     2919 2024-04-15 03:16:35.000000 pyLevelSet-0.2.0/pyLevelSet/mesh.py
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)     2182 2024-04-15 03:16:35.000000 pyLevelSet-0.2.0/pyLevelSet/progress.py
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)     4414 2024-04-15 03:16:35.000000 pyLevelSet-0.2.0/pyLevelSet/text.py
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)     4242 2024-04-15 03:16:35.000000 pyLevelSet-0.2.0/pyLevelSet/utils.py
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)     1119 2024-04-15 03:16:35.000000 pyLevelSet-0.2.0/pyLevelSet/utils23D.py
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)     1082 2024-04-15 03:16:35.000000 pyLevelSet-0.2.0/pyLevelSet/utils2D.py
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)     4282 2024-04-15 03:16:35.000000 pyLevelSet-0.2.0/pyLevelSet/utils3D.py
+drwxrwxr-x   0 eleven    (1000) eleven    (1000)        0 2024-04-17 16:17:09.841201 pyLevelSet-0.2.0/pyLevelSet.egg-info/
+-rw-r--r--   0 eleven    (1000) eleven    (1000)     5613 2024-04-17 16:17:09.000000 pyLevelSet-0.2.0/pyLevelSet.egg-info/PKG-INFO
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)      585 2024-04-17 16:17:09.000000 pyLevelSet-0.2.0/pyLevelSet.egg-info/SOURCES.txt
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)        1 2024-04-17 16:17:09.000000 pyLevelSet-0.2.0/pyLevelSet.egg-info/dependency_links.txt
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)       64 2024-04-17 16:17:09.000000 pyLevelSet-0.2.0/pyLevelSet.egg-info/requires.txt
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)       11 2024-04-17 16:17:09.000000 pyLevelSet-0.2.0/pyLevelSet.egg-info/top_level.txt
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)       38 2024-04-17 16:17:09.841201 pyLevelSet-0.2.0/setup.cfg
+-rw-rw-r--   0 eleven    (1000) eleven    (1000)     1496 2024-04-17 16:15:59.000000 pyLevelSet-0.2.0/setup.py
```

### Comparing `pyLevelSet-0.1.0/LICENSE` & `pyLevelSet-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyLevelSet-0.1.0/pyLevelSet/BasicShape.py` & `pyLevelSet-0.2.0/pyLevelSet/BasicShape.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,14 +279,20 @@
             raise RuntimeError(f"Incorrect LevelSet input: local frame is non-inertial.",
                                f"Indeed, Ixx = {inertia[0]}; Iyy = {inertia[1]}; Izz = {inertia[1]}; Ixy = {inertia[3]}; Ixz = {inertia[4]}; Iyz = {inertia[5]}",
 		                       f" for inertia matrix I, making for a {ratio} non-diagonality ratio.")
         else:
             self._inertia = np.array([inertia_xx, inertia_yy, inertia_zz])
         self._is_inertia = True
 
+    def _get_bounding_box(self):
+        box_center = self.mesh.bounding_box.transform[0:3, 3]
+        self._lower_bound = box_center -0.5 * self.mesh.bounding_box.extents
+        self._higher_bound = box_center + 0.5 * self.mesh.bounding_box.extents
+        self._is_bound = True
+
     def _get_volume(self):
         self._volume = self.mesh.volume
         self._is_volume = True
 
     def _get_mass_cener(self):
         self._center = self.mesh.center_mass
         self._is_center = True
@@ -313,23 +319,25 @@
     def mesh_operation(self):
         if self._reset:
             self.mesh.apply_translation(-self.mesh.center_mass)
             _, new_axis = tm.inertia.principal_axis(self.mesh.moment_inertia)
             default_axis = np.eye(3)
             rotation_matrix = transformation_matrix_coordinate_system(new_axis, default_axis)
             self.mesh.apply_transform(rotation_matrix)
+            self.generate_sdf()
 
     def split(self, iteration=1):
         if self.mesh is None:
             raise RuntimeError("Primitive should be generate first")
         pass
 
     def generate_sdf(self):
-        self._estimate_bounding_box()
+        self._get_bounding_box()
         region_size = self.upper_bound - self.lower_bound
+        self.grid.clear()
         self.grid.set_grid(self.lower_bound, region_size)
         self.grid.build_node_coords()
         self.grid.generate_sdf(self(self.grid.node_coord).reshape(-1))
 
     def construct_surface_mesh_from_point_cloud(self, points, estimate_normals=False):
         pcd = o3d.geometry.PointCloud()
         if not estimate_normals:
@@ -337,16 +345,17 @@
         else:
             normals = pcd.estimate_normals(search_param=o3d.geometry.KDTreeSearchParamKNN(knn=20))
         pcd.points = o3d.utility.Vector3dVector(points)
         pcd.normals = o3d.utility.Vector3dVector(normals)
 
         # ball pivoting method
         distances = pcd.compute_nearest_neighbor_distance()
-        avg_dist = np.mean(distances)
-        meshs = o3d.geometry.TriangleMesh.create_from_point_cloud_ball_pivoting(pcd, o3d.utility.DoubleVector(np.linspace(avg_dist, 8*avg_dist, 4)))
+        min_dist = np.min(distances)
+        max_dist = np.max(distances)
+        meshs = o3d.geometry.TriangleMesh.create_from_point_cloud_ball_pivoting(pcd, o3d.utility.DoubleVector(np.linspace(0.2*min_dist, 8*max_dist, 8)))
         meshs.remove_degenerate_triangles()
         meshs.remove_duplicated_triangles()
         meshs.remove_duplicated_vertices()
         meshs.remove_non_manifold_edges()
         return meshs
 
     def ray_tracing(self, samples, ray_path):
@@ -535,47 +544,45 @@
 class pointcloud(BasicShape):
     def __init__(self, points) -> None:
         super().__init__(ray=False)
         meshs = self.construct_surface_mesh_from_point_cloud(points, estimate_normals=True)
         self.mesh = tm.Trimesh(vertices=np.asarray(meshs.vertices), faces=np.asarray(meshs.triangles))
 
     def generate(self, *args, **kwargs):
+        self.generate_sdf()
         self.mesh_operation()
-        self.grid.move(self.mesh.center_mass)
 
 
 class MeshBased(BasicShape):
     def __init__(self):
         super().__init__(ray=False)
 
     def _estimate_bounding_box(self):
-        self._lower_bound = self.center -0.5 * self.mesh.bounding_box.extents
-        self._higher_bound = self.center + 0.5 * self.mesh.bounding_box.extents
-        self._is_bound = True
+        self._get_bounding_box()
     
     def side(self, p):
         p = self.transfer(p)
         return self.mesh.contains(p)
     
     def generate(self, *args, **kwargs):
+        self.generate_sdf()
         self.mesh_operation()
 
     def _normal(self, p):
         pass
 
 
 class arbitrarily(MeshBased):
     def __init__(self, start_point, region_size, distance_field, node_coordinate, vertices, faces) -> None:
         super().__init__()
         self.is_simple_shape = 1
         self.mesh = tm.Trimesh(vertices=vertices, faces=faces)
         self.grid = LocalGrid()
         self.grid.set_distance_field(np.array(start_point), np.array(region_size), 
                                      np.array(node_coordinate), np.array(distance_field), self.mesh.center_mass)
-        
 
 
 class polyhedron(MeshBased):
     def __init__(self, file: str) -> None:
         super().__init__()
         self.is_simple_shape = 1
         self.mesh: tm.Trimesh = tm.load(file, force='mesh')
```

### Comparing `pyLevelSet-0.1.0/pyLevelSet/BuildSurfaceNode.py` & `pyLevelSet-0.2.0/pyLevelSet/BuildSurfaceNode.py`

 * *Files identical despite different names*

### Comparing `pyLevelSet-0.1.0/pyLevelSet/FastMarchingMethod.py` & `pyLevelSet-0.2.0/pyLevelSet/FastMarchingMethod.py`

 * *Files identical despite different names*

### Comparing `pyLevelSet-0.1.0/pyLevelSet/LevelSetGrid.py` & `pyLevelSet-0.2.0/pyLevelSet/LevelSetGrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,20 @@
     
     def maxBox(self):
         return self.start_point + self.region_size
 
     def read_grid(self, space, extent=0):
         self.grid_space = space
         self.extent = extent
+
+    def clear(self):
+        self.gnum = np.zeros(3, dtype=np.int32)
+        self.gridSum = 0
+        self.distance_field = None
+        self.node_coord = None
     
     def set_distance_field(self, start_point, region_size, node_cood, distance_field, center_mass):
         self.start_point = start_point - center_mass
         self.region_size = region_size - center_mass
         self.node_coord = node_cood - center_mass
         self.distance_field = distance_field
```

### Comparing `pyLevelSet-0.1.0/pyLevelSet/MultiSDF.py` & `pyLevelSet-0.2.0/pyLevelSet/MultiSDF.py`

 * *Files identical despite different names*

### Comparing `pyLevelSet-0.1.0/pyLevelSet/SDFs.py` & `pyLevelSet-0.2.0/pyLevelSet/SDFs.py`

 * *Files identical despite different names*

### Comparing `pyLevelSet-0.1.0/pyLevelSet/SDFs2D.py` & `pyLevelSet-0.2.0/pyLevelSet/SDFs2D.py`

 * *Files identical despite different names*

### Comparing `pyLevelSet-0.1.0/pyLevelSet/SDFs3D.py` & `pyLevelSet-0.2.0/pyLevelSet/SDFs3D.py`

 * *Files identical despite different names*

### Comparing `pyLevelSet-0.1.0/pyLevelSet/__init__.py` & `pyLevelSet-0.2.0/pyLevelSet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) 2023, multiscale geomechanics lab, Zhejiang University
 # This file is from the GeoTaichi project, released under the GNU General Public License v3.0
 
 __author__ = "Shi-Yihao, Guo-Ning"
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 __license__ = "GNU License"
 
 
 from .BasicShape import pointcloud, arbitrarily, polyhedron, surfacefunction, polysuperquadrics, polysuperellipsoid
 
 from .SDFs2D import (
     circle, line, slab,
```

### Comparing `pyLevelSet-0.1.0/pyLevelSet/ease.py` & `pyLevelSet-0.2.0/pyLevelSet/ease.py`

 * *Files identical despite different names*

### Comparing `pyLevelSet-0.1.0/pyLevelSet/mesh.py` & `pyLevelSet-0.2.0/pyLevelSet/mesh.py`

 * *Files identical despite different names*

### Comparing `pyLevelSet-0.1.0/pyLevelSet/progress.py` & `pyLevelSet-0.2.0/pyLevelSet/progress.py`

 * *Files identical despite different names*

### Comparing `pyLevelSet-0.1.0/pyLevelSet/text.py` & `pyLevelSet-0.2.0/pyLevelSet/text.py`

 * *Files identical despite different names*

### Comparing `pyLevelSet-0.1.0/pyLevelSet/utils.py` & `pyLevelSet-0.2.0/pyLevelSet/utils.py`

 * *Files identical despite different names*

### Comparing `pyLevelSet-0.1.0/pyLevelSet/utils23D.py` & `pyLevelSet-0.2.0/pyLevelSet/utils23D.py`

 * *Files identical despite different names*

### Comparing `pyLevelSet-0.1.0/pyLevelSet/utils2D.py` & `pyLevelSet-0.2.0/pyLevelSet/utils2D.py`

 * *Files identical despite different names*

### Comparing `pyLevelSet-0.1.0/pyLevelSet/utils3D.py` & `pyLevelSet-0.2.0/pyLevelSet/utils3D.py`

 * *Files identical despite different names*

### Comparing `pyLevelSet-0.1.0/pyLevelSet.egg-info/SOURCES.txt` & `pyLevelSet-0.2.0/pyLevelSet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyLevelSet-0.1.0/setup.py` & `pyLevelSet-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
           name="pyLevelSet",
-          version="0.1.0",
+          version="0.2.0",
           author="Shi-YiHao",
           author_email="syh-1999@outlook.com",
           description="A Level-set particles generator",
           long_description=long_description,
           long_description_content_type="text/markdown",
           url="https://github.com/Yihao-Shi/pyLevelSet",
           packages=find_packages(exclude='images'),
@@ -19,15 +19,16 @@
           install_requires=[
                                'numpy',
                                'scipy',
                                'trimesh',
                                'scikit-image',
                                'rtree',
                                'open3d',
-                               'matplotlib'
+                               'matplotlib',
+                               'pyevtk'
                            ],
           classifiers=[
                           'Programming Language :: Python :: 3.8',
                           'Programming Language :: Python :: 3.9',
                           'Programming Language :: Python :: 3.10',
                           'License :: OSI Approved :: GNU Affero General Public License v3',
                           'Development Status :: 3 - Alpha'
```

