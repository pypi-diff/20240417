# Comparing `tmp/cPredictor-0.3.1-py3-none-any.whl.zip` & `tmp/cPredictor-0.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 19472 bytes, number of entries: 11
--rw-r--r--  2.0 unx    38247 b- defN 24-Feb-07 12:22 cPredictor/SVM_prediction.py
--rw-r--r--  2.0 unx      354 b- defN 24-Feb-07 12:22 cPredictor/__init__.py
--rw-r--r--  2.0 unx     6777 b- defN 24-Feb-07 12:22 cPredictor/tests/SVM_prediction_test.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-07 12:22 cPredictor/tests/__init__.py
--rw-r--r--  2.0 unx     2398 b- defN 24-Feb-07 12:22 cPredictor/tests/cPredictor_test_model.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Feb-07 12:24 cPredictor-0.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3349 b- defN 24-Feb-07 12:24 cPredictor-0.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-07 12:24 cPredictor-0.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      227 b- defN 24-Feb-07 12:24 cPredictor-0.3.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Feb-07 12:24 cPredictor-0.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      941 b- defN 24-Feb-07 12:24 cPredictor-0.3.1.dist-info/RECORD
-11 files, 63753 bytes uncompressed, 17864 bytes compressed:  72.0%
+Zip file size: 20111 bytes, number of entries: 11
+-rw-r--r--  2.0 unx    42101 b- defN 24-Apr-17 06:36 cPredictor/SVM_prediction.py
+-rw-r--r--  2.0 unx      354 b- defN 24-Apr-17 06:36 cPredictor/__init__.py
+-rw-r--r--  2.0 unx     6922 b- defN 24-Apr-17 06:36 cPredictor/tests/SVM_prediction_test.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 06:36 cPredictor/tests/__init__.py
+-rw-r--r--  2.0 unx     2398 b- defN 24-Apr-17 06:36 cPredictor/tests/cPredictor_test_model.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-17 06:36 cPredictor-0.3.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3349 b- defN 24-Apr-17 06:36 cPredictor-0.3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 06:36 cPredictor-0.3.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      227 b- defN 24-Apr-17 06:36 cPredictor-0.3.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-17 06:36 cPredictor-0.3.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      941 b- defN 24-Apr-17 06:36 cPredictor-0.3.2.dist-info/RECORD
+11 files, 67752 bytes uncompressed, 18503 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: cPredictor/tests/__init__.py
 Comment: 
 
 Filename: cPredictor/tests/cPredictor_test_model.py
 Comment: 
 
-Filename: cPredictor-0.3.1.dist-info/LICENSE
+Filename: cPredictor-0.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: cPredictor-0.3.1.dist-info/METADATA
+Filename: cPredictor-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: cPredictor-0.3.1.dist-info/WHEEL
+Filename: cPredictor-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: cPredictor-0.3.1.dist-info/entry_points.txt
+Filename: cPredictor-0.3.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: cPredictor-0.3.1.dist-info/top_level.txt
+Filename: cPredictor-0.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cPredictor-0.3.1.dist-info/RECORD
+Filename: cPredictor-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cPredictor/SVM_prediction.py

