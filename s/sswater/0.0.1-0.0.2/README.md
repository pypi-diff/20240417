# Comparing `tmp/sswater-0.0.1.tar.gz` & `tmp/sswater-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sswater-0.0.1.tar", last modified: Mon Apr 15 08:18:39 2024, max compression
+gzip compressed data, was "sswater-0.0.2.tar", last modified: Wed Apr 17 06:30:05 2024, max compression
```

## Comparing `sswater-0.0.1.tar` & `sswater-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 08:18:39.590467 sswater-0.0.1/
--rw-rw-rw-   0        0        0      285 2024-04-15 08:18:39.588099 sswater-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-15 08:18:39.590467 sswater-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      549 2024-04-15 08:17:40.000000 sswater-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:18:39.577142 sswater-0.0.1/sswater/
--rw-rw-rw-   0        0        0     3566 2024-03-18 02:10:44.000000 sswater-0.0.1/sswater/GAILinear.py
--rw-rw-rw-   0        0        0     1437 2024-03-28 00:19:20.000000 sswater-0.0.1/sswater/NLinear.py
--rw-rw-rw-   0        0        0       21 2024-04-15 08:18:06.000000 sswater-0.0.1/sswater/__init__.py
--rw-rw-rw-   0        0        0     1117 2024-03-29 05:14:58.000000 sswater-0.0.1/sswater/calData.py
--rw-rw-rw-   0        0        0      490 2024-02-06 07:46:54.000000 sswater-0.0.1/sswater/config.py
--rw-rw-rw-   0        0        0      679 2024-03-18 05:21:00.000000 sswater-0.0.1/sswater/create_seq.py
--rw-rw-rw-   0        0        0     1375 2024-04-09 03:47:10.000000 sswater-0.0.1/sswater/getDatas.py
--rw-rw-rw-   0        0        0     1881 2024-04-11 09:24:14.000000 sswater-0.0.1/sswater/preprocessing.py
--rw-rw-rw-   0        0        0     4519 2024-04-11 09:38:20.000000 sswater-0.0.1/sswater/services.py
--rw-rw-rw-   0        0        0     4142 2024-04-08 04:44:26.000000 sswater-0.0.1/sswater/train.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:18:39.586620 sswater-0.0.1/sswater.egg-info/
--rw-rw-rw-   0        0        0      285 2024-04-15 08:18:39.000000 sswater-0.0.1/sswater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-04-15 08:18:39.000000 sswater-0.0.1/sswater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 08:18:39.000000 sswater-0.0.1/sswater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-15 08:18:39.000000 sswater-0.0.1/sswater.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       32 2024-04-15 08:18:39.000000 sswater-0.0.1/sswater.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-15 08:18:39.000000 sswater-0.0.1/sswater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 06:30:05.295050 sswater-0.0.2/
+-rw-rw-rw-   0        0        0      341 2024-04-17 06:30:05.293050 sswater-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-17 06:30:05.295050 sswater-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      509 2024-04-17 06:30:01.000000 sswater-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:30:05.280036 sswater-0.0.2/sswater/
+-rw-rw-rw-   0        0        0     3566 2024-03-18 02:10:44.000000 sswater-0.0.2/sswater/GAILinear.py
+-rw-rw-rw-   0        0        0     1437 2024-03-28 00:19:20.000000 sswater-0.0.2/sswater/NLinear.py
+-rw-rw-rw-   0        0        0       21 2024-04-17 06:29:56.000000 sswater-0.0.2/sswater/__init__.py
+-rw-rw-rw-   0        0        0      490 2024-02-06 07:46:54.000000 sswater-0.0.2/sswater/config.py
+-rw-rw-rw-   0        0        0      679 2024-03-18 05:21:00.000000 sswater-0.0.2/sswater/create_seq.py
+-rw-rw-rw-   0        0        0     3226 2024-04-17 05:10:05.000000 sswater-0.0.2/sswater/preprocessing.py
+-rw-rw-rw-   0        0        0     4074 2024-04-17 00:17:26.000000 sswater-0.0.2/sswater/services.py
+-rw-rw-rw-   0        0        0     3858 2024-04-17 06:28:31.000000 sswater-0.0.2/sswater/train.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:30:05.292051 sswater-0.0.2/sswater.egg-info/
+-rw-rw-rw-   0        0        0      341 2024-04-17 06:30:05.000000 sswater-0.0.2/sswater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-04-17 06:30:05.000000 sswater-0.0.2/sswater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 06:30:05.000000 sswater-0.0.2/sswater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-15 08:18:40.000000 sswater-0.0.2/sswater.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       32 2024-04-17 06:30:05.000000 sswater-0.0.2/sswater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 06:30:05.000000 sswater-0.0.2/sswater.egg-info/top_level.txt
```

### Comparing `sswater-0.0.1/sswater/GAILinear.py` & `sswater-0.0.2/sswater/GAILinear.py`

 * *Files identical despite different names*

### Comparing `sswater-0.0.1/sswater/NLinear.py` & `sswater-0.0.2/sswater/NLinear.py`

 * *Files identical despite different names*

### Comparing `sswater-0.0.1/sswater/create_seq.py` & `sswater-0.0.2/sswater/create_seq.py`

 * *Files identical despite different names*

### Comparing `sswater-0.0.1/sswater/services.py` & `sswater-0.0.2/sswater/services.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from .NLinear import NLinear_Model
 from .GAILinear import GAILinear_model
 
 from .config import Config
 from .create_seq import create_seq
 from .train import model_train
 from .preprocessing import preprocess
