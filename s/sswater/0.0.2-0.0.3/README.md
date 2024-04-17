# Comparing `tmp/sswater-0.0.2.tar.gz` & `tmp/sswater-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sswater-0.0.2.tar", last modified: Wed Apr 17 06:30:05 2024, max compression
+gzip compressed data, was "sswater-0.0.3.tar", last modified: Wed Apr 17 08:04:06 2024, max compression
```

## Comparing `sswater-0.0.2.tar` & `sswater-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 06:30:05.295050 sswater-0.0.2/
--rw-rw-rw-   0        0        0      341 2024-04-17 06:30:05.293050 sswater-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-17 06:30:05.295050 sswater-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      509 2024-04-17 06:30:01.000000 sswater-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:30:05.280036 sswater-0.0.2/sswater/
--rw-rw-rw-   0        0        0     3566 2024-03-18 02:10:44.000000 sswater-0.0.2/sswater/GAILinear.py
--rw-rw-rw-   0        0        0     1437 2024-03-28 00:19:20.000000 sswater-0.0.2/sswater/NLinear.py
--rw-rw-rw-   0        0        0       21 2024-04-17 06:29:56.000000 sswater-0.0.2/sswater/__init__.py
--rw-rw-rw-   0        0        0      490 2024-02-06 07:46:54.000000 sswater-0.0.2/sswater/config.py
--rw-rw-rw-   0        0        0      679 2024-03-18 05:21:00.000000 sswater-0.0.2/sswater/create_seq.py
--rw-rw-rw-   0        0        0     3226 2024-04-17 05:10:05.000000 sswater-0.0.2/sswater/preprocessing.py
--rw-rw-rw-   0        0        0     4074 2024-04-17 00:17:26.000000 sswater-0.0.2/sswater/services.py
--rw-rw-rw-   0        0        0     3858 2024-04-17 06:28:31.000000 sswater-0.0.2/sswater/train.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:30:05.292051 sswater-0.0.2/sswater.egg-info/
--rw-rw-rw-   0        0        0      341 2024-04-17 06:30:05.000000 sswater-0.0.2/sswater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-04-17 06:30:05.000000 sswater-0.0.2/sswater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 06:30:05.000000 sswater-0.0.2/sswater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-15 08:18:40.000000 sswater-0.0.2/sswater.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       32 2024-04-17 06:30:05.000000 sswater-0.0.2/sswater.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 06:30:05.000000 sswater-0.0.2/sswater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 08:04:05.998079 sswater-0.0.3/
+-rw-rw-rw-   0        0        0      341 2024-04-17 08:04:05.997077 sswater-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-17 08:04:05.998079 sswater-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      509 2024-04-17 08:04:02.000000 sswater-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:04:05.985602 sswater-0.0.3/sswater/
+-rw-rw-rw-   0        0        0     3566 2024-03-18 02:10:44.000000 sswater-0.0.3/sswater/GAILinear.py
+-rw-rw-rw-   0        0        0     1437 2024-03-28 00:19:20.000000 sswater-0.0.3/sswater/NLinear.py
+-rw-rw-rw-   0        0        0       21 2024-04-17 08:03:57.000000 sswater-0.0.3/sswater/__init__.py
+-rw-rw-rw-   0        0        0      490 2024-02-06 07:46:54.000000 sswater-0.0.3/sswater/config.py
+-rw-rw-rw-   0        0        0      679 2024-03-18 05:21:00.000000 sswater-0.0.3/sswater/create_seq.py
+-rw-rw-rw-   0        0        0     3437 2024-04-17 07:49:37.000000 sswater-0.0.3/sswater/preprocessing.py
+-rw-rw-rw-   0        0        0     4352 2024-04-17 07:57:47.000000 sswater-0.0.3/sswater/services.py
+-rw-rw-rw-   0        0        0     3858 2024-04-17 07:34:50.000000 sswater-0.0.3/sswater/train.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:04:05.995078 sswater-0.0.3/sswater.egg-info/
+-rw-rw-rw-   0        0        0      341 2024-04-17 08:04:05.000000 sswater-0.0.3/sswater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-04-17 08:04:05.000000 sswater-0.0.3/sswater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 08:04:05.000000 sswater-0.0.3/sswater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-15 08:18:40.000000 sswater-0.0.3/sswater.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       32 2024-04-17 08:04:05.000000 sswater-0.0.3/sswater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 08:04:05.000000 sswater-0.0.3/sswater.egg-info/top_level.txt
```

### Comparing `sswater-0.0.2/sswater/GAILinear.py` & `sswater-0.0.3/sswater/GAILinear.py`

 * *Files identical despite different names*

### Comparing `sswater-0.0.2/sswater/NLinear.py` & `sswater-0.0.3/sswater/NLinear.py`

 * *Files identical despite different names*

### Comparing `sswater-0.0.2/sswater/create_seq.py` & `sswater-0.0.3/sswater/create_seq.py`

 * *Files identical despite different names*

### Comparing `sswater-0.0.2/sswater/preprocessing.py` & `sswater-0.0.3/sswater/preprocessing.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,21 @@
     data_scaled_df['ma_q'] = data_scaled_df['learningma_q'] # ma_Q/의 경우 scaling 하지 않고 target으로 사용해봄. <=== 해당 부분 문제 가능성이 있어 주석처리
     data_scaled_df.drop('learningma_q',axis=1, inplace=True)
 
     features = data_scaled_df.values
     
     return features, scaler2
 