```diff
@@ -1,41 +1,49 @@
 import argparse
 import gc
 import os
 import numpy as np
 import pandas as pd
+import pyarrow as pa
 import scanpy as sc
+from scanpy import read_h5ad
 import time as tm
 import seaborn as sns
 import matplotlib
 import matplotlib.pyplot as plt
-from sklearnex import patch_sklearn 
-patch_sklearn()
-from sklearn.svm import LinearSVC
+#import matplotlib.gridspec as gridspec
+#from sklearnex import patch_sklearn
+#patch_sklearn()
 from sklearn.calibration import CalibratedClassifierCV
+#from sklearn.calibration import CalibrationDisplay
+#from sklearn.calibration import calibration_curve
 from sklearn.metrics import confusion_matrix
+#from sklearn.model_selection import train_test_split
 from sklearn.model_selection import StratifiedKFold
 from sklearn.model_selection import KFold
 from sklearn.preprocessing import LabelEncoder
 from sklearn.preprocessing import MinMaxScaler
 from sklearn.metrics import f1_score
 from sklearn.metrics import accuracy_score
 from sklearn.metrics import precision_score
-import pyarrow as pa
-from scanpy import read_h5ad
+from sklearn.svm import LinearSVC
 import logging
+import pickle
+import joblib
+import json
 
 class CpredictorClassifier():
     def __init__(self, Threshold_rej, rejected, OutputDir):
         self.scaler = MinMaxScaler()
         self.Classifier = LinearSVC(dual = False, random_state = 42, class_weight = 'balanced', max_iter = 2500)
         self.threshold = Threshold_rej
         self.rejected = rejected
         self.output_dir = OutputDir
         self.expression_treshold = 162
+        self.kf = StratifiedKFold(n_splits = 3, shuffle = True, random_state = 42)
 
     def expression_cutoff(self, Data, LabelsPath):
         logging.info(f'Selecting genes based on an summed expression threshold of minimally {self.expression_treshold} in each cluster')
         labels = pd.read_csv(LabelsPath,index_col=False)
         h5ad_object = Data.copy()
         cluster_id = 'labels'
         h5ad_object.obs[cluster_id] = labels.iloc[:, 0].tolist()
@@ -76,14 +84,38 @@
         self.rejected = True
         self.threshold = threshold
         self.output_dir = output_dir
         logging.info('Running SVMrejection')
         kf = StratifiedKFold(n_splits = 3, shuffle = True, random_state = 42)
         clf = CalibratedClassifierCV(self.Classifier, cv=kf)
         clf.fit(data_train, labels_train.ravel())
+        joblib.dump(clf, "data/model_SVMrej.pkl")
+        self.Classifier.get_params()
+        with open('data/params_SVMrej.json', 'w', encoding='utf-8') as outfile:
+            json.dump(self.Classifier.get_params(), outfile)
+        predicted = clf.predict(data_test)
+        prob = np.max(clf.predict_proba(data_test), axis = 1)
+        unlabeled = np.where(prob < self.threshold)
+
+        # For unlabeled values from the SVMrejection put values of strings and integers
+        try:
+            predicted[unlabeled] = 'Unlabeled'
+        except ValueError:
+            unlabeled = list(unlabeled[0])
+            predicted[unlabeled] = 999999
+        self.predictions = predicted
+        self.probabilities = prob
+        self.save_results(self.rejected)
+
+    def predict_only_svmrejection(self, threshold, output_dir, data_test):
+        self.rejected = True
+        self.threshold = threshold
+        self.output_dir = output_dir
+        clf = joblib.load("data/model_SVMrej.pkl")
+        logging.info('Running SVMrejection')
         predicted = clf.predict(data_test)
         prob = np.max(clf.predict_proba(data_test), axis = 1)
         unlabeled = np.where(prob < self.threshold)
 
         # For unlabeled values from the SVMrejection put values of strings and integers
         try:
             predicted[unlabeled] = 'Unlabeled'
@@ -95,17 +127,29 @@
         self.save_results(self.rejected)
 
     def fit_and_predict_svm(self, labels_train, output_dir, data_train, data_test):
         self.rejected = False
         self.output_dir = output_dir
         logging.info('Running SVM')
         self.Classifier.fit(data_train, labels_train.ravel())
+        joblib.dump(self.Classifier, "data/model_SVM.pkl")
+        self.Classifier.get_params()
+        with open('data/params_SVM.json', 'w', encoding='utf-8') as outfile:
+            json.dump(self.Classifier.get_params(), outfile)
         self.predictions = self.Classifier.predict(data_test)
         self.save_results(self.rejected)
 
+    def predict_only_svm(self, output_dir, data_test):
+        self.rejected = False
+        self.output_dir = output_dir
+        clf = joblib.load("data/model_SVM.pkl")
+        logging.info('Running SVM')
+        self.predictions = clf.predict(data_test)
+        self.save_results(self.rejected)
+
     def save_results(self, rejected):
         self.rejected = rejected
         self.predictions = pd.DataFrame(self.predictions)
         if self.rejected is True:
             self.probabilities = pd.DataFrame(self.probabilities)
             self.predictions.to_csv(f"{self.output_dir}/SVMrej_Pred_Labels.csv", index=False)
             self.probabilities.to_csv(f"{self.output_dir}/SVMrej_Prob.csv", index=False)
@@ -123,78 +167,121 @@
         return self.predictions, self.probabilities
 
     def fit_and_predict_svm(self, labels_train, OutputDir, data_train, data_test):
         # Calls the function from parent class and extends it for the child
         super().fit_and_predict_svm(labels_train, OutputDir, data_train, data_test)
         return self.predictions
 
-def SVM_predict(reference_H5AD, query_H5AD, LabelsPath, OutputDir, rejected=False, Threshold_rej=0.7,meta_atlas=False):
+def SVM_predict(query_H5AD, LabelsPath, OutputDir, reference_H5AD=None, rejected=False, Threshold_rej=0.7, meta_atlas=False):
     '''
     run baseline classifier: SVM
     Wrapper script to run an SVM classifier with a linear kernel on a benchmark dataset with 5-fold cross validation,
     outputs lists of true and predicted cell labels as csv files, as well as computation time.
 
     Parameters:
     reference_H5AD, query_H5AD : H5AD files that produce training and testing data,
         cells-genes matrix with cell unique barcodes as row names and gene names as column names.
     LabelsPath : Cell population annotations file path matching the training data (.csv).
     OutputDir : Output directory defining the path of the exported file.
     rejected: If the flag is added, then the SVMrejected option is chosen. Default: False.
     Threshold_rej : Threshold used when rejecting the cells, default is 0.7.
-    meta_atlas : If the flag is added the predictions will use meta-atlas data.
-    meaning that reference_H5AD and LabelsPath do not need to be specified.
+    meta_atlas : If the flag is added the predictions will use meta_atlas data.
+    This means that reference_H5AD and LabelsPath do not need to be specified.
     '''
     logging.basicConfig(level=logging.DEBUG, 
                         format='%(asctime)s - %(name)s - %(levelname)s - %(message)s', datefmt='%d/%m/%Y %H:%M:%S',
                         filename='cPredictor_predict.log', filemode='w')
-    logging.info('Reading in the reference and query H5AD objects')
     
-    # Load in the cma.h5ad object or use a different reference
-    if meta_atlas is False:
-        training = read_h5ad(reference_H5AD) 
-    if meta_atlas is True:
-        meta_dir = 'data/cma_meta_atlas.h5ad'
-        training = read_h5ad(meta_dir) 
-
     # Get an instance of the Cpredictor class
     cpredictor = CpredictorClassifier(Threshold_rej, rejected, OutputDir)
-    training = cpredictor.expression_cutoff(training, LabelsPath)
-    
+
+    SVM_type = "SVMrej" if rejected is True else "SVM"
+
     # Load in the test data
+    logging.info('Reading in the test data')
     testing = read_h5ad(query_H5AD)
 
     # Checks if the test data contains a raw data slot and sets it as the count value
     try:
         testing = testing.raw.to_adata()
     except AttributeError:
         logging.warning('Query object does not contain raw data, using sparce matrix from adata.X')
         logging.warning('Please manually check if this sparce matrix contains actual raw counts')
 
-    logging.info('Generating training and testing matrices from the H5AD objects')
-    
-    # training data
-    matrix_train = pd.DataFrame.sparse.from_spmatrix(training.X, index=list(training.obs.index.values), columns=list(training.var.features.values))
-
     # testing data
     try: 
         testing.var['features']
     except KeyError:
         testing.var['features'] = testing.var.index
         logging.debug('Setting the var index as var features')
-    
+
     matrix_test = pd.DataFrame.sparse.from_spmatrix(testing.X, index=list(testing.obs.index.values), columns=list(testing.var.features.values))
+
+    # If there is a pregenerated model the pipeline will try to run this first
+    if os.path.exists(f"data/model_{SVM_type}.pkl") and meta_atlas is True:
+        logging.info('Using a predifined model for predictions as well as for subselected genes')
+        
+        with open ('data/mergedgenes', 'rb') as fp:
+            col_one_list = pickle.load(fp)
+
+        missing_cols = list(set(col_one_list) - set(matrix_test.columns.to_list()))
+        length_missing = len(missing_cols)
+
+        if missing_cols:
+            logging.warning(f'Filling in missing values as 0 in test data for {length_missing} genes')
+            logging.warning('Please check the validity of your query H5AD object')
+            matrix_test = matrix_test.reindex(col_one_list, axis=1)
+
+        new_col_values = np.full(len(matrix_test), 0)
+        for col in missing_cols:
+            matrix_test[col] = new_col_values
+
+        matrix_test = matrix_test[matrix_test.columns.intersection(col_one_list)]
+        data_test = matrix_test.to_numpy(dtype="float16")
+
+        logging.info('Processing test data')
+        data_test = cpredictor.preprocess_data_test(data_test)
+
+        if rejected is True:
+            cpredictor.predict_only_svmrejection(Threshold_rej, OutputDir, data_test)
+            cpredictor.save_results(rejected)
+        
+        else:
+            cpredictor.predict_only_svm(OutputDir, data_test)
+            cpredictor.save_results(rejected)
+
+        return
+    
+    logging.info('Reading in the reference and query H5AD objects')
+    # Load in the cma.h5ad object or use a different reference
+    if meta_atlas is False:
+        training = read_h5ad(reference_H5AD) 
+    if meta_atlas is True:
+        meta_dir = 'data/cma_meta_atlas.h5ad'
+        training = read_h5ad(meta_dir) 
+
+    training = cpredictor.expression_cutoff(training, LabelsPath)
+
+    logging.info('Generating training matrix from the H5AD object')
+    
+    # training data
+    matrix_train = pd.DataFrame.sparse.from_spmatrix(training.X, index=list(training.obs.index.values), columns=list(training.var.features.values))
     
     logging.info('Unifying training and testing matrices for shared genes')
     
     # subselect the train matrix for values that are present in both
     df_all = training.var[["features"]].merge(testing.var[["features"]].drop_duplicates(), on=['features'], how='left', indicator=True)
     df_all['_merge'] == 'left_only'
     training1 = df_all[df_all['_merge'] == 'both']
     col_one_list = training1['features'].tolist()
 
+    # Save the list present in both
+    with open('data/mergedgenes', 'wb') as fp:
+        pickle.dump(col_one_list, fp)
+
     matrix_test = matrix_test[matrix_test.columns.intersection(col_one_list)]
     matrix_train = matrix_train[matrix_train.columns.intersection(col_one_list)]
     matrix_train = matrix_train[list(matrix_test.columns)]
     
     logging.info('Number of genes remaining after unifying training and testing matrices: '+str(len(matrix_test.columns)))
     
     # Convert the ordered dataframes back to nparrays
@@ -243,23 +330,27 @@
     Imports the output of the SVM_predictor and saves it to the query_H5AD.
 
     Parameters:
     query_H5AD: H5AD file of datasets of interest.
     OutputDir: Output directory defining the path of the exported SVM_predictions.
     SVM_type: Type of SVM prediction, SVM (default) or SVMrej.
     Replicates: A string value specifying a column in query_H5AD.obs.
-    colord: A .tsv file with the order of the meta-atlas and corresponding colors.
-    meta_atlas : If the flag is added the predictions will use meta-atlas data.
+    colord: A .tsv file with the order of the meta_atlas and corresponding colors.
+    meta_atlas : If the flag is added the predictions will use meta_atlas data.
     show_bar: Shows bar plots depending on the SVM_type, split over replicates.
 
     '''
     logging.basicConfig(level=logging.DEBUG, 
                         format='%(asctime)s - %(name)s - %(levelname)s - %(message)s', datefmt='%d/%m/%Y %H:%M:%S',
                         filename='cPredictor_import.log', filemode='w')
     logging.info('Reading query data')
+
+    # Makes a figure dir in the output dir if it does not exist yet
+    if not os.path.isdir(f"{OutputDir}/figures"):
+        os.makedirs(f"{OutputDir}/figures")
     
     adata = read_h5ad(query_H5AD)
     SVM_key = f"{SVM_type}_predicted"
 
     # Load in the object and add the predicted labels
     logging.info('Adding predictions to query data')
     for file in os.listdir(OutputDir):
@@ -366,15 +457,15 @@
 
         fig.legend(loc=7,title="Cell state")
 
         stacked_data.plot(kind="bar", stacked=True, legend = False, ax=ax[1],color=lstval[::-1], rot=45, title='Percentage of cells')
 
         fig.tight_layout()
         fig.subplots_adjust(right=0.9)
-        fig.savefig(f"figures/{SVM_key}_bar.pdf", bbox_inches='tight')
+        fig.savefig(f"{OutputDir}/figures/{SVM_key}_bar.pdf", bbox_inches='tight')
         plt.close(fig)
     else:
         None
 
     if SVM_key == "SVM_predicted":
         logging.info('Plotting label prediction certainty scores')
         category_colors = category_colors
@@ -392,21 +483,21 @@
         plt.ylabel('Density')
         plt.title('Stacked Density Plots of Prediction Certainty Scores by Cell State')
 
         # Add a legend
         plt.legend(bbox_to_anchor=(1.04, 1), loc="upper left")
 
         # Saving the density plot
-        fig.savefig("figures/Density_prediction_scores.pdf", bbox_inches='tight')
+        fig.savefig(f"{OutputDir}/figures/Density_prediction_scores.pdf", bbox_inches='tight')
         plt.close(fig)
     else:
         None
         
     logging.info('Saving H5AD file')
-    adata.write_h5ad(f"{SVM_key}.h5ad")
+    adata.write_h5ad(f"{OutputDir}/{SVM_key}.h5ad")
     return
 
 def SVM_performance(reference_H5AD, LabelsPath, OutputDir, rejected=True, Threshold_rej=0.7, fold_splits=5):
     '''
     Tests performance of SVM model based on a reference H5AD dataset.
 
     Parameters:
@@ -415,14 +506,19 @@
     SVM_type: Type of SVM prediction, SVM or SVMrej (default).
     '''
     logging.basicConfig(level=logging.DEBUG, 
                         format='%(asctime)s - %(name)s - %(levelname)s - %(message)s', datefmt='%d/%m/%Y %H:%M:%S',
                         filename='cPredictor_performance.log', filemode='w')
 
     logging.info('Reading in the data')
+
+    # Makes a figure dir in the output dir if it does not exist yet
+    if not os.path.isdir(f"{OutputDir}/figures"):
+        os.makedirs(f"{OutputDir}/figures")
+
     Data = read_h5ad(reference_H5AD)
 
     # Using the child class of the CpredictorClassifier to process the data
     cpredictorperf = CpredictorClassifierPerformance(Threshold_rej, rejected, OutputDir)
     
     Data = cpredictorperf.expression_cutoff(Data, LabelsPath)
 
@@ -458,16 +554,14 @@
         # Store the indices of the training and test sets for each fold
         train_indices.append(list(train_index))
         test_indices.append(list(test_index))
 
     # Run the SVM model
     test_ind = test_indices
     train_ind = train_indices
-    #if SVM_type == "SVMrej":
-    #    clf = CalibratedClassifierCV(Classifier, cv=3)
 
     tr_time=[]
     ts_time=[]
     truelab = []
     pred = []
     prob_full = []
 
@@ -546,30 +640,30 @@
     cnf_matrix = cnf_matrix.loc[true["True"].astype(str).unique(), pred["Predicted"].astype(str).unique()]
     cnf_matrix = cnf_matrix.div(cnf_matrix.sum(1), axis=0)
 
     cnf_matrix = cnf_matrix.sort_index(axis=1)
     cnf_matrix = cnf_matrix.sort_index()
 
     # Plot png
-    sns.set(font_scale=0.8)
+    sns.set_theme(font_scale=0.8)
     cm = sns.clustermap(cnf_matrix.T, cmap="Blues", annot=True,fmt='.2%', row_cluster=False,col_cluster=False)
-    cm.savefig(f"figures/{SVM_type}_cnf_matrix.png")
+    cm.savefig(f"{OutputDir}/figures/{SVM_type}_cnf_matrix.png")
     return F1score,acc_score,prec_score
 
 def SVM_pseudobulk(condition_1, condition_1_batch, condition_2, condition_2_batch, Labels_1, OutputDir="pseudobulk_output/", min_cells=50, SVM_type="SVM"):
     '''
     Produces pseudobulk RNA-seq count files and sample files of either technical or biological replicates.
     It produces pseudobulk of all labels from LabelsPath against predicted labels after SVMprediction.
     Moreover, it produces overall pseudobulk of condition_1 vs condition_2 split by indicated batches.
 
     Parameters:
     condition_1, condition_2 : H5AD files with cells-genes matrix with cell unique barcodes as 
-        row names and gene names as column names. Condition_1 should be the meta-atlas and
+        row names and gene names as column names. Condition_1 should be the meta_atlas and
         condition_2 should be the queried object.
-    condition_1_batch : batch name for the meta-atlas object replicates (biological, technical etc.)
+    condition_1_batch : batch name for the meta_atlas object replicates (biological, technical etc.)
     condition_2_batch: batch name for the queried object
     Labels_1 : Cell population annotations file path matching the training data (.csv) or 
         a string that specifies an .obs value in condition 1.
     OutputDir: The directory into which the results are outputted; default: "pseudobulk_output/"
     '''
     logging.basicConfig(level=logging.DEBUG, 
                         format='%(asctime)s - %(name)s - %(levelname)s - %(message)s', datefmt='%d/%m/%Y %H:%M:%S',
@@ -739,39 +833,40 @@
         cond_samples_file = str(outputdir+str(cluster_id)+"_samples.tsv")
         cond_samples.to_csv(cond_samples_file, sep="\t", index=False)
         logging.info('Finished constructing contrast between conditions for: '+str(cluster_id))
     
     return
 
 def predpars():
+
     # Create the parser
     parser = argparse.ArgumentParser(description='Run SVM prediction')
 
     # Add arguments
-    parser.add_argument('--reference_H5AD', type=str, help='Path to reference H5AD file')
     parser.add_argument('--query_H5AD', type=str, help='Path to query H5AD file')
     parser.add_argument('--LabelsPath', type=str, help='Path to cell population annotations file')
     parser.add_argument('--OutputDir', type=str, help='Path to output directory')
+    parser.add_argument('--reference_H5AD', type=str, help='Path to reference H5AD file')
     parser.add_argument('--rejected', dest='rejected', action='store_true', help='Use SVMrejected option')
     parser.add_argument('--Threshold_rej', type=float, default=0.7, help='Threshold used when rejecting cells, default is 0.7')
     parser.add_argument('--meta_atlas', dest='meta_atlas', action='store_true', help='Use meta_atlas data')
 
     # Parse the arguments
     args = parser.parse_args()
     
     # check that output directory exists, create it if necessary
     if not os.path.isdir(args.OutputDir):
         os.makedirs(args.OutputDir)
 
     # Call the svm_prediction function with the parsed arguments
     SVM_predict(
-        args.reference_H5AD,
         args.query_H5AD,
         args.LabelsPath,
         args.OutputDir,
+        args.reference_H5AD,
         args.rejected,
         args.Threshold_rej,
         args.meta_atlas)
 
 
 def performpars():
 
@@ -804,15 +899,15 @@
 
     parser = argparse.ArgumentParser(description="Imports predicted results back to H5AD file")
     parser.add_argument("--query_H5AD", type=str, help="Path to query H5AD file")
     parser.add_argument("--OutputDir", type=str, help="Output directory path")
     parser.add_argument("--SVM_type", type=str, help="Type of SVM prediction (SVM or SVMrej)")
     parser.add_argument("--replicates", type=str, help="Replicates")
     parser.add_argument("--colord", type=str, help=".tsv file with meta-atlas order and colors")
-    parser.add_argument("--meta-atlas", dest="meta_atlas", action="store_true", help="Use meta-atlas data")
+    parser.add_argument("--meta_atlas", dest="meta_atlas", action="store_true", help="Use meta-atlas data")
     parser.add_argument("--show_bar", dest="show_bar", action="store_true", help="Plot barplot with SVM labels over specified replicates")
 
     args = parser.parse_args()
 
     SVM_import(
         args.query_H5AD,
         args.OutputDir,
```

