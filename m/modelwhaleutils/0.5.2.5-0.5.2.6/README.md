# Comparing `tmp/modelwhaleutils-0.5.2.5.tar.gz` & `tmp/modelwhaleutils-0.5.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelwhaleutils-0.5.2.5.tar", last modified: Fri Mar  1 10:50:52 2024, max compression
+gzip compressed data, was "modelwhaleutils-0.5.2.6.tar", last modified: Wed Apr 17 08:31:17 2024, max compression
```

## Comparing `modelwhaleutils-0.5.2.5.tar` & `modelwhaleutils-0.5.2.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 yuanyuan  (1001) yuanyuan  (1001)        0 2024-03-01 10:50:52.377969 modelwhaleutils-0.5.2.5/
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)      370 2024-03-01 10:50:52.377969 modelwhaleutils-0.5.2.5/PKG-INFO
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)     3078 2024-03-01 10:32:13.000000 modelwhaleutils-0.5.2.5/README.md
-drwxrwxr-x   0 yuanyuan  (1001) yuanyuan  (1001)        0 2024-03-01 10:50:52.373969 modelwhaleutils-0.5.2.5/modelwhaleutils.egg-info/
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)      370 2024-03-01 10:50:52.000000 modelwhaleutils-0.5.2.5/modelwhaleutils.egg-info/PKG-INFO
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)      360 2024-03-01 10:50:52.000000 modelwhaleutils-0.5.2.5/modelwhaleutils.egg-info/SOURCES.txt
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)        1 2024-03-01 10:50:52.000000 modelwhaleutils-0.5.2.5/modelwhaleutils.egg-info/dependency_links.txt
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)       42 2024-03-01 10:50:52.000000 modelwhaleutils-0.5.2.5/modelwhaleutils.egg-info/requires.txt
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)        8 2024-03-01 10:50:52.000000 modelwhaleutils-0.5.2.5/modelwhaleutils.egg-info/top_level.txt
-drwxrwxr-x   0 yuanyuan  (1001) yuanyuan  (1001)        0 2024-03-01 10:50:52.377969 modelwhaleutils-0.5.2.5/mwutils/
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)        0 2024-03-01 10:32:13.000000 modelwhaleutils-0.5.2.5/mwutils/__init__.py
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)     1580 2024-03-01 10:32:13.000000 modelwhaleutils-0.5.2.5/mwutils/keras.py
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)     4062 2024-03-01 10:32:13.000000 modelwhaleutils-0.5.2.5/mwutils/logs.py
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)    21952 2024-03-01 10:32:13.000000 modelwhaleutils-0.5.2.5/mwutils/run.py
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)     6285 2024-03-01 10:32:13.000000 modelwhaleutils-0.5.2.5/mwutils/sys_stat.py
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)     1163 2024-03-01 10:32:13.000000 modelwhaleutils-0.5.2.5/mwutils/tf_utils.py
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)      562 2024-03-01 10:32:13.000000 modelwhaleutils-0.5.2.5/mwutils/torch_utils.py
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)     5203 2024-03-01 10:32:13.000000 modelwhaleutils-0.5.2.5/mwutils/utils.py
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)       38 2024-03-01 10:50:52.377969 modelwhaleutils-0.5.2.5/setup.cfg
--rw-rw-r--   0 yuanyuan  (1001) yuanyuan  (1001)      544 2024-03-01 10:32:44.000000 modelwhaleutils-0.5.2.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 08:31:17.097742 modelwhaleutils-0.5.2.6/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3718 2024-04-17 08:31:17.097742 modelwhaleutils-0.5.2.6/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3078 2024-04-17 06:27:25.000000 modelwhaleutils-0.5.2.6/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 08:31:17.097742 modelwhaleutils-0.5.2.6/modelwhaleutils.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3718 2024-04-17 08:31:17.000000 modelwhaleutils-0.5.2.6/modelwhaleutils.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      375 2024-04-17 08:31:17.000000 modelwhaleutils-0.5.2.6/modelwhaleutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-17 08:31:17.000000 modelwhaleutils-0.5.2.6/modelwhaleutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       42 2024-04-17 08:31:17.000000 modelwhaleutils-0.5.2.6/modelwhaleutils.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2024-04-17 08:31:17.000000 modelwhaleutils-0.5.2.6/modelwhaleutils.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 08:31:17.093742 modelwhaleutils-0.5.2.6/mwutils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 06:27:25.000000 modelwhaleutils-0.5.2.6/mwutils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1580 2024-04-17 06:27:25.000000 modelwhaleutils-0.5.2.6/mwutils/keras.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4157 2024-04-17 07:41:48.000000 modelwhaleutils-0.5.2.6/mwutils/logs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22262 2024-04-17 07:41:22.000000 modelwhaleutils-0.5.2.6/mwutils/run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6287 2024-04-17 07:41:15.000000 modelwhaleutils-0.5.2.6/mwutils/sys_stat.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1163 2024-04-17 06:27:25.000000 modelwhaleutils-0.5.2.6/mwutils/tf_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      562 2024-04-17 06:27:25.000000 modelwhaleutils-0.5.2.6/mwutils/torch_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5213 2024-04-17 07:00:37.000000 modelwhaleutils-0.5.2.6/mwutils/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      622 2024-04-17 08:31:09.000000 modelwhaleutils-0.5.2.6/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-17 08:31:17.097742 modelwhaleutils-0.5.2.6/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      544 2024-04-17 07:46:46.000000 modelwhaleutils-0.5.2.6/setup.py
```

### Comparing `modelwhaleutils-0.5.2.5/README.md` & `modelwhaleutils-0.5.2.6/README.md`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.2.5/mwutils/keras.py` & `modelwhaleutils-0.5.2.6/mwutils/keras.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.2.5/mwutils/logs.py` & `modelwhaleutils-0.5.2.6/mwutils/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,52 +22,53 @@
             f.write(json.dumps(entry))
 
 
 def append_logs_buf_to_remote(logs_buf, name, metadata, post_addr):
     json_struct = {"logs": logs_buf, "phase": name, "metadata": metadata}
     # try 3 times
     for _ in range(3):
-        print('append log', name)
+        # print('append log', name)
         r = requests.post(post_addr, json=json_struct, headers={"Authorization": jwt.encode(
             {"whatever": "1"}, "857851b2-c28c-4d94-83c8-f607b50ccd03")})
         if r.status_code >= 400:
             # something wrong
             jb = ''
             try:
                 jb = r.json()
             except:
                 pass
-            print("resp:", r)
-            warnings.warn("code: {}, resp.json: {}, resp.text: {}".format(
-                r.status_code, jb, r.text))
+            # print("resp:", r)
+            # warnings.warn("code: {}, resp.json: {}, resp.text: {}".format(
+            #     r.status_code, jb, r.text))
         else:
             return True
     return False
 
 
 class RepeatedTimer(object):
     def __init__(self, interval, function, *args, **kwargs):
         self._timer = None
         self.interval = interval
         self.function = function
         self.args = args
         self.kwargs = kwargs
         self.is_running = False
-        print('timer registerd')
+        # print('timer registerd')
         self.start()
 
     def _run(self):
         self.is_running = False
         self.start()
         self.function(*self.args, **self.kwargs)
 
     def start(self):
         if not self.is_running:
             self._timer = threading.Timer(self.interval, self._run)
             self._timer.start()
+            # print("thread ", self._timer.getName())
             self.is_running = True
 
     def stop(self):
         self._timer.cancel()
         self.is_running = False
 
 
@@ -105,14 +106,15 @@
         if self.local_path:
             with open(self.local_path, 'w+'):
                 pass
         self._thread.start()
 
     def cancel(self):
         self.flush()
+        # print("thread stop")
         self._thread.stop()
 
     def flush(self):
         with self.mutex:
             if self._logs_buf:
                 if self.remote:
                     good = append_logs_buf_to_remote(
```

