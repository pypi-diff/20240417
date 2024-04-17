# Comparing `tmp/BIDSit-0.0.9.tar.gz` & `tmp/bidsit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BIDSit-0.0.9.tar", last modified: Mon Jul 31 22:58:38 2023, max compression
+gzip compressed data, was "bidsit-0.1.0.tar", last modified: Wed Apr 17 18:46:12 2024, max compression
```

## Comparing `BIDSit-0.0.9.tar` & `bidsit-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:58:38.179807 BIDSit-0.0.9/
--rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-07-31 22:58:38.179470 BIDSit-0.0.9/PKG-INFO
--rw-r--r--   0 labmanager   (501) staff       (20)      762 2023-04-19 23:00:43.000000 BIDSit-0.0.9/README.rst
--rw-r--r--   0 labmanager   (501) staff       (20)       38 2023-07-31 22:58:38.179923 BIDSit-0.0.9/setup.cfg
--rw-r--r--   0 labmanager   (501) staff       (20)     2068 2023-07-31 20:54:57.000000 BIDSit-0.0.9/setup.py
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:58:38.173698 BIDSit-0.0.9/src/
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:58:38.176659 BIDSit-0.0.9/src/BIDSit/
--rw-r--r--   0 labmanager   (501) staff       (20)     5330 2023-06-28 22:32:23.000000 BIDSit-0.0.9/src/BIDSit/Test_script.py
--rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-03-23 19:34:37.000000 BIDSit-0.0.9/src/BIDSit/__init__.py
--rw-r--r--   0 labmanager   (501) staff       (20)       87 2023-07-31 22:57:25.000000 BIDSit-0.0.9/src/BIDSit/__main__.py
--rw-r--r--   0 labmanager   (501) staff       (20)    24979 2023-04-26 21:48:18.000000 BIDSit-0.0.9/src/BIDSit/dicom_to_bids2.py
--rw-r--r--   0 labmanager   (501) staff       (20)    68398 2023-07-31 22:57:05.000000 BIDSit-0.0.9/src/BIDSit/go.py
--rw-r--r--   0 labmanager   (501) staff       (20)      576 2023-07-31 22:57:44.000000 BIDSit-0.0.9/src/BIDSit/version.py
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:58:38.178948 BIDSit-0.0.9/src/BIDSit.egg-info/
--rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-07-31 22:58:38.000000 BIDSit-0.0.9/src/BIDSit.egg-info/PKG-INFO
--rw-r--r--   0 labmanager   (501) staff       (20)      328 2023-07-31 22:58:38.000000 BIDSit-0.0.9/src/BIDSit.egg-info/SOURCES.txt
--rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-07-31 22:58:38.000000 BIDSit-0.0.9/src/BIDSit.egg-info/dependency_links.txt
--rw-r--r--   0 labmanager   (501) staff       (20)       54 2023-07-31 22:58:38.000000 BIDSit-0.0.9/src/BIDSit.egg-info/requires.txt
--rw-r--r--   0 labmanager   (501) staff       (20)        7 2023-07-31 22:58:38.000000 BIDSit-0.0.9/src/BIDSit.egg-info/top_level.txt
+drwxr-xr-x   0 labmanager   (502) staff       (20)        0 2024-04-17 18:46:12.794561 bidsit-0.1.0/
+-rw-r--r--   0 labmanager   (502) staff       (20)     1162 2024-04-17 18:46:12.794158 bidsit-0.1.0/PKG-INFO
+-rw-rw-r--   0 labmanager   (502) staff       (20)      762 2023-08-08 21:00:19.000000 bidsit-0.1.0/README.rst
+-rw-r--r--   0 labmanager   (502) staff       (20)      582 2024-04-17 18:22:52.000000 bidsit-0.1.0/pyproject.toml
+-rw-r--r--   0 labmanager   (502) staff       (20)       38 2024-04-17 18:46:12.794648 bidsit-0.1.0/setup.cfg
+-rw-rw-r--   0 labmanager   (502) staff       (20)     2169 2024-02-28 00:38:56.000000 bidsit-0.1.0/setup.py
+drwxr-xr-x   0 labmanager   (502) staff       (20)        0 2024-04-17 18:46:12.785517 bidsit-0.1.0/src/
+drwxr-xr-x   0 labmanager   (502) staff       (20)        0 2024-04-17 18:46:12.790979 bidsit-0.1.0/src/BIDSit/
+-rw-rw-r--   0 labmanager   (502) staff       (20)        1 2023-08-08 21:00:19.000000 bidsit-0.1.0/src/BIDSit/__init__.py
+-rw-rw-r--   0 labmanager   (502) staff       (20)       58 2023-08-08 21:00:19.000000 bidsit-0.1.0/src/BIDSit/__main__.py
+-rw-rw-r--   0 labmanager   (502) staff       (20)    24979 2023-08-08 21:00:19.000000 bidsit-0.1.0/src/BIDSit/dicom_to_bids2.py
+-rw-r--r--   0 labmanager   (502) staff       (20)    70485 2024-04-17 18:44:11.000000 bidsit-0.1.0/src/BIDSit/go.py
+-rw-rw-r--   0 labmanager   (502) staff       (20)    68637 2023-08-08 21:00:19.000000 bidsit-0.1.0/src/BIDSit/go_old.py
+-rw-rw-r--   0 labmanager   (502) staff       (20)      576 2024-04-17 18:43:58.000000 bidsit-0.1.0/src/BIDSit/version.py
+drwxr-xr-x   0 labmanager   (502) staff       (20)        0 2024-04-17 18:46:12.793483 bidsit-0.1.0/src/BIDSit.egg-info/
+-rw-r--r--   0 labmanager   (502) staff       (20)     1162 2024-04-17 18:46:12.000000 bidsit-0.1.0/src/BIDSit.egg-info/PKG-INFO
+-rw-r--r--   0 labmanager   (502) staff       (20)      375 2024-04-17 18:46:12.000000 bidsit-0.1.0/src/BIDSit.egg-info/SOURCES.txt
+-rw-r--r--   0 labmanager   (502) staff       (20)        1 2024-04-17 18:46:12.000000 bidsit-0.1.0/src/BIDSit.egg-info/dependency_links.txt
+-rw-r--r--   0 labmanager   (502) staff       (20)       42 2024-04-17 18:46:12.000000 bidsit-0.1.0/src/BIDSit.egg-info/entry_points.txt
+-rw-r--r--   0 labmanager   (502) staff       (20)       53 2024-04-17 18:46:12.000000 bidsit-0.1.0/src/BIDSit.egg-info/requires.txt
+-rw-r--r--   0 labmanager   (502) staff       (20)        7 2024-04-17 18:46:12.000000 bidsit-0.1.0/src/BIDSit.egg-info/top_level.txt
```

### Comparing `BIDSit-0.0.9/PKG-INFO` & `bidsit-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: BIDSit
-Version: 0.0.9
+Version: 0.1.0
 Summary: A BIDS conversion tool for fMRI data
 Home-page: https://github.com/jenburrell/BIDSit
 Author: Jen Burrell