## cPredictor/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 from .SVM_prediction import SVM_predict
 from .SVM_prediction import SVM_import
 from .SVM_prediction import SVM_performance
 from .SVM_prediction import SVM_pseudobulk
 from .SVM_prediction import predpars
 from .SVM_prediction import importpars
```

## cPredictor/tests/SVM_prediction_test.py

```diff
@@ -63,43 +63,43 @@
     assert os.path.exists(f'{outdir_unit}SVMrej_Pred_Labels.csv') == 1
 
     
 def test_SVM_import():
 
     SVM_import(query_H5AD=query,OutputDir=outdir_unit,SVM_type="SVM",replicates="time_point")
 
-    assert os.path.exists(f'figures/Density_prediction_scores.pdf') == 1
-    assert os.path.exists(f'SVM_predicted.h5ad') == 1
+    assert os.path.exists(f'{outdir_unit}figures/Density_prediction_scores.pdf') == 1
+    assert os.path.exists(f'{outdir_unit}SVM_predicted.h5ad') == 1
 
 
 def test_SVM_plot_import():
 
     SVM_import(query_H5AD=query,OutputDir=outdir_unit,
       SVM_type="SVM",replicates="time_point",show_bar=True)
 
-    assert os.path.exists(f'figures/SVM_predicted_bar.pdf') == 1
+    assert os.path.exists(f'{outdir_unit}figures/SVM_predicted_bar.pdf') == 1
 
 def test_SVMrej_plot_import():
 
     SVM_import(query_H5AD=query,OutputDir=outdir_unit,
       SVM_type="SVMrej",replicates="time_point",show_bar=True)
 