### Comparing `modelwhaleutils-0.5.2.5/mwutils/run.py` & `modelwhaleutils-0.5.2.6/mwutils/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,30 +103,30 @@
         elif env_org_id:
             self.org_id = env_org_id
         else:
             self.org_id = org_id
 
         # self.user_token = user_token
         if config_token:
-            print('using config_token')
+            # print('using config_token')
             self.user_token = config_token
         elif env_token:
-            print('using env_token')
+            # print('using env_token')
             self.user_token = env_token
         else:
             self.user_token = user_token
 
         if remote_path:
             self.remote_path = remote_path
         elif _remote_path:
             self.remote_path = _remote_path + '/api/runs'
         else:
             self.remote_path = 'https://www.heywhale.com/api/runs'
 
-        print('api 地址: ', self.remote_path)
+        # print('api 地址: ', self.remote_path)
         timestr = str(mili_time())
         if not (self.user_id and self.lab_id and self.org_id):
             s = "At least one of required fields is empty:\nuser_id: {}\norg_id: {}\nlab_id: {}\n".format(
                 user_id, org_id, lab_id)
             raise Exception(s)
         self.run_id = name + '_' + timestr
         self.flush_interval_seconds = max(5, flush_interval_seconds)
@@ -165,26 +165,26 @@
                                        buffer_all=self.buffer_all_logs)
         self._loggers['system'] = CustomLogger("system", sample_time_interval_seconds=self.flush_interval_seconds,
                                                metadata=self.metadata, local_path=sys_path, post_addr=self.logs_remote_path,
                                                buffer_all=self.buffer_all_logs)
         self._loggers['meta'] = CustomLogger("meta", sample_time_interval_seconds=self.flush_interval_seconds,
                                              metadata=self.metadata, local_path=sys_path, post_addr=self.logs_remote_path,
                                              buffer_all=self.buffer_all_logs)
