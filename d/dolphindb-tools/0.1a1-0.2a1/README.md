# Comparing `tmp/dolphindb_tools-0.1a1-py3-none-any.whl.zip` & `tmp/dolphindb_tools-0.2a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 20794 bytes, number of entries: 13
--rw-rw-r--  2.0 unx       27 b- defN 23-Sep-19 08:28 dolphindb_tools/__init__.py
--rw-rw-r--  2.0 unx      171 b- defN 23-Sep-19 08:28 dolphindb_tools/dataloader/__init__.py
--rw-rw-r--  2.0 unx       51 b- defN 23-Sep-19 08:28 dolphindb_tools/dataloader/config.py
--rw-rw-r--  2.0 unx    15756 b- defN 23-Sep-19 08:28 dolphindb_tools/dataloader/dataloader.py
--rw-rw-r--  2.0 unx     8463 b- defN 23-Sep-19 08:28 dolphindb_tools/dataloader/datamanager.py
--rw-rw-r--  2.0 unx    12702 b- defN 23-Sep-22 07:03 dolphindb_tools/dataloader/datasource.py
--rw-rw-r--  2.0 unx     9455 b- defN 23-Sep-19 08:28 dolphindb_tools/dataloader/helper.py
--rw-rw-r--  2.0 unx    12664 b- defN 23-Sep-19 08:28 dolphindb_tools/dataloader/utils.py
--rw-rw-r--  2.0 unx    11392 b- defN 23-Sep-27 06:10 dolphindb_tools-0.1a1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2042 b- defN 23-Sep-27 06:10 dolphindb_tools-0.1a1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Sep-27 06:10 dolphindb_tools-0.1a1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 23-Sep-27 06:10 dolphindb_tools-0.1a1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1174 b- defN 23-Sep-27 06:10 dolphindb_tools-0.1a1.dist-info/RECORD
-13 files, 74005 bytes uncompressed, 18800 bytes compressed:  74.6%
+Zip file size: 23170 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       27 b- defN 24-Apr-07 02:46 dolphindb_tools/__init__.py
+-rw-r--r--  2.0 unx      171 b- defN 24-Jan-04 02:50 dolphindb_tools/dataloader/__init__.py
+-rw-r--r--  2.0 unx       51 b- defN 24-Jan-04 02:50 dolphindb_tools/dataloader/config.py
+-rw-r--r--  2.0 unx    23404 b- defN 24-Apr-11 05:52 dolphindb_tools/dataloader/dataloader.py
+-rw-r--r--  2.0 unx     8463 b- defN 24-Jan-04 02:50 dolphindb_tools/dataloader/datamanager.py
+-rw-r--r--  2.0 unx    13144 b- defN 24-Apr-11 05:52 dolphindb_tools/dataloader/datasource.py
+-rw-r--r--  2.0 unx     9981 b- defN 24-Mar-06 06:33 dolphindb_tools/dataloader/helper.py
+-rw-r--r--  2.0 unx    13394 b- defN 24-Apr-08 03:50 dolphindb_tools/dataloader/utils.py
+-rw-r--r--  2.0 unx    11392 b- defN 24-Apr-11 05:52 dolphindb_tools-0.2a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2420 b- defN 24-Apr-11 05:52 dolphindb_tools-0.2a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 05:52 dolphindb_tools-0.2a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-11 05:52 dolphindb_tools-0.2a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1174 b- defN 24-Apr-11 05:52 dolphindb_tools-0.2a1.dist-info/RECORD
+13 files, 83729 bytes uncompressed, 21176 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: dolphindb_tools/dataloader/helper.py
 Comment: 
 
 Filename: dolphindb_tools/dataloader/utils.py
 Comment: 
 
-Filename: dolphindb_tools-0.1a1.dist-info/LICENSE
+Filename: dolphindb_tools-0.2a1.dist-info/LICENSE
 Comment: 
 
-Filename: dolphindb_tools-0.1a1.dist-info/METADATA
+Filename: dolphindb_tools-0.2a1.dist-info/METADATA
 Comment: 
 
-Filename: dolphindb_tools-0.1a1.dist-info/WHEEL
+Filename: dolphindb_tools-0.2a1.dist-info/WHEEL
 Comment: 
 
-Filename: dolphindb_tools-0.1a1.dist-info/top_level.txt
+Filename: dolphindb_tools-0.2a1.dist-info/top_level.txt
 Comment: 
 
-Filename: dolphindb_tools-0.1a1.dist-info/RECORD
+Filename: dolphindb_tools-0.2a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dolphindb_tools/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1-alpha1"
+__version__ = "0.2-alpha1"
```

## dolphindb_tools/dataloader/dataloader.py

```diff
@@ -1,45 +1,163 @@
 import copy
 import random
 from queue import Empty, Full, Queue
 from threading import Event, Thread
 from typing import List, Optional, Union
 