-Author-email: jenbur@psych.ubc.ca
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
+Author-email: Jen Burrell <jenbur@psych.ubc.ca>
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+Requires-Dist: PySimpleGUI<=5.0.0
+Requires-Dist: natsort>=8.3.1
 Provides-Extra: dev
+Requires-Dist: pytest>=3.7; extra == "dev"
 
 BIDSit
 ===========
 
 The ``BIDSit`` project is a toolbox to organize MRI data into BIDS format written in Python.
 
 Installation
```

### Comparing `BIDSit-0.0.9/README.rst` & `bidsit-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.9/setup.py` & `bidsit-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,29 +36,34 @@
     version=version,
     description='A BIDS conversion tool for fMRI data',
     long_description=readme,
     long_description_content_type='text/x-rst',
     url='https://github.com/jenburrell/BIDSit',
     author='Jen Burrell',
     author_email='jenbur@psych.ubc.ca',
-    python_requires='>=3.10',
+    python_requires='>=3.9',
     
     package_dir={"":"src"},
     packages=find_namespace_packages(where='src'),
     
     classifiers=[
     'Programming Language :: Python :: 3.10',
     'Operating System :: OS Independent',
     'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     
     install_requires=[
-        'PySimpleGUI>=4.60.4',
+        'PySimpleGUI<=5.0.0',
         'natsort>=8.3.1',
     ],
     extras_require={
         "dev": [
             "pytest>=3.7",
         ],
     },
+    entry_points={
+        'console_scripts': [
+            'BIDSit = BIDSit.go:DOit',
+        ]
+    }
 )
