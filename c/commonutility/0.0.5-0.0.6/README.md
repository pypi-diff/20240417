# Comparing `tmp/commonutility-0.0.5-py3-none-any.whl.zip` & `tmp/commonutility-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3976 bytes, number of entries: 6
--rw-rw-r--  2.0 unx     7082 b- defN 23-Jul-25 19:37 commonutility/__init__.py
--rw-rw-r--  2.0 unx     1073 b- defN 23-Jul-25 19:46 commonutility-0.0.5.dist-info/LICENCE.txt
--rw-rw-r--  2.0 unx      533 b- defN 23-Jul-25 19:46 commonutility-0.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 19:46 commonutility-0.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Jul-25 19:46 commonutility-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      501 b- defN 23-Jul-25 19:46 commonutility-0.0.5.dist-info/RECORD
-6 files, 9295 bytes uncompressed, 3062 bytes compressed:  67.1%
+Zip file size: 4416 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx     8679 b- defN 24-Apr-17 09:21 commonutility/__init__.py
+-rw-rw-r--  2.0 unx     1073 b- defN 24-Apr-17 09:22 commonutility-0.0.6.dist-info/LICENCE.txt
+-rw-rw-r--  2.0 unx      533 b- defN 24-Apr-17 09:22 commonutility-0.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-17 09:22 commonutility-0.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 24-Apr-17 09:22 commonutility-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      501 b- defN 24-Apr-17 09:22 commonutility-0.0.6.dist-info/RECORD
+6 files, 10892 bytes uncompressed, 3502 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: commonutility/__init__.py
 Comment: 
 
-Filename: commonutility-0.0.5.dist-info/LICENCE.txt
+Filename: commonutility-0.0.6.dist-info/LICENCE.txt
 Comment: 
 
-Filename: commonutility-0.0.5.dist-info/METADATA
+Filename: commonutility-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: commonutility-0.0.5.dist-info/WHEEL
+Filename: commonutility-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: commonutility-0.0.5.dist-info/top_level.txt
+Filename: commonutility-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: commonutility-0.0.5.dist-info/RECORD
+Filename: commonutility-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## commonutility/__init__.py

```diff
@@ -172,10 +172,43 @@
             logger.log(f"after line 172 :: {str(modelScopefileJson)}","0")
             file.write(modelScopefileJson)
             file.close()
             logger.log(f"File updated","0")
         
         return "File Updated successfully "
     
+def write_JsonFile(self, fileName, intent_input, read_data_json, invokeIntentModel, finalResult=""):
+    '''
+    This function is used to create a json file and maintain the history count of each input query and its resultant output. 
+    Params  :
+        fileName            : str  --> userId_uuid.json
+        intent_input        : str  --> Stock of item Peanut
+        invokeIntentModel   : str  --> OpenAI / LocalAI
+        read_data_json      : dict --> [{"role": "user", "content": "Stock of item Peanut"}, {"role": "assistant", "content": ""}
+        finalResult         : dict -->  output of the intent query
+    '''
+    directoryPath = invokeIntentModel + "_Instruction"
+    fileName      = directoryPath + "/" + fileName
+    jsonList      = []
+    
+    if len(read_data_json ) != 0:
+        with open(fileName, "w") as file :
+            read_data_json.append({"role" : "user",       "content"  : intent_input })
+            read_data_json.append({"role" : "assistant",  "content"  : finalResult  })
+            json.dump(read_data_json, file)
+            file.close()
+            logger.log(f"File {fileName} overwritten.")
+    else:
+        if not os.path.exists(self.directoryPath):
+            os.mkdir(self.directoryPath)
+        with open(fileName, "w") as file:
+            jsonList.append({"role" : "user",       "content"  : intent_input })
+            jsonList.append({"role" : "assistant",  "content"  : finalResult  })
+            json.dump(jsonList, file)
+            file.close()
+        logger.log(f"File {fileName} created.")
+    
+    
+
```

## Comparing `commonutility-0.0.5.dist-info/LICENCE.txt` & `commonutility-0.0.6.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `commonutility-0.0.5.dist-info/METADATA` & `commonutility-0.0.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonutility
-Version: 0.0.5
+Version: 0.0.6
 Summary: Proteus zipcommon File
 Author: Proteus Technology PVT. LTD.
 Author-email: <apps@baseinformation.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