-import torch
+
 from dolphindb import session as Session
 
 from .config import TIMEOUT
 from .datamanager import DataManager
 from .datasource import DataRealSource
 from .helper import DataIndexHelper, RandomSampleHelper
 from .utils import (MetaSQL, SequentialSession, _generate_tablename,
-                    make_MetaSQL)
+                    make_MetaSQL, MODE_TYPE, import_framework)
+from . import utils
 
 
 class DDBDataLoader(object):
+    """The DDBDataLoader class is used to import data stored in DolphinDB for
+    machine learning.
+
+    Args:
+        ddbSession (Session): Session connection used to obtain data,
+        including contextual information required for training.
+
+        sql (str): metacode of SQL statements to extract data for training.
+        Currently TOP, LIMIT, GROUP BY and CONTEXT BY clauses are not supported.
+
+        targetCol (Union[List[str], str]): a list of str, indicating the column
+        name corresponding to y in the iteration.
+
+    Kwargs:
+        batchSize (int, optional): batch size that specifies the number of
+        messages in each batch of data. Defaults to 1.
+
+        shuffle (bool, optional): whether to randomly shuffle the data.
+        Defaults to False.
+
+        windowSize (Union[List[int], int, None], optional): the size of the
+        sliding window. If not specified, sliding window will not be used.
+        Defaults to None.
+        - If an integer (int) is specified, e.g., windowSize=3, the sliding
+        window size of x is 3 and the sliding window size of y is 1.
+        - If a list with 2 integers is specified, e.g., windowSize=[4, 2],
+        the sliding window size of x is 4 and the sliding window size of y is 2.
+
+        windowStride (Union[List[int], int, None], optional): sliding step of
+        the window. This parameter only takes effect when windowSize is specified.
+        Defaults to None.
+        - If an integer (int) is specified, e.g., windowStride=2, the sliding
+        step of x is 2 and the sliding step of y is 1.
+        - If a list with 2 integers is specified, e.g., windowStride=[3, 1],
+        the sliding step for x is 3 and the sliding step for y is 1.
+
+        inputCol (Optional[Union[List[str], str]], optional): a list of str,
+        indicating the column name corresponding to x in the iteration. If not
+        specified, it indicates all columns. Defaults to None.
+
+        excludeCol (Optional[Union[List[str], str]], optional): a list of str,
+        indicating the column names excluded by x in the iteration. Defaults to None.
+
+    Note:
+        - If inputCol is specified, x is the column corresponding to inputCol,
+        and y is the column corresponding to targetCol. excludeCol will not take effect.
+
+        - If inputCol is unspecified and excludeCol is specified, x is all columns
+        excluding excludeCol, and y is the column corresponding to targetCol.
+
+        - If neither inputCol or excludeCol is specified, x indicates all columns,
+        and y is the column corresponding to targetCol.
+
+    Kwargs:
+        repartitionCol (str, optional): column used to further split the grouped
+        query into subqueries. Defaults to None.
+
+        repartitionScheme (List[str], optional): a list of str indicating the partition
+        values. Data is further filtered and split based on the list element and
+        repartitionCol column. Defaults to None.
+
+        groupCol (str, optional): column used to divide the query into groups.
+        Defaults to None.
+
+        groupScheme (List[str], optional): a list of str indicating the group values.
+        Data is further filtered and split based on the list element and groupCol
+        column. Defaults to None.
+
+    Note:
+        - The parameters repartitionCol and repartitionScheme can be used if a single
+        partition has a large amount of data that cannot be directly processed.
+        By filtering the data based on the value of repartitionScheme, the data can be
+        split into multiple subpartitions, each of which will be ordered in the
+        repartitionScheme. For example, if repartitionCol is date(TradeTime) and
+        repartitionScheme is ["2020.01.01", "2020.01.02", "2020.01.03"], the data will
+        be subdivided into three partitions, each partition corresponding to a date value.
+
+        - Different from repartitionCol/repartitionScheme, no cross-group data will be
+        generated if groupCol/groupScheme is used. For example, if groupCol is Code
+        and groupScheme is ["`000001.SH", "`000002.SH", "`000003. SH"], the data will be
+        divided into three groups, each group corresponding to a stock code.
+
+    Kwargs:
+        seed (Optional[int], optional): random seed, which only takes effect within
+        the DDBDataLoader object. Defaults to None, meaning no random seed is specified.
+
+        dropLast (bool, optional): whether to discard the last batch of messages
+        that is less than batchSize when batchSize cannot divide the size of the
+        query result. Defaults to False, meaning that the last batch that is less
+        than batchSize will not be discarded.
+
+        offset (int, optional): a non-negative integer indicating the number of rows
+        y is offset from x. If windowSize is specified, the default value is the
+        window size of x. If windowSize is not specified, the default value is 0,
+        meaning that the training data are all in the same row.
+
+        mode (str, optional): the deep learning framework used by DDBDataLoader.
+        Its value can be "pytorch" (default) or "tensorflow".
+
+        device (Optional[str], optional): device on which the tensor will be created.
+        Set this to "cuda" or device name supported by torch.device and tf.device
+        to create tensors on the GPU.
+
+        prefetchBatch (int, optional): the number of batches preloaded in the
+        background. Defaults to 1.
+
+        prepartitionNum (int, optional): the number of preloaded partitions for
+        each data source. The worker thread will preload the partition into memory
+        in the background. Defaults to 2. Note that too many preloaded partitions
+        may result in insufficient memory.
+
+        groupPoolSize (int, optional): the number of data sources selected for data
+        preparation if groupCol and groupScheme are specified. If a selected source
+        is used, a new one will be added until all data sources are used.
+        Defaults to 3.
+    """
     def __init__(
         self,
         ddbSession: Session,
         sql: str,
-        targetCol: List[str],
+        targetCol: Union[List[str], str],
         batchSize: int = 1,
         shuffle: bool = False,
         windowSize: Union[List[int], int, None] = None,
         windowStride: Union[List[int], int, None] = None,
         *,
-        inputCol: Optional[List[str]] = None,
-        excludeCol: Optional[List[str]] = None,
+        inputCol: Optional[Union[List[str], str]] = None,
+        excludeCol: Optional[Union[List[str], str]] = None,
         repartitionCol: str = None,
         repartitionScheme: List[str] = None,
         groupCol: str = None,
         groupScheme: List[str] = None,
         seed: Optional[int] = None,
         dropLast: bool = False,
         offset: int = None,
-        device: str = "cpu",
+        mode: str = "pytorch",
+        device: Optional[str] = None,
         prefetchBatch: int = 1,
         prepartitionNum: int = 2,
         groupPoolSize: int = 3,
         **kwargs
     ):
         if not isinstance(ddbSession, Session):
             raise TypeError("The type of ddbSession must be dolphindb.Session.")
