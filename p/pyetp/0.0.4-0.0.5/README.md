# Comparing `tmp/pyetp-0.0.4.tar.gz` & `tmp/pyetp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyetp-0.0.4.tar", max compression
+gzip compressed data, was "pyetp-0.0.5.tar", max compression
```

## Comparing `pyetp-0.0.4.tar` & `pyetp-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7652 2024-04-09 12:18:29.210834 pyetp-0.0.4/LICENSE.md
--rw-r--r--   0        0        0     1224 2024-04-09 12:18:29.210834 pyetp-0.0.4/README.md
--rw-r--r--   0        0        0      123 2024-04-09 12:18:30.038834 pyetp-0.0.4/pyetp/__init__.py
--rw-r--r--   0        0        0    32411 2024-04-09 12:18:30.038834 pyetp-0.0.4/pyetp/client.py
--rw-r--r--   0        0        0      879 2024-04-09 12:18:30.038834 pyetp-0.0.4/pyetp/config.py
--rw-r--r--   0        0        0    50492 2024-04-09 12:18:30.038834 pyetp-0.0.4/pyetp/resqml_objects/__init__.py
--rw-r--r--   0        0        0   783914 2024-04-09 12:18:30.042834 pyetp-0.0.4/pyetp/resqml_objects/generated.py
--rw-r--r--   0        0        0     2487 2024-04-09 12:18:30.042834 pyetp-0.0.4/pyetp/types.py
--rw-r--r--   0        0        0     2675 2024-04-09 12:18:30.042834 pyetp-0.0.4/pyetp/uri.py
--rw-r--r--   0        0        0     2248 2024-04-09 12:18:30.042834 pyetp-0.0.4/pyetp/utils_arrays.py
--rw-r--r--   0        0        0    18443 2024-04-09 12:18:30.042834 pyetp-0.0.4/pyetp/utils_xml.py
--rw-r--r--   0        0        0      877 2024-04-09 12:19:03.038812 pyetp-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pyetp-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-04-17 10:15:57.691925 pyetp-0.0.5/LICENSE.md
+-rw-r--r--   0        0        0     1224 2024-04-17 10:15:57.691925 pyetp-0.0.5/README.md
+-rw-r--r--   0        0        0      123 2024-04-17 10:16:00.739954 pyetp-0.0.5/pyetp/__init__.py
+-rw-r--r--   0        0        0    33452 2024-04-17 10:16:00.739954 pyetp-0.0.5/pyetp/client.py
+-rw-r--r--   0        0        0      879 2024-04-17 10:16:00.739954 pyetp-0.0.5/pyetp/config.py
+-rw-r--r--   0        0        0    50492 2024-04-17 10:16:00.739954 pyetp-0.0.5/pyetp/resqml_objects/__init__.py
+-rw-r--r--   0        0        0   783914 2024-04-17 10:16:00.743954 pyetp-0.0.5/pyetp/resqml_objects/generated.py
+-rw-r--r--   0        0        0     2487 2024-04-17 10:16:00.743954 pyetp-0.0.5/pyetp/types.py
+-rw-r--r--   0        0        0     2675 2024-04-17 10:16:00.743954 pyetp-0.0.5/pyetp/uri.py
+-rw-r--r--   0        0        0     2248 2024-04-17 10:16:00.743954 pyetp-0.0.5/pyetp/utils_arrays.py
+-rw-r--r--   0        0        0    24379 2024-04-17 10:16:00.743954 pyetp-0.0.5/pyetp/utils_xml.py
+-rw-r--r--   0        0        0      877 2024-04-17 10:16:37.552336 pyetp-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pyetp-0.0.5/PKG-INFO
```

### Comparing `pyetp-0.0.4/LICENSE.md` & `pyetp-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.4/README.md` & `pyetp-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.4/pyetp/client.py` & `pyetp-0.0.5/pyetp/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,18 +99,15 @@
 
         return msg.header.message_id
 
     async def _recv(self, correlation_id: int) -> ETPModel:
         assert correlation_id in self._recv_events, "trying to recv response on non-existing message"
 
         try:
-            
             async with timeout(self.timeout):
-                #await inner()
-            # async with asyncio.timeout(self.timeout):
                 await self._recv_events[correlation_id].wait()
         except asyncio.CancelledError as e:
             raise TimeoutError(f'Timeout before reciving {correlation_id=}') from e
 
         # cleanup
         bodies = self._clear_msg_on_buffer(correlation_id)
 
@@ -473,16 +470,24 @@
         )
 
         return cprop0, values
 
     async def put_epc_mesh(
         self, epc_filename, title_in, property_titles, projected_epsg, dataspace
     ):
-        uns, crs, epc, hexa = utils_xml.convert_epc_mesh_to_resqml_mesh(epc_filename, title_in, projected_epsg)
+        uns, crs, epc, timeseries, hexa = utils_xml.convert_epc_mesh_to_resqml_mesh(epc_filename, title_in, projected_epsg)
         epc_uri, crs_uri, uns_uri = await self.put_resqml_objects(epc, crs, uns, dataspace=dataspace)
+        timeseries_uri = ""
+        if timeseries is not None:
+            timeseries_uris = await self.put_resqml_objects(timeseries, dataspace=dataspace)
+            timeseries_uri = list(timeseries_uris)[0] if (len(list(timeseries_uris)) > 0) else ""
+        
+        # print("put_epc_mesh", uns, crs, epc, timeseries)
+        # print("put_epc_mesh", epc_uri, crs_uri, uns_uri, timeseries_uri)
+        print("put_epc_mesh property_titles", property_titles)
 
         #
         # mesh geometry (six arrays)
         #
         response = await self.put_array(
             DataArrayIdentifier(
                 uri=epc_uri.raw_uri if isinstance(epc_uri, DataObjectURI) else epc_uri,
@@ -532,32 +537,41 @@
         )
 
         #
         # mesh properties: one Property, one array of values, and an optional PropertyKind per property
         #
         prop_rddms_uris = {}
         for propname in property_titles:
-            cprop0, prop, propertykind0 = utils_xml.convert_epc_mesh_property_to_resqml_mesh(epc_filename, hexa, propname, uns, epc)
-
-            assert isinstance(cprop0, ro.ContinuousProperty) or isinstance(cprop0, ro.DiscreteProperty), "prop must be a Property"
-            assert len(cprop0.patch_of_values) == 1, "property obj must have exactly one patch of values"
-
-            propkind_uri = "" if (propertykind0 is None) else (await self.put_resqml_objects(propertykind0, dataspace=dataspace))
-            cprop_uri = await self.put_resqml_objects(cprop0, dataspace=dataspace)
-
-            prop_rddms_uris[propname] = [propkind_uri, cprop_uri]
-            response = await self.put_array(
-                DataArrayIdentifier(
-                    uri=epc_uri.raw_uri if isinstance(epc_uri, DataObjectURI) else epc_uri,
-                    pathInResource=cprop0.patch_of_values[0].values.values.path_in_hdf_file,
-                ),
-                prop.array_ref(),  # type: ignore
-            )
+            if timeseries is not None:
+                time_indices = list(range(len(timeseries.time)))
+                # print(f"prop {propname}: len of timeseries: {len(timeseries.time)}")
+                cprop0s, props, propertykind0 = utils_xml.convert_epc_mesh_property_to_resqml_mesh(epc_filename, hexa, propname, uns, epc, timeseries=timeseries, time_indices=time_indices)
+            else:
+                time_indices = [-1]
+                cprop0s, props, propertykind0 = utils_xml.convert_epc_mesh_property_to_resqml_mesh(epc_filename, hexa, propname, uns, epc)
+
+            cprop_uris = []
+            for cprop0, prop, time_index in zip(cprop0s, props, time_indices):
+                assert isinstance(cprop0, ro.ContinuousProperty) or isinstance(cprop0, ro.DiscreteProperty), "prop must be a Property"
+                assert len(cprop0.patch_of_values) == 1, "property obj must have exactly one patch of values"
+
+                propkind_uri = "" if (propertykind0 is None) else (await self.put_resqml_objects(propertykind0, dataspace=dataspace))
+                cprop_uri = await self.put_resqml_objects(cprop0, dataspace=dataspace)
+                
+                response = await self.put_array(
+                    DataArrayIdentifier(
+                        uri=epc_uri.raw_uri if isinstance(epc_uri, DataObjectURI) else epc_uri,
+                        pathInResource=cprop0.patch_of_values[0].values.values.path_in_hdf_file,
+                    ),
+                    prop.array_ref(),  # type: ignore
+                )
+                cprop_uris.append(cprop_uri)
+            prop_rddms_uris[propname] = [propkind_uri, cprop_uris]
 
-        return [epc_uri, crs_uri, uns_uri], prop_rddms_uris
+        return [epc_uri, crs_uri, uns_uri, timeseries_uri], prop_rddms_uris
 
     #
     # array
     #
 
     async def get_array_metadata(self, *uids: DataArrayIdentifier):
         from etptypes.energistics.etp.v12.protocol.data_array.get_data_array_metadata import \
```

### Comparing `pyetp-0.0.4/pyetp/config.py` & `pyetp-0.0.5/pyetp/config.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.4/pyetp/resqml_objects/__init__.py` & `pyetp-0.0.5/pyetp/resqml_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.4/pyetp/resqml_objects/generated.py` & `pyetp-0.0.5/pyetp/resqml_objects/generated.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.4/pyetp/types.py` & `pyetp-0.0.5/pyetp/types.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.4/pyetp/uri.py` & `pyetp-0.0.5/pyetp/uri.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.4/pyetp/utils_arrays.py` & `pyetp-0.0.5/pyetp/utils_arrays.py`

 * *Files identical despite different names*

### Comparing `pyetp-0.0.4/pyetp/utils_xml.py` & `pyetp-0.0.5/pyetp/utils_xml.py`

 * *Files 21% similar despite different names*

```diff
@@ -207,14 +207,16 @@
     return epc, crs, gri
 
 
 def convert_epc_mesh_to_resqml_mesh(epc_filename, title_in, projected_epsg):
     import numpy as np
     import resqpy.model as rq
     import resqpy.unstructured as rug
+    import resqpy.property as rqp
+    import resqpy.time_series as rts
 
     title = title_in or "hexamesh"
 
     model = rq.Model(epc_filename)
     assert model is not None
 
     #
@@ -223,14 +225,100 @@
     hexa_uuid = model.uuid(obj_type='UnstructuredGridRepresentation', title=title_in)
     assert hexa_uuid is not None
     hexa = rug.HexaGrid(model, uuid=hexa_uuid)
     assert hexa is not None
     assert hexa.cell_shape == 'hexahedral'
     hexa.check_hexahedral()
 
+    ts_uuid = model.uuid(obj_type = "TimeSeries")
+    # ts_uuid_2 = model.uuid(obj_type='GeologicTimeSeries')
+    # print("TS UUIDs: ", ts_uuid, ts_uuid_2)
+    gts = rts.GeologicTimeSeries(model, uuid=ts_uuid)
+    print("gts: ", gts)
+    timeseries = None
+    # dynamic_points = []    
+    if (ts_uuid is not None) and (gts is not None):
+        temp_uuids = model.uuids(title = 'Temperature')
+        node_uuids = model.uuids(title = 'points')        
+        # print("temp_uuids", temp_uuids)
+        # print("node_uuids", node_uuids)
+
+        points_cached_series = []
+        Temp_per_vertex_series = []
+
+        # for uuid in node_uuids[0:-1:10]:
+        ro_timestamps = []
+        for uuid in node_uuids:
+            prop = rqp.Property(model, uuid = uuid)
+            # print(uuid, prop)
+            tst = float(str(gts.timestamp( prop.time_index())).replace(' Ma',''))
+            # print(f'index: {prop.time_index()}  time stamp: {gts.timestamp( prop.time_index())}   tst: {int(tst*1e6)}' )
+            ro_timestamps.append(
+                ro.Timestamp(
+                    date_time=XmlDateTime.from_string("0001-01-01T00:00:00.00+00:00"),
+                    year_offset=int(tst*1e6),
+                )
+            )
+            # points = prop.array_ref()
+            # # print(f'time stamp: {gts.timestamp( prop.time_index())} -- thickness of crust+sed: {(np.amax(points)-np.amin(points)):.2f}    shape: {points.shape}')  # type: ignore
+            # dynamic_points.append(points)
+
+        print(f"Generating time series with {len(ro_timestamps)} indices, year offsets: {ro_timestamps[0].year_offset} -- {ro_timestamps[-1].year_offset}.")
+
+        timeseries = ro.TimeSeries(
+            citation=create_common_citation(str(gts.citation_title)),
+            schema_version=schema_version,
+            uuid=str(gts.uuid),
+            time = ro_timestamps,
+        )
+
+        # for tti in self.time_indices:
+        #     x_original_order, T_per_vertex = self.get_node_pos_and_temp(tti)
+        #     T_per_vertex_filt = [ T_per_vertex[i] for i in range(x_original_order.shape[0]) if i in p_to_keep  ]
+        #     Temp_per_vertex_series.append(np.array(T_per_vertex_filt))
+        #     points_cached = []
+        #     point_original_to_cached = np.ones(x_original_order.shape[0], dtype = np.int32)  * (-1)
+        #     for i in range(x_original_order.shape[0]):
+        #         if (i in p_to_keep):
+        #             point_original_to_cached[i] = len(points_cached)
+        #             points_cached.append(x_original_order[i,:])
+        #     points_cached_series.append(np.array(points_cached))
+
+        # for uuid_t,uuid_p in zip(temp_uuids[0:-1:10], node_uuids[0:-1:10]):
+        #     prop = rqp.Property(model, uuid = uuid_t)
+        #     temperature = prop.array_ref()
+        #     prop_p = rqp.Property(model, uuid = uuid_p)
+        #     points = prop_p.array_ref()
+        #     sumT = 0
+        #     sumW = 0
+        #     for i,c in enumerate(cells):
+        #         p0 = points[c,:]
+        #         vv = volumeOfHex(p0[[0,2,6,4,1,3,7,5]])
+        #         sumT = sumT + temperature[i]*vv
+        #         sumW = sumW + vv
+        #     Tmean = sumT / sumW
+        #     print(f'time stamp: {gts.timestamp( prop.time_index())} -- mean temperature: {Tmean:.2f}')
+
+        # import numpy as np
+        # for uuid in node_uuids[0:-1:10]:
+        #     prop = rqp.Property(model, uuid = uuid)
+        #     points = prop.array_ref()
+        #     print(f'time stamp: {gts.timestamp( prop.time_index())} -- thickness of crust+sed: {(np.amax(points)-np.amin(points)):.2f}    shape: {points.shape}')  # type: ignore
+        #     c0 = cells[0,:]
+        #     p0 = points[c0,:]
+        #     vv = volumeOfHex(p0[[0,2,6,4,1,3,7,5]])
+        #     if ( np.abs(vv-312805.18)<1) :
+        #         print(vv)
+        #         print(c0)
+        #         print(p0)
+                
+        #     print(f'time stamp: {gts.timestamp( prop.time_index())} -- volume of cell 0: {vv:.2f}')
+
+        pass
+
     crs = create_common_crs(title, projected_epsg)
 
     epc = ro.EpcExternalPartReference(
         citation=create_common_citation("Hdf Proxy"),
         schema_version=schema_version,
         uuid=str(uuid4()),
         mime_type="application/x-hdf5",
@@ -323,18 +411,18 @@
         schema_version=schema_version,
         # surface_role=resqml_objects.SurfaceRole.MAP,
         citation=create_common_citation(hexa.title),
         cell_count=hexa.cell_count or -1,
         geometry=geom,
     )
 
-    return uns, crs, epc, hexa
+    return uns, crs, epc, timeseries, hexa
 
 
-def convert_epc_mesh_property_to_resqml_mesh(epc_filename, hexa, prop_title, uns, epc):
+def convert_epc_mesh_property_to_resqml_mesh(epc_filename, hexa, prop_title, uns, epc, timeseries=None, time_indices:list[int]=[]):
     import resqpy.model as rq
     import resqpy.property as rqp
 
     def uom_for_prop_title(pt):
         if (pt == "Age"):
             return ro.ResqmlUom.A_1
         if (pt == "Temperature"):
@@ -347,114 +435,152 @@
             return ro.ResqmlUom.VALUE_1_M
         if (pt == "Density_solid"):
             return ro.ResqmlUom.KG_M3
         if (pt == "insulance_thermal"):
             return ro.ThermalInsulanceUom.DELTA_K_M2_W
         if (pt == "Radiogenic_heat_production"):
             return ro.ResqmlUom.U_W_M3
+        if (pt == 'dynamic nodes') or (pt=='points'):
+            return ro.ResqmlUom.M
         return ro.ResqmlUom.EUC
 
     model = rq.Model(epc_filename)
     assert model is not None
-    prop_uuid = model.uuid(title=prop_title)
-    prop = rqp.Property(model, uuid=prop_uuid)
 
-    continuous = prop.is_continuous()
+    use_timeseries = (timeseries is not None) and (time_indices)
+    if not use_timeseries:
+        prop_uuid0 = model.uuid(title=prop_title)
+        prop0 = rqp.Property(model, uuid=prop_uuid0)
+    else:
+        prop_uuids = model.uuids(title=prop_title)
+        prop_uuid0 = prop_uuids[time_indices[0]]
+        prop0 = rqp.Property(model, uuid=prop_uuid0)   # a prop representative of all in the timeseries
+
+    continuous = prop0.is_continuous()
 
-    if (prop.local_property_kind_uuid() is None):
+    if (prop0.local_property_kind_uuid() is None):
         propertykind0 = None
     else:
-        pk = rqp.PropertyKind(model, uuid=prop.local_property_kind_uuid())
+        pk = rqp.PropertyKind(model, uuid=prop0.local_property_kind_uuid())
         propertykind0 = ro.PropertyKind(
             schema_version=schema_version,
             citation=create_common_citation(f"{prop_title}"),
             naming_system="urn:resqml:bp.com:resqpy",
             is_abstract=False,
             representative_uom=uom_for_prop_title(prop_title),
             parent_property_kind=ro.StandardPropertyKind(
                 kind=ro.ResqmlPropertyKind.CONTINUOUS if continuous else ro.ResqmlPropertyKind.DISCRETE
             ),
             uuid=str(pk.uuid),
         )
 
-    pov = ro.PatchOfValues(
-        values=ro.DoubleHdf5Array(
-            values=ro.Hdf5Dataset(
-                path_in_hdf_file=f"/RESQML/{str(prop_uuid)}/values",
-                hdf_proxy=ro.DataObjectReference(
-                    content_type=f"application/x-eml+xml;version={schema_version};type={get_data_object_type(epc)}",
-                    title=epc.citation.title,
-                    uuid=str(epc.uuid),
+
+    cprop0s, props = [], []
+    
+    for i in range( len(time_indices) if use_timeseries else 1 ):
+        if (not use_timeseries):
+            prop_uuid = prop_uuid0
+            prop = prop0
+        else:
+            prop_uuid = prop_uuids[time_indices[i]]
+            prop = rqp.Property(model, uuid=prop_uuid)
+
+        pov = ro.PatchOfValues(
+            values=ro.DoubleHdf5Array(
+                values=ro.Hdf5Dataset(
+                    path_in_hdf_file=f"/RESQML/{str(prop_uuid)}/values",
+                    hdf_proxy=ro.DataObjectReference(
+                        content_type=f"application/x-eml+xml;version={schema_version};type={get_data_object_type(epc)}",
+                        title=epc.citation.title,
+                        uuid=str(epc.uuid),
+                    ),
+                )
+            ) if continuous else
+            ro.IntegerHdf5Array(
+                values=ro.Hdf5Dataset(
+                    path_in_hdf_file=f"/RESQML/{str(prop_uuid)}/values",
+                    hdf_proxy=ro.DataObjectReference(
+                        content_type=f"application/x-eml+xml;version={schema_version};type={get_data_object_type(epc)}",
+                        title=epc.citation.title,
+                        uuid=str(epc.uuid),
+                    ),
                 ),
+                null_value=int(1e30),
             )
-        ) if continuous else
-        ro.IntegerHdf5Array(
-            values=ro.Hdf5Dataset(
-                path_in_hdf_file=f"/RESQML/{str(prop_uuid)}/values",
-                hdf_proxy=ro.DataObjectReference(
-                    content_type=f"application/x-eml+xml;version={schema_version};type={get_data_object_type(epc)}",
-                    title=epc.citation.title,
-                    uuid=str(epc.uuid),
-                ),
-            ),
-            null_value=int(1e30),
         )
-    )
 
-    if (continuous):
-        cprop0 = ro.ContinuousProperty(
-            schema_version=schema_version,
-            citation=create_common_citation(f"{prop_title}"),
-            uuid=str(prop.uuid),
-            uom=prop.uom(),
-            count=1,
-            indexable_element=prop.indexable_element(),
-            supporting_representation=ro.DataObjectReference(
-                content_type=f"application/x-resqml+xml;version={schema_version};type={get_data_object_type(uns)}",
-                title=uns.citation.title,
-                uuid=uns.uuid,
-            ),
-            property_kind=ro.LocalPropertyKind(
-                local_property_kind=ro.DataObjectReference(
-                    content_type=f"application/x-resqml+xml;version={schema_version};type={get_data_object_type(propertykind0)}",
-                    title=propertykind0.citation.title,
-                    uuid=propertykind0.uuid,
-                )
-            ) if (propertykind0 is not None) else ro.StandardPropertyKind(kind=prop.property_kind()),
-            minimum_value=[prop.minimum_value() or 0.0],
-            maximum_value=[prop.maximum_value() or 1.0],
-            facet=[ro.PropertyKindFacet(
-                facet=ro.Facet.WHAT,
-                value=prop_title,  # prop.facet(),
-            )],
-            patch_of_values=[pov],
-        )
-    else:
-        cprop0 = ro.DiscreteProperty(
-            schema_version=schema_version,
-            citation=create_common_citation(f"{prop_title}"),
-            uuid=str(prop.uuid),
-            # uom = prop.uom(),
-            count=1,
-            indexable_element=prop.indexable_element(),
-            supporting_representation=ro.DataObjectReference(
-                content_type=f"application/x-resqml+xml;version={schema_version};type={get_data_object_type(uns)}",
-                title=uns.citation.title,
-                uuid=uns.uuid,
-            ),
-            property_kind=ro.LocalPropertyKind(
-                local_property_kind=ro.DataObjectReference(
-                    content_type=f"application/x-resqml+xml;version={schema_version};type={get_data_object_type(propertykind0)}",
-                    title=propertykind0.citation.title,
-                    uuid=propertykind0.uuid,
-                )
-            ) if (propertykind0 is not None) else ro.StandardPropertyKind(kind=prop.property_kind()),
-            minimum_value=[int(prop.minimum_value() or 0)],
-            maximum_value=[int(prop.maximum_value() or 1)],
-            facet=[ro.PropertyKindFacet(
-                facet=ro.Facet.WHAT,
-                value=prop_title,  # prop.facet(),
-            )],
-            patch_of_values=[pov],
-        )
+        timeindex_ref = None
+        if use_timeseries:
+            time_index = time_indices[i]
+            timeindex_ref = ro.TimeIndex(
+                index = time_index,
+                time_series = ro.DataObjectReference(
+                    content_type=f"application/x-resqml+xml;version={schema_version};type={get_data_object_type(timeseries)}",
+                    title=timeseries.citation.title,
+                    uuid=timeseries.uuid,
+                )
+            )
+
+        r_uom = ro.ResqmlUom( value= uom_for_prop_title(prop_title) ) if (prop.uom() is None) else prop.uom()
+
+        if (continuous):
+            cprop0 = ro.ContinuousProperty(
+                schema_version=schema_version,
+                citation=create_common_citation(f"{prop_title}"),
+                uuid=str(prop.uuid),
+                uom = r_uom,
+                count=1,
+                indexable_element=prop.indexable_element(),
+                supporting_representation=ro.DataObjectReference(
+                    content_type=f"application/x-resqml+xml;version={schema_version};type={get_data_object_type(uns)}",
+                    title=uns.citation.title,
+                    uuid=uns.uuid,
+                ),
+                property_kind=ro.LocalPropertyKind(
+                    local_property_kind=ro.DataObjectReference(
+                        content_type=f"application/x-resqml+xml;version={schema_version};type={get_data_object_type(propertykind0)}",
+                        title=propertykind0.citation.title,
+                        uuid=propertykind0.uuid,
+                    )
+                ) if (propertykind0 is not None) else ro.StandardPropertyKind(kind=prop.property_kind()),
+                minimum_value=[prop.minimum_value() or 0.0],
+                maximum_value=[prop.maximum_value() or 1.0],
+                facet=[ro.PropertyKindFacet(
+                    facet=ro.Facet.WHAT,
+                    value=prop_title,  # prop.facet(),
+                )],
+                patch_of_values=[pov],
+                time_index=timeindex_ref,
+            )
+        else:
+            cprop0 = ro.DiscreteProperty(
+                schema_version=schema_version,
+                citation=create_common_citation(f"{prop_title}"),
+                uuid=str(prop.uuid),
+                # uom = prop.uom(),
+                count=1,
+                indexable_element=prop.indexable_element(),
+                supporting_representation=ro.DataObjectReference(
+                    content_type=f"application/x-resqml+xml;version={schema_version};type={get_data_object_type(uns)}",
+                    title=uns.citation.title,
+                    uuid=uns.uuid,
+                ),
+                property_kind=ro.LocalPropertyKind(
+                    local_property_kind=ro.DataObjectReference(
+                        content_type=f"application/x-resqml+xml;version={schema_version};type={get_data_object_type(propertykind0)}",
+                        title=propertykind0.citation.title,
+                        uuid=propertykind0.uuid,
+                    )
+                ) if (propertykind0 is not None) else ro.StandardPropertyKind(kind=prop.property_kind()),
+                minimum_value=[int(prop.minimum_value() or 0)],
+                maximum_value=[int(prop.maximum_value() or 1)],
+                facet=[ro.PropertyKindFacet(
+                    facet=ro.Facet.WHAT,
+                    value=prop_title,  # prop.facet(),
+                )],
+                patch_of_values=[pov],
+                time_index=timeindex_ref,
+            )
+        cprop0s.append(cprop0)
+        props.append(prop)
 
-    return cprop0, prop, propertykind0
+    return cprop0s, props, propertykind0
```

### Comparing `pyetp-0.0.4/pyproject.toml` & `pyetp-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyetp"
-version = "0.0.4"
+version = "0.0.5"
 description = "Interface with OSDU RDDMS using ETP protocol"
 authors = ["Adam Cheng <52572642+adamchengtkc@users.noreply.github.com>"]
 readme = "README.md"
 license = "LGPL-3.0-only"
 homepage = "https://github.com/equinor/pyetp"
 
 [tool.poetry.dependencies]
```

### Comparing `pyetp-0.0.4/PKG-INFO` & `pyetp-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyetp
-Version: 0.0.4
+Version: 0.0.5
 Summary: Interface with OSDU RDDMS using ETP protocol
 Home-page: https://github.com/equinor/pyetp
 License: LGPL-3.0-only
 Author: Adam Cheng
 Author-email: 52572642+adamchengtkc@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

