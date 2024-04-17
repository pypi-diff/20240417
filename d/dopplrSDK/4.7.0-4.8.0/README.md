# Comparing `tmp/dopplrSDK-4.7.0-py3-none-any.whl.zip` & `tmp/dopplrSDK-4.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7367 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    27524 b- defN 24-Mar-28 13:54 dopplrSDK/__init__.py
--rw-rw-rw-  2.0 fat     1077 b- defN 24-Mar-29 04:31 dopplrSDK-4.7.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2889 b- defN 24-Mar-29 04:31 dopplrSDK-4.7.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-29 04:31 dopplrSDK-4.7.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Mar-29 04:31 dopplrSDK-4.7.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      479 b- defN 24-Mar-29 04:31 dopplrSDK-4.7.0.dist-info/RECORD
-6 files, 32071 bytes uncompressed, 6501 bytes compressed:  79.7%
+Zip file size: 7697 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    33860 b- defN 24-Apr-17 10:51 dopplrSDK/__init__.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 24-Apr-17 11:05 dopplrSDK-4.8.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     3808 b- defN 24-Apr-17 11:05 dopplrSDK-4.8.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-17 11:05 dopplrSDK-4.8.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-17 11:05 dopplrSDK-4.8.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      479 b- defN 24-Apr-17 11:05 dopplrSDK-4.8.0.dist-info/RECORD
+6 files, 39326 bytes uncompressed, 6831 bytes compressed:  82.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: dopplrSDK/__init__.py
 Comment: 
 
-Filename: dopplrSDK-4.7.0.dist-info/LICENSE.txt
+Filename: dopplrSDK-4.8.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dopplrSDK-4.7.0.dist-info/METADATA
+Filename: dopplrSDK-4.8.0.dist-info/METADATA
 Comment: 
 
-Filename: dopplrSDK-4.7.0.dist-info/WHEEL
+Filename: dopplrSDK-4.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: dopplrSDK-4.7.0.dist-info/top_level.txt
+Filename: dopplrSDK-4.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dopplrSDK-4.7.0.dist-info/RECORD
+Filename: dopplrSDK-4.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dopplrSDK/__init__.py