@@ -51,30 +169,42 @@
         self.group_scheme = groupScheme
 
         if repartitionCol is not None and not isinstance(repartitionCol, str):
             raise TypeError("The type of repartitionCol must be str.")
         self.repartition_col = repartitionCol
         self.repartition_scheme = repartitionScheme
 
+        if not isinstance(mode, str):
+            raise TypeError("The type of mode must be str.")
+
+        if mode == MODE_TYPE.PYTORCH.value:
+            self.mode = MODE_TYPE.PYTORCH
+            import_framework(MODE_TYPE.PYTORCH)
+        elif mode == MODE_TYPE.TENSORFLOW.value:
+            self.mode = MODE_TYPE.TENSORFLOW
+            import_framework(MODE_TYPE.TENSORFLOW)
+        else:
+            raise ValueError("The value of mode must be 'pytorch' or 'tensorflow'.")
+
         self.device = device
 
         if not isinstance(prefetchBatch, int):
-            raise TypeError("The type of prefetchBatch must be str.")
+            raise TypeError("The type of prefetchBatch must be int.")
         if prefetchBatch <= 0:
             raise ValueError("The value of prefetchBatch must be greater than 0.")
         self.prefetch = prefetchBatch
 
         if not isinstance(prepartitionNum, int):
-            raise TypeError("The type of prepartitionNum must be str.")
+            raise TypeError("The type of prepartitionNum must be int.")
         if prepartitionNum <= 0:
             raise ValueError("The value of prepartitionNum must be greater than 0.")
         self.prepartition_num = prepartitionNum
 
         if not isinstance(groupPoolSize, int):
-            raise TypeError("The type of groupPoolSize must be str.")
+            raise TypeError("The type of groupPoolSize must be int.")
         if groupPoolSize <= 0:
             raise ValueError("The value of groupPoolSize must be greater than 0.")
         self.grouppool_size = groupPoolSize
 
         if not isinstance(sql, str):
             raise TypeError("The type of sql must be str.")
         sql = make_MetaSQL(ddbSession, sql)
@@ -83,39 +213,39 @@
 
         if windowSize is None:
             self.window_size = [None, None]
         elif isinstance(windowSize, int):
             self.window_size = [windowSize, 1]
         elif isinstance(windowSize, list):
             if len(windowSize) != 2:
-                raise ValueError("windowSize must be like int or [int, int].")
+                raise ValueError("windowSize must be an int or a list with 2 int.")
             self.window_size = windowSize
         else:
-            raise ValueError("windowSize must be like int or [int, int].")
+            raise ValueError("windowSize must be an int or a list with 2 int.")
 
         if windowStride is None:
             self.window_stride = [None, None]
         elif isinstance(windowStride, int):
             self.window_stride = [windowStride, 1]
         elif isinstance(windowStride, list):
             if len(windowStride) != 2:
-                raise ValueError("windowStride must be like int or [int, int].")
+                raise ValueError("windowStride must be an int or a list with 2 int.")
             self.window_stride = windowStride
         else:
-            raise ValueError("windowStride must be like int or [int, int].")
+            raise ValueError("windowStride must be an int or a list with 2 int.")
 
         if offset is None:
             if self.window_size[0] is not None:
                 offset = self.window_size[0]
             else:
                 offset = 0
         if not isinstance(offset, int):
             raise TypeError("The type of offset must be int.")
         if offset < 0:
-            raise ValueError("The value of offset must not be less than 0.")
+            raise ValueError("The value of offset must be no less than 0.")
         self.offset = offset
 
         if not isinstance(batchSize, int):
             raise TypeError("The type of batchSize must be int.")
         if batchSize <= 0:
             raise ValueError("The value of batchSize must be greater than 0.")
         self.batch_size = batchSize
@@ -123,30 +253,28 @@
         self.shuffle = shuffle
         self.drop_last = dropLast
 
         if inputCol is not None:
             if isinstance(inputCol, str):
                 inputCol = [inputCol]
             if not isinstance(inputCol, list):
-                raise TypeError("The type of inputCol must be str or List[str].")
+                raise TypeError("The type of inputCol must be str or list of str.")
         self.input_cols = inputCol
 
-        if targetCol is None:
-            raise ValueError("Parameter targetCol must be specified.")
         if isinstance(targetCol, str):
             targetCol = [targetCol]
         if not isinstance(targetCol, list):
-            raise TypeError("The type of targetCol must be str or List[str].")
+            raise TypeError("The type of targetCol must be str or list of str.")
         self.target_cols = targetCol
 
         if excludeCol is not None:
             if isinstance(excludeCol, str):
                 excludeCol = [excludeCol]
             if not isinstance(excludeCol, list):
-                raise TypeError("The type of excludeCol must be str or List[str].")
+                raise TypeError("The type of excludeCol must be str or list of str.")
         self.exclude_cols = excludeCol if excludeCol is not None else []
 
         if "verbose" in kwargs:
             self.verbose = bool(kwargs["verbose"])
         else:
             self.verbose = False
 
@@ -158,34 +286,34 @@
 
     def _take_group_effect(self, group_col, group_scheme, sql: MetaSQL):
         if group_col is None and group_scheme is None:
             return [sql]
         if not (group_col and group_scheme):
             raise ValueError("Both groupCol and groupScheme must be specified simultaneously.")
         if not isinstance(group_col, str):
-            raise TypeError("groupCol must be str.")
+            raise TypeError("The type of groupCol must be str.")
         if not isinstance(group_scheme, list):
-            raise TypeError("groupScheme must be list.")
+            raise TypeError("The type of groupScheme must be list of str.")
         res_sqls = []
         for scheme in group_scheme:
             scheme = str(scheme)
             res_sql = copy.deepcopy(sql)
             res_sql.add_where([f"< {group_col} = {scheme} >"])
             res_sqls.append(res_sql)
         return res_sqls
 
     def _take_repartition_effect(self, repartition_col, repartition_scheme, sqls):
         if repartition_col is None and repartition_scheme is None:
             return [[sql] for sql in sqls]
         if not (repartition_col and repartition_scheme):
             raise ValueError("Both repartitionCol and repartitionScheme must be specified simultaneously.")
         if not isinstance(repartition_col, str):
-            raise TypeError("repartitionCol must be str.")
+            raise TypeError("The type of repartitionCol must be str.")
         if not isinstance(repartition_scheme, list):
-            raise TypeError("repartitionScheme must be list.")
+            raise TypeError("The type of repartitionScheme must be list of str.")
         res_sqls = [[] for _ in range(len(sqls))]
         for i, sql in enumerate(sqls):
             for scheme in repartition_scheme:
                 res_sql = copy.deepcopy(sql)
                 res_sql.add_where([f"< {repartition_col} = {scheme} >"])
                 res_sqls[i].append(res_sql)
         return res_sqls
@@ -234,18 +362,24 @@
             ndata = self.queue.get()
             self.queue.task_done()
             if ndata is None:
                 break
             elif isinstance(ndata, Exception):
                 raise ndata
             x, y = ndata