-    assert os.path.exists(f'figures/SVMrej_predicted_bar.pdf') == 1
+    assert os.path.exists(f'{outdir_unit}figures/SVMrej_predicted_bar.pdf') == 1
 
 def test_SVM_plot_import_meta_atlas():
 
     SVM_import(query_H5AD=query,OutputDir=outdir_unit,colord=colord_tsv,
       SVM_type="SVM",replicates="time_point",show_bar=True,meta_atlas=True)
 
-    assert os.path.exists(f'figures/SVM_predicted_bar.pdf') == 1
+    assert os.path.exists(f'{outdir_unit}figures/SVM_predicted_bar.pdf') == 1
       
 def test_SVM_pseudobulk():
 
     SVM_pseudobulk(condition_1=reference, condition_1_batch="donors", 
-      condition_2="SVM_predicted.h5ad", condition_2_batch="batch", Labels_1=labels)
+      condition_2=f"{outdir_unit}SVM_predicted.h5ad", condition_2_batch="batch", Labels_1=labels)
     assert os.path.exists("pseudobulk_output/full_batch_samples.tsv") == 1
     assert os.path.exists("pseudobulk_output/merged_batch_samples.tsv") == 1
 
 # Issue to still fix, no priority for now
 #def test_SVMrej_pseudobulk():
 
 #    SVM_pseudobulk(condition_1=reference, condition_1_batch="donors", 