```diff
@@ -137,14 +137,22 @@
             delete="DELETE FROM Dopplr.\"DopplrSchema\" WHERE\"SourceKey\"="+SourceKey
             cur_del.execute(delete)
             cnxn.commit()
             cur_sch=cnxn.cursor()
             for name, dtype in df.dtypes.items():
                 if(dtype == 'datetime64[ns]'):
                     dtype = 'Datetime'
+                elif dtype=='object':
+                    dtype='string'
+                elif dtype=='float64':
+                    dtype='DOUBLE'
+                elif dtype=='int64':
+                    dtype='long'                
+                else:
+                    dtype='long'
                 maxlength = max(df[name].map(str).apply(len))
                 tpp=str(maxlength)
                 tp=str(dtype)
                 insert1="INSERT INTO dopplr.\"DopplrSchema\"(\"SourceKey\",\"Column\" ,\"Type\",\"Length\") VALUES ({},'{}','{}','{}')".format(SourceKey,name,tp,tpp)
                 cur_sch.execute(insert1)
                 cnxn.commit()
 
@@ -183,36 +191,164 @@
         else:
             #print(keys['Cloud'])
             blob_client = client.get_blob_client(container=ContainerName, blob=file_name)
             with open(filePath+'.'+file_type, "rb") as data:
                 blob_client.upload_blob(data)
             
         cnxn.close()
+           
+            
+    except Exception as error:
+        if 'NoneType' in str(error):
+            dopplrsource= 'File does not exists'
+            print("Error : ", dopplrsource)
+            sys.exit()
+        else:
+            print("Error : ",error)
+
+def putFileTomywrkspace_Ingestion(filePath,file_type,loginName,Project_name,Option,de_key):
+    try:
+        keys,db,client=decrypt_keys(de_key)
+        api=db['api']
+        fapi=db['fastapi']
+        Cloud=keys['Cloud']
+        query="select DOR.\"OrgName\",Du.\"UserKey\",P.\"Project_key\" FROM dopplr.\"DopplrUser\" Du join dopplr.\"DopplrOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" \
+join dopplr.\"DopplrProject\" P on P.\"UserKey\"=Du.\"UserKey\" where Du.\"LoginName\"='{0}' and p.\"ProjectName\"='{1}'".format(loginName,Project_name)
+        
+        ContainerName = keys['Bucket']
+
+        cnxn = psycopg2.connect(host=db['host'],database=db['database'],user=db['user'],password=db['password'],port=db['port'])
+    
+        cur=cnxn.cursor()
+        cur.execute(query)
+        results = cur.fetchone()
       
+
+        OrgName=results[0]
+        
+        UserKey=results[1]
+        ProjectKey=results[2]
+        
+        cur=cnxn.cursor()
+      
+        file_name = os.path.basename(filePath)
+        file_name=file_name.lower()
+        query="select count(\"TableName\") from dopplr.\"DopplrLake\" DL join dopplr.\"DopplrUser\" US on DL.\"UserKey\"=US.\"UserKey\" where \"TableName\"="+"'"+file_name+"'"+" and US.\"LoginName\"="+"'"+loginName+"'"
+        cur.execute(query)
+        results = cur.fetchone()
+        if results[0]<1:
+        
+            insert_query = "INSERT INTO dopplr.\"DopplrLake\"(\"UserKey\", \"TableName\",\"ResourceType\",\"DopplrConnectionDetailsKey\",\"Projectid\",\"Status\",\"Schema\",\"Source\",\"CreatedTs\") \
+VALUES ("+str(UserKey)+",'"+file_name+"','"+file_type+"',null,'"+str(ProjectKey)+"','Uploaded','"+loginName+'_schema'+"','MLStudio',CURRENT_TIMESTAMP)"
+            cur.execute(insert_query)
+            cnxn.commit()
+        else:
+            pass
+                    
+        cur1=cnxn.cursor()
+        insert_query1 = "SELECT max(\"SourceKey\") as \"SourceKey\" FROM dopplr.\"DopplrLake\" where \"UserKey\"="+str(UserKey)+" and \"TableName\"='"+file_name+"'"
+        
+        cur1.execute(insert_query1)
+        results = cur1.fetchone()
+        SourceKey=results[0]
+        SourceKey=str(SourceKey)
         if file_type == 'csv' or file_type == 'xlsx':
-            api=f"http://{api}/Workflow/WorkflowDruidSave?SourceID="+(str(SourceKey).lstrip())
-           
-            response=requests.get(api,verify=False)
+            df = pd.read_csv(filePath+'.'+file_type)
             
-            fapi=f"http://{fapi}/Profiling/?sourcekey="+(str(SourceKey).lstrip())
+            cur_del=cnxn.cursor()
+            delete="DELETE FROM Dopplr.\"DopplrSchema\" WHERE\"SourceKey\"="+SourceKey
+            cur_del.execute(delete)
+            cnxn.commit()
+            cur_sch=cnxn.cursor()
+            for name, dtype in df.dtypes.items():
+                if(dtype == 'datetime64[ns]'):
+                    dtype = 'Datetime'
+                elif dtype=='object':
+                    dtype='string'
+                elif dtype=='float64':
+                    dtype='DOUBLE'
+                elif dtype=='int64':
+                    dtype='long'                
+                else:
+                    dtype='long'
+                maxlength = max(df[name].map(str).apply(len))
+                tpp=str(maxlength)
+                tp=str(dtype)
+                insert1="INSERT INTO dopplr.\"DopplrSchema\"(\"SourceKey\",\"Column\" ,\"Type\",\"Length\") VALUES ({},'{}','{}','{}')".format(SourceKey,name,tp,tpp)
+                cur_sch.execute(insert1)
+                cnxn.commit()
+
+        ConnectionString = str(OrgName)+"/"+str(loginName).upper()+"/"+(str(SourceKey).lstrip()+'/Source/'+file_name+'.'+file_type)
+        update_query = "UPDATE dopplr.\"DopplrLake\" set \"ConnectionString\"='"+ConnectionString+"' where \"SourceKey\"="+str(SourceKey)
+        cur2=cnxn.cursor()
+
+        cur2.execute(update_query)
+        cnxn.commit()
+
+
+        
+        if Cloud =='AWS':
             
-            response=requests.get(fapi,verify=False)
+            client.upload_file(filePath+'.'+file_type, ContainerName, ConnectionString)
+            # Generate a pre-signed URL        
+            client.put_object_acl(ACL='public-read',
+                              Bucket=ContainerName,
+                              Key=ConnectionString)
+            url = f"s3://{ContainerName}/{ConnectionString}"
+            print("uri : ",url)
+        elif Cloud == 'MinIO':
+            client.upload_file(filePath+'.'+file_type, ContainerName, ConnectionString)
+            # Generate a pre-signed URL
+            endpoint_url=keys['endpoint_url']
+            presigned_url = client.generate_presigned_url(
+                'get_object',
+                Params={
+                    'Bucket': ContainerName,
+                    'Key': ConnectionString
+                },
+                ExpiresIn=3600  # URL expiration time in seconds (e.g., 1 hour)
+            )
+            url = presigned_url#f"http://{endpoint_url}/{ContainerName}/{ConnectionString}"            
+            print("uri : ",url)
+        else:
+            #print(keys['Cloud'])
+            blob_client = client.get_blob_client(container=ContainerName, blob=file_name)
+            with open(filePath+'.'+file_type, "rb") as data:
+                blob_client.upload_blob(data)
             
-
         
+
+        if Option.upper()=='YES':
+
+              
+            if file_type == 'csv' or file_type == 'xlsx':
+                api=f"http://{api}/Workflow/WorkflowDruidSave?SourceID="+(str(SourceKey).lstrip())
+               
+                response=requests.get(api,verify=False)
+
+                row_count, column_count = df.shape
+                update_query = "UPDATE dopplr.\"DopplrLake\" set \"Status\"='Ready',\"FieldCount\"='"+str(column_count)+"',\"RowCount\"='"+str(row_count)+"' where \"SourceKey\"="+str(SourceKey)
+                cur3=cnxn.cursor()
+
+                cur3.execute(update_query)
+                cnxn.commit()
+            
+                
+            
+        cnxn.close()
             
+        
     except Exception as error:
         if 'NoneType' in str(error):
             dopplrsource= 'File does not exists'
             print("Error : ", dopplrsource)
             sys.exit()
         else:
             print("Error : ",error)
-
-def putFileTomywrkspace_Ingestion(filePath,file_type,loginName,Project_name,Option,de_key):
+def putFileTomywrkspace_Profiling(filePath,file_type,loginName,Project_name,Option,de_key):
     try:
         keys,db,client=decrypt_keys(de_key)
         api=db['api']
         fapi=db['fastapi']
         Cloud=keys['Cloud']
         query="select DOR.\"OrgName\",Du.\"UserKey\",P.\"Project_key\" FROM dopplr.\"DopplrUser\" Du join dopplr.\"DopplrOrg\" DOR on DOR.\"OrgId\"=Du.\"OrgId\" \
 join dopplr.\"DopplrProject\" P on P.\"UserKey\"=Du.\"UserKey\" where Du.\"LoginName\"='{0}' and p.\"ProjectName\"='{1}'".format(loginName,Project_name)
@@ -260,14 +396,22 @@
             delete="DELETE FROM Dopplr.\"DopplrSchema\" WHERE\"SourceKey\"="+SourceKey
             cur_del.execute(delete)
             cnxn.commit()
             cur_sch=cnxn.cursor()
             for name, dtype in df.dtypes.items():
                 if(dtype == 'datetime64[ns]'):
                     dtype = 'Datetime'
+                elif dtype=='object':
+                    dtype='string'
+                elif dtype=='float64':
+                    dtype='DOUBLE'
+                elif dtype=='int64':
+                    dtype='long'                
+                else:
+                    dtype='long'
                 maxlength = max(df[name].map(str).apply(len))
                 tpp=str(maxlength)
                 tp=str(dtype)
                 insert1="INSERT INTO dopplr.\"DopplrSchema\"(\"SourceKey\",\"Column\" ,\"Type\",\"Length\") VALUES ({},'{}','{}','{}')".format(SourceKey,name,tp,tpp)
                 cur_sch.execute(insert1)
                 cnxn.commit()
 
@@ -307,25 +451,27 @@
             #print(keys['Cloud'])
             blob_client = client.get_blob_client(container=ContainerName, blob=file_name)
             with open(filePath+'.'+file_type, "rb") as data:
                 blob_client.upload_blob(data)
             
         cnxn.close()
 
-        if Option=='yes' or Option=='YES':
+        if Option.upper()=='YES':
             print("Ingestion started")
               
             if file_type == 'csv' or file_type == 'xlsx':
                 api=f"http://{api}/Workflow/WorkflowDruidSave?SourceID="+(str(SourceKey).lstrip())
                
                 response=requests.get(api,verify=False)
+                print(response)
                 
-                fapi=f"http://{fapi}/Profiling/?sourcekey="+(str(SourceKey).lstrip())
-                
+                fapi=f"http://{fapi}/Profiling/?sourcekey="+(str(SourceKey).lstrip())           
                 response=requests.get(fapi,verify=False)
+                print(response)
+                
             print("Ingestion Done")
             
 
         
             
     except Exception as error:
         if 'NoneType' in str(error):
@@ -614,9 +760,7 @@
                         blob_data.readinto(my_blob)
                         #print("downloaded")
                         
     except Exception as error:
         print("Error : ",error)
 
 
-
-
```