-            if self.window_size[0] is None:
-                x = torch.squeeze(x, dim=1)
-            if self.window_size[1] is None:
-                y = torch.squeeze(y, dim=1)
+            if self.mode == MODE_TYPE.PYTORCH:
+                if self.window_size[0] is None:
+                    x = utils.torch.squeeze(x, dim=1)
+                if self.window_size[1] is None:
+                    y = utils.torch.squeeze(y, dim=1)
+            elif self.mode == MODE_TYPE.TENSORFLOW:
+                if self.window_size[0] is None:
+                    x = utils.tf.squeeze(x, axis=1)
+                if self.window_size[1] is None:
+                    y = utils.tf.squeeze(y, axis=1)
             yield x, y
         self.back_thread.join()
 
     def _prepare_next_batch(self):
         try:
             dm_pool_size = self.grouppool_size
             dms = copy.deepcopy(self.dms)
@@ -261,34 +395,45 @@
             while len(generators) != 0:
                 ndata = []
                 try:
                     if self.shuffle:
                         random_generator = self.random_ins.choice(generators)
                     else:
                         random_generator = generators[0]
-                    data_row = [next(dm) for dm in random_generator]
+                    data_row = [next(dm[0]) for dm in random_generator]
                     for i, data in enumerate(data_row):
                         data_rows[i].append(data)
-                        if len(data_rows[i]) >= self.batch_size:
-                            ndata.append(torch.stack([_.data for _ in data_rows[i]]))
-                            data_rows[i] = []
+                        if self.mode == MODE_TYPE.PYTORCH:
+                            if len(data_rows[i]) >= self.batch_size:
+                                ndata.append(utils.torch.stack([_ for _ in data_rows[i]]))
+                                data_rows[i] = []
+                        elif self.mode == MODE_TYPE.TENSORFLOW:
+                            if len(data_rows[i]) >= self.batch_size:
+                                ndata.append(utils.tf.stack([_ for _ in data_rows[i]]))
+                                data_rows[i] = []
                     if len(ndata) > 0:
                         self.queue.put(ndata)
                 except StopIteration:
+                    for dm in random_generator:
+                        dm[1].exit()
                     generators.remove(random_generator)
                     if all_flag:
                         try:
                             new_generator = next(dm_iter)
                             generators.append(new_generator)
                         except StopIteration:
                             all_flag = False
             if len(data_rows[0]) and not self.drop_last:
                 ndata = []
-                for data in data_rows:
-                    ndata.append(torch.stack([_.data for _ in data]))
+                if self.mode == MODE_TYPE.PYTORCH:
+                    for data in data_rows:
+                        ndata.append(utils.torch.stack([_.data for _ in data]))
+                elif self.mode == MODE_TYPE.TENSORFLOW:
+                    for data in data_rows:
+                        ndata.append(utils.tf.stack([_.numpy() for _ in data]))
                 self.queue.put(ndata)
             self.queue.put(None)
             self.dm_thread.join()
         except Exception as e:
             exit_flag.set()
             self.queue.put(e)
             self.dm_thread.join()
@@ -348,25 +493,25 @@
 
         ds_input = DataRealSource(
             self.s, sqls,
             "INPUT", self.func_name,
             input_cols=self.input_cols,
             target_cols=self.target_cols,
             exclude_cols=self.exclude_cols,
-            offset=0, device=self.device,
+            offset=0, data_mode=self.mode, device=self.device,
             q_size=self.prepartition_num,
             verbose=self.verbose,
         )
         ds_target = DataRealSource(
             self.s, sqls,
             "TARGET", self.func_name,
             input_cols=self.input_cols,
             target_cols=self.target_cols,
             exclude_cols=self.exclude_cols,
-            offset=self.offset, device=self.device,
+            offset=self.offset, data_mode=self.mode, device=self.device,
             q_size=self.prepartition_num,
             verbose=self.verbose,
         )
         data_num_input = (ds_input.data_len() - input_window_size) // input_window_stride + 1
         data_num_target = (ds_target.data_len() - target_window_size) // target_window_stride + 1
 
         if self.shuffle and data_num_input <= data_num_target:
@@ -392,9 +537,9 @@
 
     def _start_data_manager(self, dm_pair, exit_flag: Event):
         dms = []
         for dm_msg in dm_pair:
             ds, index, wsize, wstride = dm_msg
             dm = DataManager(ds, index, wsize, wstride, exit_flag=exit_flag)
             dm.start()
-            dms.append(iter(dm))
+            dms.append([iter(dm), dm])
         return dms
```

## dolphindb_tools/dataloader/datasource.py

```diff
@@ -1,22 +1,24 @@
 import copy
 import time
 from queue import Empty, Full, Queue
 from threading import Event, Thread
 from typing import List
 
 import numpy as np