@@ -107,20 +107,20 @@
 #      Labels_1=labels,SVM_type="SVMrej")
 #    assert os.path.exists("pseudobulk_output/full_batch_samples.tsv") == 1
 #    assert os.path.exists("pseudobulk_output/merged_batch_samples.tsv") == 1
 
 def test_SVM_performance():
 
     SVM_performance(reference_H5AD=reference,LabelsPath=labels,OutputDir=outdir_unit, rejected=False)
-    assert os.path.exists("figures/SVM_cnf_matrix.png") == 1
+    assert os.path.exists(f"{outdir_unit}figures/SVM_cnf_matrix.png") == 1
     
 def test_SVMrej_performance():
 
     SVM_performance(reference_H5AD=reference,LabelsPath=labels,OutputDir=outdir_unit, rejected=True)
-    assert os.path.exists("figures/SVMrej_cnf_matrix.png") == 1
+    assert os.path.exists(f"{outdir_unit}figures/SVMrej_cnf_matrix.png") == 1
 
 ### END-TO-END
 outdir = "test_output_end_to_end/"
 
 def test_CLI_SVM_predict():
 
     command_to_be_executed = ['SVM_predict',
@@ -150,42 +150,42 @@
     
 def test_CLI_SVM_import():
 
     command_to_be_executed = ['SVM_import',
                               '--query_H5AD', str(query),
                               '--OutputDir', str(outdir),
                               '--SVM_type', str("SVM"),
-                              '--meta-atlas']
+                              '--meta_atlas']
 
     subprocess.run(command_to_be_executed, shell=False, timeout=None,
                    text=True)