-from .calData import day_case
 
 import torch
 import torch.nn.functional as F
 import torch.optim as optim
 
 import numpy as np
 import pandas as pd
@@ -19,34 +18,29 @@
 
 import os
 
 device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 class AIModelService :
 
-    def __init__ (self,place,feature_num) :        
+    def __init__ (self,place,feature_num, saved_date, version=0.1) :        
         # 모델 로드를 위한 Config 정의 ==> 데이터 받아오자 
         
-        current_dir = os.path.dirname(os.path.realpath(__file__))
         if feature_num < 2:
-            directory = current_dir+"/trainedModels/"+place+"/"
+            directory = "./example/trainedModels/"+place+"/"
         else:
-            directory = current_dir+"/trainedModels/"+place+"_cli/"
+            directory = "./example/trainedModels/"+place+"_cli/"
         
         model_list = os.listdir(directory)
         model_list_pt = [file for file in model_list if file.endswith(".pt")]
 
         final_model = directory+model_list_pt[-1]
 
-        with open(directory+'latest_train_date.txt', 'r' ) as f:
-            lines = f.readlines()  # 파일의 모든 줄을 읽어옵니다.
-
-            # 첫 번째 행의 날짜와 두 번째 행의 버전 값을 분리
-            self.saved_date = datetime.strptime(lines[0].strip(), "%Y%m%d%H%M").strftime('%Y-%m-%d %H:%M')
-            self.version = float(lines[1].strip()[1:])
+        self.saved_date = saved_date
+        self.version = version
 
         self.configs = Config(336,4380,feature_num,False)
         if feature_num < 2:
             # 시간 + 유량 모델
             self.model = GAILinear_model(self.configs).cuda()
         else:
             # 추가 데이터 학습 모델
@@ -74,15 +68,15 @@
         input_date = pd.Timestamp(datetime.strptime(str(input_date), "%Y-%m-%d %H:%M:%S"))
 
         if start_date != 0:
             date_str = str(start_date)  # 시작 날짜 및 시간 문자열
             str_date = datetime.strptime(date_str, "%Y-%m-%d %H:%M:%S")  # 문자열을 datetime 객체로 변환
             end_date = datetime.strptime(str(end_date), "%Y-%m-%d %H:%M:%S")
             totalHour = (end_date - input_date).days * 24 + 24
-            #print(totalHour)
+            
             real_ma_Q = raw_df.loc[raw_df.index >= pd.to_datetime(str_date, format='%Y-%m-%d %H:%M'), 'ma_q'].tolist()
             total_list = real_ma_Q.copy()
             print(real_ma_Q)
         else :
             if(end_date != "2300"):
                 end_date = datetime.strptime(str(end_date), "%Y-%m-%d %H:%M:%S")
                 totalHour = (end_date - input_date).days * 24 + 24
@@ -106,10 +100,9 @@
             for i in range(len(prediction_list)):
                 total_list.append(prediction_list[i])
 
         #is_real = [1] * len(real_ma_Q) + [0] * len(prediction_list)
         generated_dates = [input_date + timedelta(hours=i) for i in range(0, len(total_list))]
         
         df = pd.DataFrame({"x": generated_dates, "y": total_list, "last_tr_day": self.saved_date, "last_ver": self.version })