```

### Comparing `BIDSit-0.0.9/src/BIDSit/dicom_to_bids2.py` & `bidsit-0.1.0/src/BIDSit/dicom_to_bids2.py`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.9/src/BIDSit/go.py` & `bidsit-0.1.0/src/BIDSit/go.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #========================================================================#
 # Script Name: BIDSit.py                                                 #
 #                                                                        #
+# Version: 0.1.0                                                         #
+#                                                                        #
 # Description: This script converts user inputted data based on BIDS     #
 #              specifications                                            #
 #                                                                        #
-# Authors:     Jen Burrell & Justin Andrushko  (March 28th, 2023)        #
+# Authors:     Jen Burrell & Justin Andrushko  (April 17th, 2023)        #
 #========================================================================#
 #------------------------------------------------#
 #        Import script dependency packages       #
 #------------------------------------------------#
 import subprocess
 import os
 import sys
@@ -29,29 +31,33 @@
     # - get user input - #
     sg.theme('GreenTan')
     user_info = start_gui()
     
     # - define variables in use - #
     in_dir = user_info['in_dir'] # in_dir is where the input files are
     out_dir = user_info['out_dir'] # out_dir is where the output files will go
+    if 'rawdata' in out_dir:
+        out_dir = out_dir.rsplit('/rawdata')[0]
+        user_info['out_dir'] = out_dir
     WDIR = in_dir # WDIR is wherever we are working at the time
     user_info['WDIR'] = WDIR
     
     ### --- convert files to NIFTIs --- ###
     if user_info['dcm2niix']:
         WDIR = out_dir
-        sub_folders = glob.glob(f"{in_dir}/*/")
+        sub_folders = glob.glob(f"{in_dir}/*")
         ses_folders = []
         for sub in sub_folders:
             if user_info['ses'] == "Yes":
-                ses_folders = ses_folders + list(glob.glob(f"{sub}/*/"))
-                ses = 'ses=True'
+                ses_folders = ses_folders + list(glob.glob(f"{sub}/*"))
+                ses = True
             else:
                 ses_folders = sub_folders
-                ses = 'ses=False'
+                ses = False
+            
         # - multiprocessing - #
         pool = Pool() # Create a multiprocessing Pool
         pool.starmap(dcm2niix, zip(ses_folders, repeat(WDIR), repeat(ses))) # process gets masks
         # - Close the pool, keep the kids safe - #
         pool.close()
         pool.join()
         # - set WDIR to where the new files are - #
@@ -72,29 +78,31 @@
             copy_it(WDIR, out_dir + "/sourcedata")
     
     ### --- BIDSit --- ###
     if user_info['bids_it']:
         bids_info = BIDSit_gui(user_info) # get BIDS information from GUI
         user_info = {**user_info, **bids_info}
         sub_list = listdir(WDIR)
+        nonsubs = []
         for entry in sub_list:
             if user_info['ses'] =='Yes':
                 for file in listdir(os.path.join(WDIR,entry)):
                     if os.path.isdir(os.path.join(WDIR,entry,file)):
                         if entry in sub_list:
                             sub_list = [entry.replace(entry,os.path.join(entry,file))]
                         else:
                             sub_list.append(os.path.join(entry,file))
             else:
                 if os.path.isdir(os.path.join(WDIR,entry)):
                     continue
                 else:
-                    sub_list.remove(entry)
+                    nonsubs.append(entry)
         for sub in natsorted(sub_list):
-            BIDSit(sub, user_info)
+            if not sub in nonsubs:
+                BIDSit(sub, user_info)
         # - multiprocessing - #
         ### not working with glob, wont find files ###
 #        pool = Pool(len(sub_list)) # Create a multiprocessing Pool
 #        pool.starmap(BIDSit, zip(sub_list, repeat(user_info))) # BIDSit for each participant or time point
 #        # - Close the pool, keep the kids safe - #
 #        pool.close()
 #        pool.join()
@@ -108,15 +116,19 @@
                 shutil.rmtree(WDIR+'/'+fld)
                 
         # - make derivatives folder - #
         der_dir = f"{WDIR}/derivatives"
         def ignore_files(dir, files):
             return [f for f in files if os.path.isfile(os.path.join(dir, f))]
         if dir_exists(der_dir):
-            dir = listdir(WDIR+'/rawdata')
+            dir_all = listdir(WDIR+'/rawdata')
+            dir=[]
+            for thing in dir_all:
+                if os.path.isdir(os.path.join(WDIR+'/rawdata/',thing)):
+                     dir.append(thing)
             der_fld = listdir(der_dir)
             for sub in dir:
                 if sub in der_fld:
                     continue
                 else:
                     shutil.copytree(WDIR+'/rawdata/'+sub, der_dir+'/'+sub, ignore=ignore_files)
         else:
@@ -141,30 +153,35 @@
         else:
             print("dataset_description.json already exists in the directory.")
 
         # - README file - #
         if not os.path.exists(WDIR + '/rawdata' + '/README.md'):
             # Create a new README file in BIDS format
             with open(WDIR + '/rawdata' + '/README.md', 'w') as f:
-                f.write('# ' + os.path.basename(WDIR) + 'My Project\n\nThis is a project in BIDS format.\n\n## Introduction\n\n## Data\n\n## Code\n\n## Results\n\n## Conclusion\n\n## References\n\n')
+                f.write('# ' + os.path.basename(WDIR) + f"\t{user_info['exp_name']}\n\nThis is a project in BIDS format.\n\n## Introduction\n\n## Data\n\n## Code\n\n## Results\n\n## Conclusion\n\n## References\n\n")
                 print('README.md file created successfully!')
         else:
             print('README.md file already exists.')
 
         # - participants.tsv file - #
-        if not os.path.exists(WDIR + '/rawdata' + '/participants.tsv'):
+        if not os.path.exists(WDIR + '/rawdata/participants.tsv'):
             # Create a new participants.tsv file in BIDS format
-            with open(WDIR + '/rawdata' + '/participants.tsv', 'w') as f:
+            with open(WDIR + '/rawdata/participants.tsv', 'w') as f:
                 f.write('participant_id\tage\tsex\n')
                 for sub in natsorted(sub_list):
                     sub = sub.split('/')[0]
-                    f.write(f"{sub}\t \t \n")
+                    f.write(f"\n{sub}\t \t")
                 print('participants.tsv file created successfully!')
-        else:
-            print('participants.tsv file already exists.')
+        elif os.path.exists(WDIR + '/rawdata/participants.tsv'):
+            # Add new participants to file in BIDS format
+            with open(WDIR + '/rawdata/participants.tsv', 'a+') as f:
+                for sub in natsorted(sub_list):
+                    sub = sub.split('/')[0]
+                    f.write(f"\n{sub}\t \t")
+                print('participants.tsv file editted successfully!')
 
         # - participants.json file - #
         if not os.path.exists(WDIR + '/rawdata' + '/participants.json'):
             # Create a new participants.json file in BIDS format
             data={}
             for sub in natsorted(sub_list):
                 data = {
@@ -180,20 +197,21 @@
                         }
                     }}
             with open(WDIR + '/rawdata' + '/participants.json', 'w') as f:
                 json.dump(data, f, indent=4)
                 print('participants.json file created successfully!')
         else:
             print('participants.json file already exists.')
-    else: # when not doing BIDSit, rename tempdata to sourcedata and delete tempdata
+        print('\nYour data should be BIDS-ified :)')
+    else: # when not doing BIDSit, rename tempdata to sourcedata
         WDIR = WDIR.rsplit('/',1)[0]
         dir = listdir(WDIR)
         for fld in dir:
             if 'tempdata' in fld:
-                shutil.rmtree(WDIR+'/'+fld)
+                os.rename(WDIR+'/'+fld, WDIR+'/sourcedata')
     return
     
 #------------------#
 #       GUIs       #
 #------------------#
 # - gui functions - #
 def text_element(text):
@@ -269,16 +287,15 @@
                 info['out_dir'] = values['-WDIR-'].split()[0]
                 mkdir(info['out_dir'])
             else:
                 info['out_dir'] = info['in_dir'].split()[0].rsplit('/', 1)[0]
                 mkdir(info['out_dir'])
             info['dcm2niix'] = values['-dcm2niix-']
             info['bids_it'] = values['-bids_it-']
-            if info['bids_it']:
-                info['copy'] = sg.popup_yes_no(f"Do you want to copy your NIFTI files to a 'sourcedata' folder in {info['out_dir']}")
+            info['copy'] = sg.popup_yes_no(f"Do you want to copy your NIFTI files to a 'sourcedata' folder in {info['out_dir']}")
             info['func'] = values['-func-']
             info['anat'] = values['-anat-']
             info['dwi'] = values['-dwi-']
             info['fmap'] = values['-fmap-']
             info['perf'] = values['-perf-']
             if values['-ses-'] == '...':
                 sg.popup_no_border("Please indicate if your data has mutliple sessions per participant.")
@@ -479,15 +496,15 @@
             break
         elif event == 'Go':
             info = values
             flag = False
             if echo == 'Yes':
                 for num in range(1, int(task_num)+1):
                     if not values[f"input_Task-{num}-echo"] or int(values[f"input_Task-{num}-echo"]) < 1:
-                        values[f"input_Task-{num}-echo"] = sg.popup_get_text(f"Number of echos for Task {num} must be >= 1 n\Please enter number of echos for Task {num}", title="Oops")
+                        values[f"input_Task-{num}-echo"] = sg.popup_get_text(f"Number of echos for Task {num} must be >= 1 \nPlease enter number of echos for Task {num}", title="Oops")
             info = values
             window_2.close()
     return info
     window_2.close()
     
 # - gui to specify anat data parameters - #
 def anat_butt(task_num, scan_num):
@@ -731,30 +748,32 @@
         num = re.findall(r'\d+',sub)
         if not any(num):
             sub = 'sub-'+ sub
         else:
             sub = 'sub-'+''.join(num)
         sub_solo = sub # subject variable that only has sub information
         f_sub = sub # file naming subject variable
-            
+
     task_num = int(user_info[f"{file_type}_task_num"])
     scan_num = int(user_info[f"{file_type}_scan_num"])
     
     
     if echo and isinstance(echo[0], int): # check to see if it is an intended for file or an echo file or both
+        ME = True # flag for Multi echo data
         echo_num = echo[0]
         if len(echo) > 1:
             types = echo[1]
         else:
             types = {}
     elif echo and isinstance(echo, tuple):
         types = echo[0]
         echo_num = 1
         echo = {}
     else:
+        ME = False
         types = echo
         echo_num = 1
         echo = {}
         
     files =[]
     file = ''
     if types:
@@ -772,25 +791,35 @@
         for file in files:
             if "_ph." in file: # might cause an issue for phase map files. If they are signaled by dxm2nii with ph. as end of file name
                 continue
             if f"input_Task-{task_ord[i]+1}-echo" in user_info[file_type].keys() and int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"]) >1:
                 file_list.append('_'.join(file.rsplit('_',2)[-2:]).split('.')[0])
             else:
                 file_list.append(file.rsplit('_',1)[-1].split('.')[0])
-                
-        file_list = natsorted(file_list)
+        
+        file_list = natsorted(file_list) # sort acq numbers in numeric order
         files_full = files
         files = []
-        for file in file_list:
+        j_fi=0
+        i_fi=0
+        for file_num in file_list:
             flag = False
-            for f in files_full:
-                if file in f:
-                    files.append(f)
-                    flag = True
-                    break
+            for f in files_full[j_fi:]:
+                if ME:
+                    if file_num in '_'.join(f.rsplit('_',2)[-2:]): # match acq number to file path for ME data
+                        j_fi=i_fi
+                        files.append(f)
+                        flag = True
+                        break
+                else:
+                    if file_num in f.rsplit('_',1)[-1]: # match acq number to file path
+                        j_fi=i_fi
+                        files.append(f)
+                        flag = True
+                        break
             if flag == True:
                 continue
     if not files:
         print(f"No more {file_type} files were found in {in_dir}/{og_sub}, with search terms: {exts}")
         return tasksLookedAt, file_log, "Done"
     file_list = []
     for f in files:
@@ -831,14 +860,19 @@
         file_list_full = file_list
         file_list = []
         for file in file_list_full:
             if not 'EPI' in file:
                 file_list.append(file)
         if not file_list:
             file = ''
+        elif types:
+            if echo:
+                file = file_list[int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"])*i+(echo_num-1)]
+            else:
+                file = file_list[i]
         else:
             file = file_list[0]
     if not file: # if no files are found
         if types:
             return tasksLookedAt, file_log, "Return"
         if file_type == 'func':
             print(f"No more func files for {og_sub}")
@@ -853,14 +887,16 @@
     if fill_it == '_': # if no scan parameters, empty the string
         fill_it = ''
     # - counting - #
     if echo:
         if types:
             numb = task_ord[:i+1].count(task_ord[i])
             run_num = numb
+            if echo_num == int(user_info[file_type][f"input_Task-{task_cat+1}-echo"]):
+                tasksLookedAt.append(task_cat) # add current occurance to task list
         else:
             occur = tasksLookedAt.count(task_cat) # counts occurance of task
             run_num = occur + 1 # run number based on how many times that task occured
             if echo_num == int(user_info[file_type][f"input_Task-{task_cat+1}-echo"]):
                 tasksLookedAt.append(task_cat) # add current occurance to task list
     else:
         occur = tasksLookedAt.count(task_cat) # counts occurance of task
@@ -914,15 +950,15 @@
         if not file_exists(json_new):
             if types:
                 shutil.copy(json_file, json_new) # copy file to new location if doing so for fmap 'intended for'
             else:
                 os.rename(json_file, json_new) # rename file
             json_edit(json_new, file_type, f_sub, og_sub, user_info) # edit json files to include necessary information
         elif not types:
-            with open(json_new, 'r') as file:
+            with open(json_new, 'r') as file: # Error on Brandons
                 data = json.load(file)
             if 'PhaseEncodingDirection' in data.keys():
                 PhaseEncodingDirection = data['PhaseEncodingDirection']
             os.rename(json_file, json_new) # rename file
             json_edit(json_new, file_type, f_sub, og_sub, user_info) # edit json files to include necessary information
             with open(json_new, 'r') as file:
                 datum = json.load(file)
@@ -997,30 +1033,35 @@
                     os.rename(file, new) # rename file
             else:
                 buf = True
             if ext == '.json':
                 if buf and not types:
                     with open(new, 'r') as this:
                         data = json.load(this)
-                    PhaseEncodingDirection = data['PhaseEncodingDirection']
+                    for value in data.keys():
+                        if 'PhaseEncodingDirection' in value:
+                            PhaseEncodingDirection = data[value]
+                        elif 'PhaseEncodingAxis' == value:
+                            PhaseEncodingDirection = data[value]
                     os.rename(file, new) # rename file
                     json_edit(new, file_type, f_sub, og_sub, user_info) # edit json files to include necessary information
                     with open(new, 'r') as this:
                         datum = json.load(this)
                     datum['PhaseEncodingDirection'] = PhaseEncodingDirection
                     with open(new, 'w') as this:
                         json.dump(datum, this, indent=4)
                 else:
                     json_edit(new, file_type, f_sub, og_sub, user_info, add_dict) # edit json files to include necessary information
     return tasksLookedAt, file_log, "Next"
         
                 
 # - organize all data and call function to find and rename files - #
 def BIDSit(sub, user_info, *types):
-    print(sub)
+    if not types:
+        print(f"\n{sub}")
     # - define variables in use - #
     WDIR = user_info['out_dir'] # file output (where the work is done)
     mkdir(WDIR, 'rawdata')
     mkdir(WDIR, 'derivatives')
     in_dir = user_info['WDIR'] # file input
     in_dir_og = in_dir
     if not 'tempdata' in in_dir: # make tempdata the folder we are editing to make sure we dont mess things up
@@ -1138,25 +1179,20 @@
         exts = variables[file_type]['key_words']
         if types:
             tasksLookedAt=types[2]
         else:
             tasksLookedAt=[]
         for i in range(scan_num):
             stop = False
-            if f"input_Task-{task_ord[i]+1}-echo" in user_info[file_type].keys() and int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"]) >1: # if multi-echo data
-                for echo in range(1, int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"])+1):
-                    tasksLookedAt, file_log, code = BIDSgo(og_sub, i, user_info, file_type, tasksLookedAt, exts, endings, menu, scans, task_ord, task_names, file_log, variables, echo)
-                    if code == 'Done':
-                        stop = True
-                        break
-            elif types: # if working for "intended for"
+            if types: # if working for "intended for"
                 i = types[1]
                 if f"input_Task-{task_ord[i]+1}-echo" in user_info[file_type].keys() and int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"]) >1: # if multi-echo data
                     for echo in range(1, int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"])+1):
                         tasksLookedAt, file_log, code = BIDSgo(og_sub, i, user_info, file_type, tasksLookedAt, exts, endings, menu, scans, task_ord, task_names, file_log, variables, echo, types)
+                        
                         if code == 'Done':
                             stop = True
                             break
                 else: # if single echo data
                     tasksLookedAt, file_log, code = BIDSgo(og_sub, i, user_info, file_type, tasksLookedAt, exts, endings, menu, scans, task_ord, task_names, file_log, variables, types)
                 if code == 'Return':
                     return
@@ -1168,19 +1204,27 @@
                     with open(f"{WDIR}/BIDSit/Change_logs/{f_sub}/{file_type}_change_log.json", 'w') as file:
                         json.dump(file_log, file, indent=4)
                 else:
                     mkdir(f"{WDIR}/BIDSit/Change_logs/{f_sub}")
                     with open(f"{WDIR}/BIDSit/Change_logs/{f_sub}/{file_type}_change_log.json", 'w') as file:
                         json.dump(file_log, file, indent=4)
                 if f"input_Task-{task_ord[i]+1}-echo" in user_info[file_type].keys() and int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"]) >1: # send back file names to .json edit
-                    return [file_log['changes'][f"scan {i+1} echo {echo_num} new"] for echo_num in range(1, int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"])+1)]
+                    return [[file_log['changes'][f"scan {i+1} echo {echo_num} new"] for echo_num in range(1, int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"])+1)], tasksLookedAt]
                 else:
                     return [[file_log['changes'][f"scan {i+1} new"]], tasksLookedAt]
+            elif f"input_Task-{task_ord[i]+1}-echo" in user_info[file_type].keys() and int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"]) >1: # if multi-echo data
+                for echo in range(1, int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"])+1):
+                    tasksLookedAt, file_log, code = BIDSgo(og_sub, i, user_info, file_type, tasksLookedAt, exts, endings, menu, scans, task_ord, task_names, file_log, variables, echo)
+                    if code == 'Done':
+                        stop = True
+                        break
             else: # all other data
                 tasksLookedAt, file_log, code = BIDSgo(og_sub, i, user_info, file_type, tasksLookedAt, exts, endings, menu, scans, task_ord, task_names, file_log, variables)
+                if code == 'Done':
+                    stop = True
             if stop:
                 break
         if dir_exists(f"{WDIR}/BIDSit/Change_logs/{f_sub}"): # add to change_log file
             if file_exists(f"{WDIR}/BIDSit/Change_logs/{f_sub}/{file_type}_change_log.json"):
                 with open(f"{WDIR}/BIDSit/Change_logs/{f_sub}/{file_type}_change_log.json", 'r') as file:
                     data_add = json.load(file)
                     file_log['changes'] = {**data_add['changes'], **file_log['changes']}
@@ -1193,16 +1237,18 @@
                 
 # - Edit json files - #
 def json_edit(json_f, file_type, f_sub, og_sub, info, *dicts):
     sub_solo = f_sub.split('/')[0]
     dic = {}
     for dict in dicts:
         dic = {**dic, **dict}
-    with open(json_f, 'r') as file:
+    with open(json_f, 'r', encoding='utf-8') as file: # removed encoding='utf-8' to get it to work with Brandons data
         data = json.load(file)
+#        file_string = file.read()
+#        data = json.loads(file_string, object_hook=ascii_encode_dict)
         for value in data.keys():
             if 'WaterFatShift' in value:
                 WaterFatShift = data[value]
             elif 'ImagingFrequency' in value:
                 ImagingFrequency = data[value]
             elif 'ReconMatrixPE' in value:
                 ReconMatrixPE = data[value]
@@ -1210,14 +1256,16 @@
                 EchoTrainLength = data[value]
             elif 'EstimatedEffectiveEchoSpacing' in value:
                 EstimatedEffectiveEchoSpacing = data[value]
             elif 'EstimatedTotalReadoutTime' in value:
                 EstimatedTotalReadoutTime = data[value]
             elif 'PhaseEncodingDirection' == value:
                 PhaseEncodingDirection = data[value]
+            elif 'PhaseEncodingAxis' == value:
+                PhaseEncodingDirection = data[value]
         try :
             WaterFatShift
             ImagingFrequency
             ReconMatrixPE
             EchoTrainLength
         except NameError:
             add_dict = {}
@@ -1255,15 +1303,14 @@
                 files = []
                 files_full = []
                 tasksLookedAt = []
                 for item in f_list:
                     file_t = item.split()[0] # file type to look at
                     t_num = int(item.split()[-1])-1 # scan to look at
                     if file_t in info:
-                        print(f"running BIDSit for on {file_t} {t_num} for {og_sub}")
                         these, tasksLookedAt = BIDSit(og_sub, info, file_t, t_num, tasksLookedAt)
                         that = []
                         for f in these:
                             that.append("bids::" + f.split('rawdata/')[-1])
                         files = files + that
                         files_full = files_full + these
                 data['IntendedFor'] = files
@@ -1289,17 +1336,14 @@
                         elif data['PhaseEncodingDirection'] == "j":
                             dict_add = {'PhaseEncodingDirection': "j-"}
                         elif data['PhaseEncodingDirection'] == "i-":
                             dict_add = {'PhaseEncodingDirection': "i"}
                         elif data['PhaseEncodingDirection'] == "i":
                             dict_add = {'PhaseEncodingDirection': "i-"}
                         datum = {**datum, **dict_add}
-                        print("Changed PhaseEncodingDirection to: ", datum['PhaseEncodingDirection'] )
-                    else:
-                        print("Changed PhaseEncodingDirection to: ", datum['PhaseEncodingDirection'] )
                 with open(item, 'w') as this:
                     json.dump(datum, this, indent=4)
                     
 ### --- MISC Functions --- ###
 # - make a directory - #
 def mkdir(path,extension=''):
     path = os.path.join(path, extension)
@@ -1345,10 +1389,10 @@
 def copy_it(src, dst):
     try:
         shutil.copytree(src, dst)
     except OSError as exc:
         if exc.errno in (errno.ENOTDIR, errno.EINVAL):
             shutil.copy(src, dst)
         else: raise
-    
+        
 if __name__ == '__main__':
     DOit()
```