-def correction(data, saved_date):
+def correction(data):
+    # 최종학습날짜 확인
+    directory = "./example/trainedModels/js/"
+    with open(directory+'latest_train_date.txt', 'r' ) as f:
+        lines = f.readlines() 
+        saved_date = lines[0].strip()
+        
     df = pd.DataFrame(data)
 
     cor_df = df[df['data_time'] > str(saved_date)]
     isna = cor_df.isna().sum()
     cols = cor_df.columns
 
     for i in range(len(isna)):
```

### Comparing `sswater-0.0.2/sswater/services.py` & `sswater-0.0.3/sswater/services.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,30 +18,34 @@
 
 import os
 
 device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 class AIModelService :
 
-    def __init__ (self,place,feature_num, saved_date, version=0.1) :        
+    def __init__ (self,place,feature_num) :        
         # 모델 로드를 위한 Config 정의 ==> 데이터 받아오자 
         
         if feature_num < 2:
             directory = "./example/trainedModels/"+place+"/"
         else:
             directory = "./example/trainedModels/"+place+"_cli/"
         
+        with open(directory+'latest_train_date.txt', 'r' ) as f:
+            lines = f.readlines()  # 파일의 모든 줄을 읽어옵니다.
+
+            # 첫 번째 행의 날짜와 두 번째 행의 버전 값을 분리
+            self.saved_date = datetime.strptime(lines[0].strip(), "%Y%m%d%H%M").strftime('%Y-%m-%d %H:%M')
+            self.version = float(lines[1].strip()[1:])
+
         model_list = os.listdir(directory)
         model_list_pt = [file for file in model_list if file.endswith(".pt")]
 
         final_model = directory+model_list_pt[-1]
 
-        self.saved_date = saved_date
-        self.version = version
-
         self.configs = Config(336,4380,feature_num,False)
         if feature_num < 2:
             # 시간 + 유량 모델
             self.model = GAILinear_model(self.configs).cuda()
         else:
             # 추가 데이터 학습 모델
             self.model = NLinear_Model(self.configs).cuda()
@@ -71,28 +75,28 @@
             date_str = str(start_date)  # 시작 날짜 및 시간 문자열
             str_date = datetime.strptime(date_str, "%Y-%m-%d %H:%M:%S")  # 문자열을 datetime 객체로 변환
             end_date = datetime.strptime(str(end_date), "%Y-%m-%d %H:%M:%S")
             totalHour = (end_date - input_date).days * 24 + 24
             
             real_ma_Q = raw_df.loc[raw_df.index >= pd.to_datetime(str_date, format='%Y-%m-%d %H:%M'), 'ma_q'].tolist()
             total_list = real_ma_Q.copy()
-            print(real_ma_Q)
+            
         else :
             if(end_date != "2300"):
                 end_date = datetime.strptime(str(end_date), "%Y-%m-%d %H:%M:%S")
                 totalHour = (end_date - input_date).days * 24 + 24
 
             total_list = []
 
 
         prediction_list = prediction[0].tolist()
 
         max_value = raw_df['ma_q'].max()
         min_value = raw_df['ma_q'].min()
-            # 예측값 최대 최소
+        # 예측값 최대 최소
         max_pred = max(prediction_list)
         min_pred = min(prediction_list)
         mean_pred = sum(prediction_list)/len(prediction_list)
 
         if totalHour > 0:
             for i in range(totalHour):
                 total_list.append(prediction_list[i])
```

### Comparing `sswater-0.0.2/sswater/train.py` & `sswater-0.0.3/sswater/train.py`

 * *Files identical despite different names*