-        print('logger class registered')
+        #print('logger class registered')
         # START ML
         self.started = True
         self.__register_signal_handlers()
         for _, logger in self._loggers.items():
             logger.start()
         for _, clogger in self.custom_loggers.items():
             clogger.start()
         self.sys_stat = SystemStats(self)
         self.sys_stat.start()
 
-        print('logger started')
+        # print('logger started')
         # 创建一个 RUN
         _request_meta = {
             'metadata': {
                 'name': name,
                 'user_id': self.user_id,
                 'run_id': self.run_id,
                 'lab_id': self.lab_id,
@@ -206,40 +206,45 @@
                 create_run(_request_meta, _addr)
             else:
                 _request_meta['use_mlflow'] = False
                 _request_meta['is_debug'] = False
                 create_run(_request_meta, self.logs_remote_path)
 
     def init_ml(self):
+        pass
+        # 这个函数在 run.__init__ 已经执行
+        # 实际上这个函数可以不掉用，为了兼容以前的代码
+        # 保持为空
+        # print("pid ", self.pid)
         # if self.pid:
         #     return
-        self.pid = getpid()
-        train_path = path.join(
-            self.local_path, "train.json") if self.write_logs_to_local else ''
-        test_path = path.join(
-            self.local_path, "test.json") if self.write_logs_to_local else ''
-        val_path = path.join(
-            self.local_path, "val.json") if self.write_logs_to_local else ''
-        sys_path = path.join(
-            self.local_path, "sys.json") if self.write_logs_to_local else ''
-        self._loggers['train'] = MLLoger("train", sample_time_interval_seconds=self.flush_interval_seconds,
-                                         metadata=self.metadata, local_path=train_path, post_addr=self.logs_remote_path,
-                                         buffer_all=self.buffer_all_logs)
-        self._loggers['test'] = MLLoger("test", sample_time_interval_seconds=self.flush_interval_seconds,
-                                        metadata=self.metadata, local_path=test_path, post_addr=self.logs_remote_path,
-                                        buffer_all=self.buffer_all_logs)
-        self._loggers['val'] = MLLoger("val", sample_time_interval_seconds=self.flush_interval_seconds,
-                                       metadata=self.metadata, local_path=val_path, post_addr=self.logs_remote_path,
-                                       buffer_all=self.buffer_all_logs)
-        self._loggers['system'] = CustomLogger("system", sample_time_interval_seconds=self.flush_interval_seconds,
-                                               metadata=self.metadata, local_path=sys_path, post_addr=self.logs_remote_path,
-                                               buffer_all=self.buffer_all_logs)
-        self._loggers['meta'] = CustomLogger("meta", sample_time_interval_seconds=self.flush_interval_seconds,
-                                             metadata=self.metadata, local_path=sys_path, post_addr=self.logs_remote_path,
-                                             buffer_all=self.buffer_all_logs)
+        # self.pid = getpid()
+        # train_path = path.join(
+        #     self.local_path, "train.json") if self.write_logs_to_local else ''
+        # test_path = path.join(
+        #     self.local_path, "test.json") if self.write_logs_to_local else ''
+        # val_path = path.join(
+        #     self.local_path, "val.json") if self.write_logs_to_local else ''
+        # sys_path = path.join(
+        #     self.local_path, "sys.json") if self.write_logs_to_local else ''
+        # self._loggers['train'] = MLLoger("train", sample_time_interval_seconds=self.flush_interval_seconds,
+        #                                  metadata=self.metadata, local_path=train_path, post_addr=self.logs_remote_path,
+        #                                  buffer_all=self.buffer_all_logs)
+        # self._loggers['test'] = MLLoger("test", sample_time_interval_seconds=self.flush_interval_seconds,
+        #                                 metadata=self.metadata, local_path=test_path, post_addr=self.logs_remote_path,
+        #                                 buffer_all=self.buffer_all_logs)
+        # self._loggers['val'] = MLLoger("val", sample_time_interval_seconds=self.flush_interval_seconds,
+        #                                metadata=self.metadata, local_path=val_path, post_addr=self.logs_remote_path,
+        #                                buffer_all=self.buffer_all_logs)
+        # self._loggers['system'] = CustomLogger("system", sample_time_interval_seconds=self.flush_interval_seconds,
+        #                                        metadata=self.metadata, local_path=sys_path, post_addr=self.logs_remote_path,
+        #                                        buffer_all=self.buffer_all_logs)
+        # self._loggers['meta'] = CustomLogger("meta", sample_time_interval_seconds=self.flush_interval_seconds,
+        #                                      metadata=self.metadata, local_path=sys_path, post_addr=self.logs_remote_path,
+        #                                      buffer_all=self.buffer_all_logs)
 
     def start_ml(self):
         if self.started:
             return
         self.started = True
         self.__register_signal_handlers()
         for _, logger in self._loggers.items():
@@ -337,42 +342,45 @@
 
     def __sigterm_handler(self, signum, frame):
         self.__abort_run("SIGTERM", "[SIGTERM]Terminated by user")
         traceback.print_stack(f=frame)
         raise KeyboardInterrupt("termniated by user")
 
     def __abort_run(self, sig, reason):
+        if not self.started:
+            return
         if self.remote_path:
             tp = int(time.time())
             json_struct = {"metadata": self.metadata,
                            "timestamp": tp, "signal": sig, "reason": reason}
             for _ in range(3):
                 r = requests.post(self.abort_remote_path, json=json_struct, headers={"Authorization": jwt.encode(
                     {"whatever": "1"}, "857851b2-c28c-4d94-83c8-f607b50ccd03")})
                 if r.status_code >= 400:
                     # something wrong
                     jb = ''
                     try:
                         jb = r.json()
                     except:
                         pass
-                    print("resp:", r)
+                    #print("resp:", r)
                     msg = "code: {}, resp.json: {}, resp.text: {}".format(
                         r.status_code, jb, r.text)
-                    print(msg)
+                    #print(msg)
                     warnings.warn(msg)
                 else:
-                    print("abort remote call succeed. resp:", r)
+                    #print("abort remote call succeed. resp:", r)
                     break
         self.started = False
         self.run_id = "aborted"
 
     def conclude(self, show_memoize=True, save_model=False, model_path="./saved_model", target=None, output_node=None, use_jit=False):
         if not self.started:
             pass
+        self.sys_stat.shutdown()
         for _, logger in self._loggers.items():
             logger.cancel()
             if show_memoize and logger.memoize:
                 print(logger.name, logger.memoize)
         for _, clogger in self.custom_loggers.items():
             clogger.cancel()
             if show_memoize and clogger.memoize:
@@ -485,22 +493,21 @@
                 if r.status_code >= 400:
                     # something wrong
                     jb = ''
                     try:
                         jb = r.json()
                     except:
                         pass
-                    print("resp:", r)
+                    #print("resp:", r)
                     msg = "code: {}, resp.json: {}, resp.text: {}".format(
                         r.status_code, jb, r.text)
-                    print(msg)
+                    #print(msg)
                     warnings.warn(msg)
                 else:
-                    print("conclude remote call succeed. resp:", r)
+                    # print("conclude remote call succeed. resp:", r)
                     break
         # if upload_model:
         #     self.__upload_model()
         if self.use_mlflow:
             mlflow.end_run()
         self.started = False
-        self.run_id = "concluded"
-        print('记录已结束')
+        self.run_id = "concluded"
```

### Comparing `modelwhaleutils-0.5.2.5/mwutils/sys_stat.py` & `modelwhaleutils-0.5.2.6/mwutils/sys_stat.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self.sampler = {}
         self.samples = 0
         self._shutdown = False
         if not psutil:
             print(
                 "psutil not installed, only GPU stats will be reported.  Install with pip install psutil")
         self._thread = threading.Thread(target=self._thread_body)
-        self._thread.daemon = True
+        # self._thread.daemon = True
 
     def start(self):
         self._thread.start()
 
     @property
     def proc(self):
         return psutil.Process(pid=self.run.pid)
```

### Comparing `modelwhaleutils-0.5.2.5/mwutils/tf_utils.py` & `modelwhaleutils-0.5.2.6/mwutils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.2.5/mwutils/torch_utils.py` & `modelwhaleutils-0.5.2.6/mwutils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `modelwhaleutils-0.5.2.5/mwutils/utils.py` & `modelwhaleutils-0.5.2.6/mwutils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 _TIMESTAMP = 'timestamp'
 
 _MAX_ACC = "max_accuracy"
 _MIN_LOSS = "min_loss"
 _BEST = "best"
 
 def create_run(payload, post_addr):
-    print("request address", post_addr)
+    # print("request address", post_addr)
     json_struct = {"metadata": payload['metadata']}
     if payload['is_debug'] == True:
         json_struct['mlflow_run_id'] = payload['mlflow_run']['info']['run_uuid']
     else:
         if payload['use_mlflow'] == True:
             json_struct['mlflow_run_id'] = payload['mlflow_run'].info.run_uuid
         else:
@@ -35,19 +35,19 @@
         if r.status_code >= 400:
             # something wrong
             errorMsg = ''
             try:
                 errorMsg = r.json()
             except:
                 pass
-            print("resp:", r)
-            warnings.warn("code: {}, resp.json: {}, resp.text: {}".format(
-                r.status_code, errorMsg, r.text))
+            # print("resp:", r)
+            # warnings.warn("code: {}, resp.json: {}, resp.text: {}".format(
+            #     r.status_code, errorMsg, r.text))
         else:
-            print("modelwhale run 生成成功")
+            # print("modelwhale run 生成成功")
             return True
     return False
 
 
 class MLLoger(Logger):
     def log(self, step=None, epoch=None, batch=None, loss=None, acc=None, custom_logs=None):
         val = dict()
```

### Comparing `modelwhaleutils-0.5.2.5/setup.py` & `modelwhaleutils-0.5.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="modelwhaleutils",
-    version="0.5.2.5",
+    version="0.5.2.2",
     author="modalwhale team",
     description="use in mw",
     url="https://github.com/Kesci/modelwhaleutils",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