-import torch
+
 from dolphindb import session as Session
 
 from .config import FORCEPARTITION, TIMEOUT, TRY_MAX_TIME
-from .helper import DataListCeil, DataTensorCeil
-from .utils import (GROUP_FLAG, LOAD_MODE, ExitStatus, MetaSQL,
+from .helper import DataListCeil, DataPytorchCeil, DataTensorflowCeil
+from .utils import (GROUP_FLAG, LOAD_MODE, ExitStatus, MetaSQL, MODE_TYPE,
                     _check_category, _generate_tablename, _release_table)
 
+from . import utils
+
 
 class DataSource(object):
     prefix_sum: List[int]
 
     def __getitem__(self, index):
         raise NotImplementedError
 
@@ -126,27 +128,28 @@
 
 class DataRealSource(DataSource):
     def __init__(
         self, sess: Session, sqls: List[MetaSQL],
         sql_mode, func_name: str,
         *,
         input_cols=None, target_cols=None, exclude_cols=None,
-        offset: int = 0, q_size: int = 10, device: str = "cpu",
+        offset: int = 0, q_size: int = 10, data_mode: MODE_TYPE = MODE_TYPE.PYTORCH, device: str = "cpu",
         verbose: bool = False,
     ) -> None:
         self.s = sess
         self.sqls = sqls
         self.mode = LOAD_MODE.UNKNOWN
         self.forcePartition = FORCEPARTITION
         self.func_name = func_name
         self.verbose = verbose
         self.release_list = []
         ds_names = [self._check_sql(sql) for sql in sqls]
         self.sql_mode = sql_mode
         self.offset = offset
+        self.data_mode = data_mode
         self.device = device
         self.input_cols = input_cols
         self.target_cols = target_cols
         self.exclude_cols = exclude_cols
         self.q_size = q_size
 
         self.exit_flag = Event()
@@ -255,15 +258,18 @@
                 res = self.q.get(timeout=TIMEOUT)
                 get_flag = True
                 if isinstance(res, Exception):
                     raise res
                 self.q.task_done()
             except Empty:
                 pass
-        return DataTensorCeil(res)
+        if self.data_mode == MODE_TYPE.PYTORCH:
+            return DataPytorchCeil(res)
+        else:
+            return DataTensorflowCeil(res)
 
     def _check_sql(self, sql: MetaSQL):
         counts = None
         try:
             ds_name = _generate_tablename("tds_api")
             self.release_list.append(ds_name)
             if sql.groupflag == GROUP_FLAG.PIVOTBY.value:
@@ -321,15 +327,19 @@
         if ndim == 2:
             array = array.T
         elif ndim == 3:
             array = np.transpose(array, (1, 0, 2))
         else:
             raise RuntimeError(f"Please check your sql, expected data ndim=2/3, but get {ndim}.")
 
-        ans = torch.tensor(array, device=self.device)
+        if self.data_mode == MODE_TYPE.PYTORCH:
+            ans = utils.torch.tensor(array, device=self.device)
+        elif self.data_mode == MODE_TYPE.TENSORFLOW:
+            with utils.tf.device(self.device):
+                ans = utils.tf.convert_to_tensor(array)
         return ndim, ans
 
     def _generate_colnames(self, temp_name):
         if hasattr(self, "schema"):
             return
         schema = self.s.run(f"schema({temp_name})")["colDefs"]
         all_cols = list(schema[schema["typeInt"].apply(_check_category) == 1]["name"].values)
```

## dolphindb_tools/dataloader/helper.py

```diff
@@ -1,15 +1,19 @@
 import copy
 import random
 from math import ceil, gcd
 from typing import List
 
 import numpy as np
-import torch
-from torch import Tensor
+# import torch
+# from torch import Tensor
+# import tensorflow as tf
+from . import utils
+# from .utils import torch,tf
+# Tensor=torch.Tensor
 
 
 class QueryTree:
     def __init__(self, size):
         self.pa = np.arange(size + 1, dtype="int64")
 
     def find(self, x):
@@ -58,15 +62,15 @@
 
     def __str__(self) -> str:
         return str(self.data)
 
     def __repr__(self) -> str:
         return str(self)
 
-    def get_data(self) -> Tensor:
+    def get_data(self):
         raise NotImplementedError
 
 
 def get_data_func(res_L, res_R):
     def datafunc(iv, islower):
         if islower:
             return (iv.begin, res_L, iv.data[2][:res_L-iv.begin])
@@ -86,31 +90,47 @@
     def cat(cls, datas: List[DataCeil]):
         res = DataListCeil([])
         for data in datas:
             if data is not None:
                 res = res + data
         return res
 
-    def get_data(self) -> Tensor:
-        return torch.tensor(self.data)
+    def get_data(self):
+        return utils.torch.tensor(self.data)
 
 
-class DataTensorCeil(DataCeil):
+class DataPytorchCeil(DataCeil):
 
     def __init__(self, data) -> None:
         super().__init__(data)
 
     def __add__(self, other):
-        return DataTensorCeil(torch.cat([self.data, other.data], 0))
+        return DataPytorchCeil(utils.torch.cat([self.data, other.data], 0))
 
     @classmethod
     def cat(cls, datas: List[DataCeil]):
-        return DataTensorCeil(torch.cat([_.data for _ in datas if _ is not None], 0))
+        return DataPytorchCeil(utils.torch.cat([_.data for _ in datas if _ is not None], 0))
 
-    def get_data(self) -> Tensor:
+    def get_data(self):
+        return self.data
+
+
+class DataTensorflowCeil(DataCeil):
+
+    def __init__(self, data) -> None:
+        super().__init__(data)
+
+    def __add__(self, other):
+        return DataTensorflowCeil(utils.tf.concat([self.data, other.data], axis=0))
+
+    @classmethod
+    def cat(cls, datas: List[DataCeil]):
+        return DataTensorflowCeil(utils.tf.concat([_.data for _ in datas if _ is not None], axis=0))
+
+    def get_data(self):
         return self.data
 
 
 class Interval:
     def __init__(self, left, right) -> None:
         self.left = left
         self.right = right
```

## dolphindb_tools/dataloader/utils.py

```diff
@@ -1,19 +1,32 @@
 from enum import Enum
 from threading import Lock
 from typing import Union, List, Optional
 import re
 import uuid
+import importlib
 
 from dolphindb import session as Session
 from dolphindb.settings import DT_VOID, DT_BOOL, DT_CHAR, DT_SHORT, DT_INT, DT_LONG
 from dolphindb.settings import DT_DATE, DT_MONTH, DT_TIME, DT_MINUTE, DT_SECOND, DT_DATETIME, DT_TIMESTAMP, DT_NANOTIME, DT_NANOTIMESTAMP
 from dolphindb.settings import DT_FLOAT, DT_DOUBLE, DT_SYMBOL, DT_STRING, DT_UUID, DT_DATEMINUTE, DT_DATEHOUR, DT_ANY
 from dolphindb.settings import DT_IPADDR, DT_INT128, DT_DECIMAL32, DT_DECIMAL64, DT_BLOB, ARRAY_TYPE_BASE
 
+try:
+    global torch
+    torch = __import__("torch")
+except ModuleNotFoundError:
+    torch = None
+
+try:
+    global tf
+    tf = __import__("tensorflow")
+except ModuleNotFoundError:
+    tf = None
+
 
 def _generate_tablename(tableName=None):
     if tableName is None:
         return "TMP_TBL_" + uuid.uuid4().hex[:8]
     else:
         return tableName + "_TMP_TBL_" + uuid.uuid4().hex[:8]
 
@@ -37,14 +50,32 @@
     MIXED = 7
     BINARY = 8
     COMPLEX = 9
     ARRAY = 10
     DENARY = 11
 
 
+class MODE_TYPE(Enum):
+    PYTORCH = 'pytorch'
+    TENSORFLOW = 'tensorflow'
+
+
+def import_framework(framework):
+    if framework == MODE_TYPE.PYTORCH:
+        global torch
+        if torch is None:
+            torch = importlib.import_module('torch')
+    elif framework == MODE_TYPE.TENSORFLOW:
+        global tf
+        if tf is None:
+            tf = importlib.import_module("tensorflow")
+    else:
+        raise ValueError("The value of mode must be pytorch or tensorflow.No AI framework was imported.")
+    
+    
 def getCategory(data_type):
     if data_type in [
         DT_TIME, DT_SECOND, DT_MINUTE, DT_DATE,
         DT_DATEHOUR, DT_DATEMINUTE, DT_DATETIME, DT_MONTH,
         DT_NANOTIME, DT_NANOTIMESTAMP, DT_TIMESTAMP,
     ]:
         return DATA_CATEGORY.TEMPORAL
```

## Comparing `dolphindb_tools-0.1a1.dist-info/LICENSE` & `dolphindb_tools-0.2a1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dolphindb_tools-0.1a1.dist-info/METADATA` & `dolphindb_tools-0.2a1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 Metadata-Version: 2.1
 Name: dolphindb-tools
-Version: 0.1a1
+Version: 0.2a1
 Summary: A tool package based on DolphinDB Python API.
 Home-page: https://www.dolphindb.com
 Author: DolphinDB, Inc.
 Author-email: support@dolphindb.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dolphindb (>=1.30.19.4)
+Requires-Dist: dolphindb >=1.30.19.4
 Requires-Dist: intervaltree
-Requires-Dist: numpy (>=1.18.0)
-Requires-Dist: pandas (>=1.0.0)
-Requires-Dist: torch
+Requires-Dist: numpy >=1.18.0
+Requires-Dist: pandas >=1.0.0
+Provides-Extra: pytorch
+Requires-Dist: torch ; extra == 'pytorch'
+Provides-Extra: tensorflow
+Requires-Dist: tensorflow ; extra == 'tensorflow'
 
 # dolphindb-tools
 
 DolphinDB Python Tool Collection
 
 ## How to Install
-
 ```
 pip install dolphindb-tools
 ```
-
+For installing dolphindb-tools with support for PyTorch, use the following command:
+```
+pip install dolphindb-tools[pytorch]
+```
+For installing dolphindb-tools with support for tensorflow, use the following command:
+```
+pip install dolphindb-tools[tensorflow]
+```
 ## Example
 
 ```
 import dolphindb as ddb
 from dolphindb_tools.dataloader import DDBDataLoader
 
 sess = ddb.session()
```

## Comparing `dolphindb_tools-0.1a1.dist-info/RECORD` & `dolphindb_tools-0.2a1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-dolphindb_tools/__init__.py,sha256=wlwKUhF5nFZ4uZ4lbk4qstHp5oSkEGi31R18cyMJWSQ,27
+dolphindb_tools/__init__.py,sha256=H5c6HnNF__zQOuWF65_jZJa8iGb7Aisd9UQEr2LnR3U,27
 dolphindb_tools/dataloader/__init__.py,sha256=_av_VYrZ7Twx0tgElcbVqRZcsMJoBNl99T4U2m9ldoI,171
 dolphindb_tools/dataloader/config.py,sha256=4cNf0c_WCdcr79YCptQylm0MHnGsdUcGqH1gIVjWsW8,51
-dolphindb_tools/dataloader/dataloader.py,sha256=_oNzRYbQ-krT7izcxZObpRannT4aBZ8BdYWYqiyC7fQ,15756
+dolphindb_tools/dataloader/dataloader.py,sha256=VrNDRrBy714uTzYdLCikO0kMfKrekmWwPMjBb9sf0z4,23404
 dolphindb_tools/dataloader/datamanager.py,sha256=yjMyEO4gS4MqTpv959mgFQb3BlMoHe-RGGnDxotJam0,8463
-dolphindb_tools/dataloader/datasource.py,sha256=cBDlI51bIxmDiM1OsOQCCjUFGZ2keBqjeuR4LPhk5O8,12702
-dolphindb_tools/dataloader/helper.py,sha256=tgUEAcC4p0Cw6nzLbe7sBtiGya-6nUxy-agZkiSAN6g,9455
-dolphindb_tools/dataloader/utils.py,sha256=XOLtiKh6vnbfJ2qKWmQISUpOXD5V40Sc0MRFfHWjQV0,12664
-dolphindb_tools-0.1a1.dist-info/LICENSE,sha256=djE9fEYevJ0JwCBOQhjt9qmG6RyC8gP5GF5jCeIVjbY,11392
-dolphindb_tools-0.1a1.dist-info/METADATA,sha256=4Kri8RtpWYS5RKsA2AYUZPZiUi1801KkgfM0MDaJCp8,2042
-dolphindb_tools-0.1a1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-dolphindb_tools-0.1a1.dist-info/top_level.txt,sha256=lb7oEzXGajAcaYWSgrxQK4foTKDWNcrwgllE_heJwjA,16
-dolphindb_tools-0.1a1.dist-info/RECORD,,
+dolphindb_tools/dataloader/datasource.py,sha256=YppQe3tv7_cRa--El09H-NVYqza6SqBqWo8303o3_UU,13144
+dolphindb_tools/dataloader/helper.py,sha256=ci-V3Axd6RhGBshp0EdJa6P2KFR-jy5zMo1g5vLajNI,9981
+dolphindb_tools/dataloader/utils.py,sha256=9o11sGSh9XxmfODM1NYaINet3eCXsCJeYMiRVxmD9oU,13394
+dolphindb_tools-0.2a1.dist-info/LICENSE,sha256=djE9fEYevJ0JwCBOQhjt9qmG6RyC8gP5GF5jCeIVjbY,11392
+dolphindb_tools-0.2a1.dist-info/METADATA,sha256=quQRJENslYRRM9zXmNlzDV3jBcjX5DjhkFGpZWpQavE,2420
+dolphindb_tools-0.2a1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+dolphindb_tools-0.2a1.dist-info/top_level.txt,sha256=lb7oEzXGajAcaYWSgrxQK4foTKDWNcrwgllE_heJwjA,16
+dolphindb_tools-0.2a1.dist-info/RECORD,,
```