-    assert os.path.exists(f'figures/Density_prediction_scores.pdf') == 1
-    assert os.path.exists(f'SVM_predicted.h5ad') == 1
+    assert os.path.exists(f'{outdir}figures/Density_prediction_scores.pdf') == 1
+    assert os.path.exists(f'{outdir}SVM_predicted.h5ad') == 1
 
 
 def test_CLI_SVM_import_plots():
 
     command_to_be_executed = ['SVM_import',
                               '--query_H5AD', str(query),
                               '--OutputDir', str(outdir),
                               '--SVM_type', str("SVM"),
                               '--replicates', str("time_point"),
-                              '--show-bar']
+                              '--show_bar']
 
     subprocess.run(command_to_be_executed, shell=False, timeout=None,
                    text=True)
-    assert os.path.exists(f'figures/SVM_predicted_bar.pdf') == 1
+    assert os.path.exists(f'{outdir}figures/SVM_predicted_bar.pdf') == 1
 
     
 def test_CLI_SVM_pseudobulk():
 
     command_to_be_executed = ['SVM_pseudobulk',
                               '--condition_1', str(reference),
                               '--condition_1_batch', str("donors"),
-                              '--condition_2', str("SVM_predicted.h5ad"),
+                              '--condition_2', str(f"{outdir_unit}SVM_predicted.h5ad"),
                               '--condition_2_batch', str("batch"),
                               '--Labels_1', str(labels)]
 
     subprocess.run(command_to_be_executed, shell=False, timeout=None,
                    text=True)
     assert os.path.exists("pseudobulk_output/full_batch_samples.tsv") == 1
     assert os.path.exists("pseudobulk_output/merged_batch_samples.tsv") == 1
```

## cPredictor/tests/cPredictor_test_model.py

```diff
@@ -24,15 +24,15 @@
 from cPredictor.SVM_prediction import SVM_performance
 os.environ["GIT_PYTHON_REFRESH"] = "quiet"
 import git
 
 reference = "data/cma_meta_atlas.h5ad"
 labels = "data/training_labels_meta.csv"
 outdir = "test_output/"
-cPredictor_version = "0.3.1"
+cPredictor_version = "0.3.2"
 
 metrics = SVM_performance(reference_H5AD=reference,LabelsPath=labels,OutputDir=outdir)
 
 print("Setup tokens")
 # Set environments and passwords
 DAGSHUB_USER_NAME = 'Arts-of-coding'
 DAGSHUB_TOKEN =  os.environ['DH_key']
```

## Comparing `cPredictor-0.3.1.dist-info/LICENSE` & `cPredictor-0.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cPredictor-0.3.1.dist-info/METADATA` & `cPredictor-0.3.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cPredictor
-Version: 0.3.1
+Version: 0.3.2
 Summary: Cell command line predictor
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools ==68.2.2
 Requires-Dist: wheel
 Requires-Dist: python-build
 Requires-Dist: pytest-cov
```