## Comparing `dopplrSDK-4.7.0.dist-info/LICENSE.txt` & `dopplrSDK-4.8.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dopplrSDK-4.7.0.dist-info/METADATA` & `dopplrSDK-4.8.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dopplrSDK
-Version: 4.7.0
+Version: 4.8.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Anand
 Author-email: anandt@systechusa.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -28,47 +28,62 @@
 Installation Procedure:
 
 	To install the dopplrSDK, please visit https://pypi.org/project/dopplrSDK
 	(OR)
  	pip install dopplrSDK
 
 
-It have 5 functions , those are putFileTomywrkspace, putFolderTomywrkspace, getWorkspaceFile, getWorkspaceFolderFiles and getWorkspaceFile_URL 
+It have 7 functions , those are putFileTomywrkspace, putFolderTomywrkspace, getWorkspaceFile, getWorkspaceFolderFiles and getWorkspaceFile_URL 
 
 1.	The function putFileToMyWorkspace() is designed to return your file to the DataLake. You can use the following syntax:
 
 putFileToMyWorkspace("File Path without file extension", "File Type", "user name","Project_name", "client Key") – [client key common for all users]
 
 For example:
 putFileToMyWorkspace("C:\Downloads\customer", "csv", "Dhoni","demo",  "client key")
 