### Comparing `BIDSit-0.0.9/src/BIDSit/version.py` & `bidsit-0.1.0/src/BIDSit/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 # Script Name: version.py                                                    #
 #                                                                            #
 # Description: specifies version for BIDSit                                  #
 #                                                                            #
 # Author:      Jen Burrell (April 17th, 2023)                                #
 #============================================================================#
 
-__version__ = '0.0.9'
+__version__ = '0.1.0'
```

### Comparing `BIDSit-0.0.9/src/BIDSit.egg-info/PKG-INFO` & `bidsit-0.1.0/src/BIDSit.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: BIDSit
-Version: 0.0.9
+Version: 0.1.0
 Summary: A BIDS conversion tool for fMRI data
 Home-page: https://github.com/jenburrell/BIDSit
 Author: Jen Burrell
-Author-email: jenbur@psych.ubc.ca
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
+Author-email: Jen Burrell <jenbur@psych.ubc.ca>
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+Requires-Dist: PySimpleGUI<=5.0.0
+Requires-Dist: natsort>=8.3.1
 Provides-Extra: dev
+Requires-Dist: pytest>=3.7; extra == "dev"
 
 BIDSit
 ===========
 
 The ``BIDSit`` project is a toolbox to organize MRI data into BIDS format written in Python.
 
 Installation
```