-        print(df.tail())
 
         return df
```

### Comparing `sswater-0.0.1/sswater/train.py` & `sswater-0.0.2/sswater/train.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,46 +9,43 @@
 import torch.nn.functional as F
 import torch.optim as optim
 from datetime import datetime, timedelta
 
 device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 # 학습데이터, 장소, config, 학습특성개수, 추가학습여부
-def model_train(data, place, configs, feature_num, latest_date, tuning=False):
+def model_train(data, place, configs, feature_num, latest_date):
     version = 0 # 첫버전은 0
-    current_dir = os.path.dirname(os.path.realpath(__file__))
     filtered_data = data
 
     if feature_num < 2:
         # 시간 + 유량 모델
-        directory = current_dir+"/trainedModels/"+place+"/"
+        directory = "./example/trainedModels/"+place+"/"
         loaded_model = GAILinear_model(configs).cuda()
         file_name = place
     else:
         # 추가 데이터 학습 모델
-        directory = current_dir+"/trainedModels/"+place+"_cli/"
+        directory = "./example/trainedModels/"+place+"_cli/"
         loaded_model = NLinear_Model(configs).cuda()
         file_name = place+"_cli"
 
-    if tuning:
-        print("Fine Tuning")
         # 모델 로드
-        model_list = os.listdir(directory)
-        model_list_pt = [file for file in model_list if file.endswith(".pt")]
-        final_model = directory+model_list_pt[-1]
-        loaded_model.load_state_dict(torch.load(final_model))
+    model_list = os.listdir(directory)
+    model_list_pt = [file for file in model_list if file.endswith(".pt")]
+    final_model = directory+model_list_pt[-1]
+    loaded_model.load_state_dict(torch.load(final_model))
         
-        with open(directory+'latest_train_date.txt', 'r' ) as f:
-            lines = f.readlines()  # 파일의 모든 줄을 읽어옵니다.
+    with open(directory+'latest_train_date.txt', 'r' ) as f:
+        lines = f.readlines()  # 파일의 모든 줄을 읽어옵니다.
 
-            # 첫 번째 행의 날짜와 두 번째 행의 버전 값을 분리
-            saved_date = lines[0].strip()
-            version = float(lines[1].strip()[1:])
+        # 첫 번째 행의 날짜와 두 번째 행의 버전 값을 분리
+        saved_date = lines[0].strip()
+        version = float(lines[1].strip()[1:])
         
-            date_obj = datetime.strptime(lines[0].strip(), "%Y%m%d%H%M").strftime('%Y-%m-%d %H:%M')
+        date_obj = datetime.strptime(lines[0].strip(), "%Y%m%d%H%M").strftime('%Y-%m-%d %H:%M')
 
     X,y =  create_seq(filtered_data, configs.seq_len, configs.pred_len)
     
     # 학습을 위한 설정
     n_epochs = 300
     batch_size = 100
     split_ratio = 0.9
@@ -93,21 +90,18 @@
         print("Error: Failed to create the directory.")
 
     if version > 0:
         version += 0.1
     else:
         version = 0.1
 
-    if tuning:
-        file_name = file_name+"_updated_model_"+str(version).replace(".","")+".pt"
-    else:
-        file_name = file_name+"_model_"+str(version).replace(".","")+".pt"
+    file_name = file_name+"_updated_model_"+str(version).replace(".","")+".pt"
 
     if feature_num < 2:
-        torch.save(loaded_model.state_dict(), "./example/src/trainedModels/"+place+"/"+file_name)
+        torch.save(loaded_model.state_dict(), "./example/trainedModels/"+place+"/"+file_name)
     else:
-        torch.save(loaded_model.state_dict(), "./example/src/trainedModels/"+place+"_cli/"+file_name)
+        torch.save(loaded_model.state_dict(), "./example/trainedModels/"+place+"_cli/"+file_name)
     # 업데이트된 날짜와 버전 값을 파일에 기록합니다.
     with open(directory+'latest_train_date.txt', 'w' ) as f:
         f.write(str(latest_date) + '\n') 
         f.write(f'v{version:.1f}')
```