-2.	The function putFolderTomywrkspace() is designed to return your folder to the DataLake. You can use the following syntax:
+2.	The function putFileTomywrkspace_Ingestion() is designed to return your file to the DataLake and ingest data into druid. You can use the following syntax:
+
+putFileTomywrkspace_Ingestion("File Path without file extension", "File Type", "user name","Project_name","Option" "client Key") – [client key common for all users]
+
+For example:
+putFileTomywrkspace_Ingestion("C:\Downloads\customer", "csv", "Dhoni","demo","yes"  "client key")
+
+3.	The function putFileTomywrkspace_Profiling() is designed to return your file to the DataLake,ingest data into druid and will do pandas profiling. You can use the following syntax:
+
+putFileTomywrkspace_Profiling("File Path without file extension", "File Type", "user name","Project_name","Option" "client Key") – [client key common for all users]
+
+For example:
+putFileTomywrkspace_Profiling("C:\Downloads\customer", "csv", "Dhoni","demo","yes"  "client key")
+
+
+4.	The function putFolderTomywrkspace() is designed to return your folder to the DataLake. You can use the following syntax:
 
 putFolderTomywrkspace("Folder Path ", "Target name", "user name","Project_name", "client Key") – [client key common for all users]
 
 For example:
 putFolderTomywrkspace ("C:\Downloads\folder", " Target name ", "Dhoni","demo",  "client key")
 
 
-3.	The function  getWorkspaceFile() is designed to retrieve  your file from the Data Lake with the following parameters:
+5.	The function  getWorkspaceFile() is designed to retrieve  your file from the Data Lake with the following parameters:
 getWorkspaceFile("File Name", "Download Path", "user name", "client key")
 
 For example:
 getWorkspaceFile("customer.csv", "C:\Downloads\", "Dhoni", "client key")
 
 
 
 
-4.	The function getWorkspaceFolderFiles() is designed to retrieve your files from the folder from the datalake with the following parameters:
+6.	The function getWorkspaceFolderFiles() is designed to retrieve your files from the folder from the datalake with the following parameters:
 
 getWorkspaceFolderFiles("folder","Download Path","user name", "client key")
 
 For example:
 
 getWorkspaceFolderFiles("customer","C:\Downloads\", "Dhoni", "client key")
 
-5.	The function getWorkspaceFile_URL() () is designed to retrieve pre-signed URL of your file from the storage with the following parameters:
+7.	The function getWorkspaceFile_URL() () is designed to retrieve pre-signed URL of your file from the storage with the following parameters:
 getWorkspaceFile_URL(("File Name", "user name", "client key")
 
 NOTE:
 	Please contact admin team for client key
```

