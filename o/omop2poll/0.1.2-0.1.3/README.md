# Comparing `tmp/omop2poll-0.1.2.tar.gz` & `tmp/omop2poll-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omop2poll-0.1.2.tar", max compression
+gzip compressed data, was "omop2poll-0.1.3.tar", max compression
```

## Comparing `omop2poll-0.1.2.tar` & `omop2poll-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     4515 2024-03-30 02:01:42.491653 omop2poll-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-03-30 02:20:58.191357 omop2poll-0.1.2/omop2poll/__init__.py
--rw-r--r--   0        0        0      725 2024-03-30 02:01:46.503580 omop2poll-0.1.2/omop2poll/codebook.py
--rw-r--r--   0        0        0      338 2024-03-30 02:01:46.506326 omop2poll-0.1.2/omop2poll/load_data.py
--rw-r--r--   0        0        0     1193 2024-03-30 02:01:46.508863 omop2poll-0.1.2/omop2poll/map_responses.py
--rw-r--r--   0        0        0     1511 2024-03-30 02:01:46.512471 omop2poll-0.1.2/omop2poll/pivot_data.py
--rw-r--r--   0        0        0      413 2024-03-30 02:01:46.510585 omop2poll-0.1.2/omop2poll/recode_missing.py
--rw-r--r--   0        0        0    41806 2024-03-30 02:01:46.537607 omop2poll-0.1.2/omop2poll/survey.csv
--rw-r--r--   0        0        0        0 2024-03-30 02:21:19.965168 omop2poll-0.1.2/omop2poll/tests/__init__.py
--rw-r--r--   0        0        0       27 2024-03-30 02:01:46.517346 omop2poll-0.1.2/omop2poll/tests/pivot_n_test.csv
--rw-r--r--   0        0        0       34 2024-03-30 02:01:46.519564 omop2poll-0.1.2/omop2poll/tests/pivot_t_test_text.csv
--rw-r--r--   0        0        0      547 2024-03-30 02:01:46.533897 omop2poll-0.1.2/omop2poll/tests/test_codebook.py
--rw-r--r--   0        0        0      831 2024-03-30 02:01:46.522902 omop2poll-0.1.2/omop2poll/tests/test_load_data.py
--rw-r--r--   0        0        0      756 2024-03-30 02:18:10.182488 omop2poll-0.1.2/omop2poll/tests/test_map_responses.py
--rw-r--r--   0        0        0      866 2024-03-30 02:01:46.526224 omop2poll-0.1.2/omop2poll/tests/test_pivot_data_numeric.py
--rw-r--r--   0        0        0      913 2024-03-30 02:01:46.521352 omop2poll-0.1.2/omop2poll/tests/test_pivot_data_text.py
--rw-r--r--   0        0        0      226 2024-03-30 02:01:46.527845 omop2poll-0.1.2/omop2poll/tests/test_recode_missing.py
--rw-r--r--   0        0        0      800 2024-03-30 02:29:08.474707 omop2poll-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 omop2poll-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      291 2024-04-16 17:33:06.142843 omop2poll-0.1.3/omop2poll/__init__.py
+-rw-r--r--   0        0        0     3564 2024-04-16 17:28:40.040097 omop2poll-0.1.3/omop2poll/codebook.py
+-rw-r--r--   0        0        0     1511 2024-04-16 16:37:21.487473 omop2poll-0.1.3/omop2poll/map_responses.py
+-rw-r--r--   0        0        0     1553 2024-04-16 14:50:30.296363 omop2poll-0.1.3/omop2poll/pivot_data.py
+-rw-r--r--   0        0        0      813 2024-04-16 15:10:20.536914 omop2poll-0.1.3/omop2poll/recode_missing.py
+-rw-r--r--   0        0        0    42126 2024-04-16 16:25:24.495072 omop2poll-0.1.3/omop2poll/survey_healthcare.csv
+-rw-r--r--   0        0        0        0 2024-04-16 14:50:30.298363 omop2poll-0.1.3/omop2poll/tests/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-16 14:50:30.298363 omop2poll-0.1.3/omop2poll/tests/pivot_n_test.csv
+-rw-r--r--   0        0        0       37 2024-04-16 14:50:30.298363 omop2poll-0.1.3/omop2poll/tests/pivot_t_test_text.csv
+-rw-r--r--   0        0        0      570 2024-04-16 14:50:30.299363 omop2poll-0.1.3/omop2poll/tests/test_codebook.py
+-rw-r--r--   0        0        0      853 2024-04-16 14:50:30.300363 omop2poll-0.1.3/omop2poll/tests/test_load_data.py
+-rw-r--r--   0        0        0      778 2024-04-16 14:50:30.300363 omop2poll-0.1.3/omop2poll/tests/test_map_responses.py
+-rw-r--r--   0        0        0      894 2024-04-16 14:50:30.301363 omop2poll-0.1.3/omop2poll/tests/test_pivot_data_numeric.py
+-rw-r--r--   0        0        0      940 2024-04-16 14:50:30.301363 omop2poll-0.1.3/omop2poll/tests/test_pivot_data_text.py
+-rw-r--r--   0        0        0      233 2024-04-16 14:50:30.301363 omop2poll-0.1.3/omop2poll/tests/test_recode_missing.py
+-rw-r--r--   0        0        0      527 2024-04-16 17:05:39.472430 omop2poll-0.1.3/omop2poll/tests/trial.py
+-rw-r--r--   0        0        0      835 2024-04-16 17:45:53.231110 omop2poll-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4549 2024-04-16 14:50:30.293363 omop2poll-0.1.3/README.md
+-rw-r--r--   0        0        0     5570 1970-01-01 00:00:00.000000 omop2poll-0.1.3/PKG-INFO
```

### Comparing `omop2poll-0.1.2/README.md` & `omop2poll-0.1.3/README.md`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-The **'omop2poll'** Python package offers a comprehensive solution for transforming standardized response codes from the Observational Medical Outcomes Partnership (OMOP) Common Data Model (CDM) survey variables into numeric values, streamlining the data preparation process. By automating the mapping and conversion of response codes, as well as the handling of missing data, it makes data analysis more accessible and reliable. The package provides a range of functions designed to help researchers and data analysts efficiently work through OMOP CDM survey data, ensuring accurate mappings of responses and effective management of data discrepancies. This package is a helpful tool for those working with OMOP CDM survey data, offering a path to more profound and accurate analyses by dramatically lowering the burden of data preprocessing.
-
-## load_data.py
->
->**load_survey_data(filename='survey.csv')**: Loads survey data from a CSV file into a pandas DataFrame. This function takes an optional filename argument, which defaults to 'healthcare_survey.csv'. It constructs the file path by joining the current working directory with the specified filename. If the file does not exist at the constructed path, it raises a FileNotFoundError. Finally, it reads the CSV file into a DataFrame using pandas and returns this DataFrame.
->
-
-## map_responses.py
-
->
->**map_responses(input_data)**: Maps numeric and text responses from a survey to their corresponding questions based on a preloaded survey data file. This function first calls load_survey_data() without arguments to load the default survey dataset. It then creates two mappings: one for numeric answers (mapping_numeric) and one for text answers (mapping_text), grouped by question_concept_id. 
->
->The function iterates over the input_data DataFrame, updating each row with the corresponding answer_numeric and answer_text based on the mappings. If an answer_text is numeric (detected as either int, float, or digit-containing string), it ensures the text remains as a string. The function returns the updated input_data DataFrame with the mapped answers.
->
-
-## pivot_data.py
-
->
->**pivot_data_numeric(filename)**: Pivots a dataset to structure numeric survey responses in a wide format. The function checks if the specified file exists; if not, it prints an error message and returns. It reads the data from the file into a DataFrame, then pivots this DataFrame so that each row represents a respondent and each column represents a question, with cells containing the numeric answers. 
->
->The column names are prefixed with 'q' to denote question IDs. The pivoted DataFrame is then saved to a new CSV file with a filename prefixed by 'pivot_n_'. The function concludes by printing the name of the newly saved file.
->
->**pivot_data_text(filename)**: Similar to pivot_data_numeric, but pivots text responses instead. It processes and pivots the dataset to structure text survey responses in a wide format, follows the same file existence check, reading, and pivoting process, but focuses on answer_text values. The output file is named with a 'pivot_t_' prefix, and the function notifies the user of the successfully saved file.
->
-
-## recode_missing.py
->
->**recode_missing_values(input_data)**: Recodes missing values in a dataset with NaN (Not a Number). This function supports both CSV and Excel files. It identifies missing values based on a predefined list ([-99, -98, -97]) and uses pandas to read the file, recoding occurrences of these values with NaN. The function raises a ValueError if the input file is not in one of the supported formats.
->
-
-## codebook.py
->
->**create_codebook(df)**: Generates a codebook from a DataFrame containing survey data. The function selects relevant columns (question_concept_id, question, answer_concept_id, answer_numeric, answer_text), removes duplicates, and sorts the entries by question_concept_id to create the codebook DataFrame. This DataFrame is returned for further use or inspection.
->
+The **'omop2poll'** Python package offers a comprehensive solution for transforming standardized response codes from the Observational Medical Outcomes Partnership (OMOP) Common Data Model (CDM) survey variables into numeric values, streamlining the data preparation process. By automating the mapping and conversion of response codes, as well as the handling of missing data, it makes data analysis more accessible and reliable. The package provides a range of functions designed to help researchers and data analysts efficiently work through OMOP CDM survey data, ensuring accurate mappings of responses and effective management of data discrepancies. This package is a helpful tool for those working with OMOP CDM survey data, offering a path to more profound and accurate analyses by dramatically lowering the burden of data preprocessing.
+
+## load_data.py
+>
+>**load_survey_data(filename='survey.csv')**: Loads survey data from a CSV file into a pandas DataFrame. This function takes an optional filename argument, which defaults to 'healthcare_survey.csv'. It constructs the file path by joining the current working directory with the specified filename. If the file does not exist at the constructed path, it raises a FileNotFoundError. Finally, it reads the CSV file into a DataFrame using pandas and returns this DataFrame.
+>
+
+## map_responses.py
+
+>
+>**map_responses(input_data)**: Maps numeric and text responses from a survey to their corresponding questions based on a preloaded survey data file. This function first calls load_survey_data() without arguments to load the default survey dataset. It then creates two mappings: one for numeric answers (mapping_numeric) and one for text answers (mapping_text), grouped by question_concept_id. 
+>
+>The function iterates over the input_data DataFrame, updating each row with the corresponding answer_numeric and answer_text based on the mappings. If an answer_text is numeric (detected as either int, float, or digit-containing string), it ensures the text remains as a string. The function returns the updated input_data DataFrame with the mapped answers.
+>
+
+## pivot_data.py
+
+>
+>**pivot_data_numeric(filename)**: Pivots a dataset to structure numeric survey responses in a wide format. The function checks if the specified file exists; if not, it prints an error message and returns. It reads the data from the file into a DataFrame, then pivots this DataFrame so that each row represents a respondent and each column represents a question, with cells containing the numeric answers. 
+>
+>The column names are prefixed with 'q' to denote question IDs. The pivoted DataFrame is then saved to a new CSV file with a filename prefixed by 'pivot_n_'. The function concludes by printing the name of the newly saved file.
+>
+>**pivot_data_text(filename)**: Similar to pivot_data_numeric, but pivots text responses instead. It processes and pivots the dataset to structure text survey responses in a wide format, follows the same file existence check, reading, and pivoting process, but focuses on answer_text values. The output file is named with a 'pivot_t_' prefix, and the function notifies the user of the successfully saved file.
+>
+
+## recode_missing.py
+>
+>**recode_missing_values(input_data)**: Recodes missing values in a dataset with NaN (Not a Number). This function supports both CSV and Excel files. It identifies missing values based on a predefined list ([-99, -98, -97]) and uses pandas to read the file, recoding occurrences of these values with NaN. The function raises a ValueError if the input file is not in one of the supported formats.
+>
+
+## codebook.py
+>
+>**create_codebook(df)**: Generates a codebook from a DataFrame containing survey data. The function selects relevant columns (question_concept_id, question, answer_concept_id, answer_numeric, answer_text), removes duplicates, and sorts the entries by question_concept_id to create the codebook DataFrame. This DataFrame is returned for further use or inspection.
+>
 >**print_codebook(codebook_df)**: Prints the provided codebook DataFrame in a readable format. It attempts to use the tabulate library to print the DataFrame with headers, formatted as an SQL-style table. If tabulate is not installed, it falls back to pandas' built-in printing options, adjusting the display settings to ensure that all data is visible without truncation. This function is useful for displaying the codebook in a terminal or other environments where a visual representation of the DataFrame is beneficial.
```

### Comparing `omop2poll-0.1.2/omop2poll/map_responses.py` & `omop2poll-0.1.3/omop2poll/map_responses.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,38 @@
-import pandas as pd
-from omop2poll.load_data import load_survey_data
-
-
-def map_responses(input_data):
-    survey_data = load_survey_data()
-
-    mapping_numeric = survey_data.groupby('question_concept_id').apply(
-        lambda x: dict(zip(x['answer_concept_id'], x['answer_numeric']))).to_dict()
-
-    mapping_text = survey_data.groupby('question_concept_id').apply(
-        lambda x: dict(zip(x['answer_concept_id'], x['answer_text'].str.strip()))).to_dict()
-
-    input_data['answer_numeric'] = None
-    input_data['answer_text'] = None
-
-    for idx, row in input_data.iterrows():
-        question_id = row['question_concept_id']
-        answer_id = row['answer_concept_id']
-
-        input_data.at[idx, 'answer_numeric'] = mapping_numeric.get(question_id, {}).get(answer_id, None)
-        input_data.at[idx, 'answer_text'] = mapping_text.get(question_id, {}).get(answer_id, None)
-
-        if isinstance(input_data.at[idx, 'answer_text'], (int, float)):
-            input_data.at[idx, 'answer_text'] = str(input_data.at[idx, 'answer_text'])
-        elif isinstance(input_data.at[idx, 'answer_text'], str) and input_data.at[idx, 'answer_text'].isdigit():
-            pass
-
-    return input_data
+import pandas as pd
+import os
+
+
+def load_survey_data(filename='survey_healthcare.csv'):
+    current_dir = os.path.dirname(os.path.realpath(__file__))
+
+    file_path = os.path.join(current_dir, filename)
+    if not os.path.exists(file_path):
+        raise FileNotFoundError(f"File path {file_path} does not exist.")
+    return pd.read_csv(file_path)
+
+
+def map_responses(input_data):
+    survey_data = load_survey_data()
+
+    mapping_numeric = survey_data.groupby('question_concept_id').apply(
+        lambda x: dict(zip(x['answer_concept_id'], x['answer_numeric']))).to_dict()
+
+    mapping_text = survey_data.groupby('question_concept_id').apply(
+        lambda x: dict(zip(x['answer_concept_id'], x['answer_text'].str.strip()))).to_dict()
+
+    input_data['answer_numeric'] = None
+    input_data['answer_text'] = None
+
+    for idx, row in input_data.iterrows():
+        question_id = row['question_concept_id']
+        answer_id = row['answer_concept_id']
+
+        input_data.at[idx, 'answer_numeric'] = mapping_numeric.get(question_id, {}).get(answer_id, None)
+        input_data.at[idx, 'answer_text'] = mapping_text.get(question_id, {}).get(answer_id, None)
+
+        if isinstance(input_data.at[idx, 'answer_text'], (int, float)):
+            input_data.at[idx, 'answer_text'] = str(input_data.at[idx, 'answer_text'])
+        elif isinstance(input_data.at[idx, 'answer_text'], str) and input_data.at[idx, 'answer_text'].isdigit():
+            pass
+
+    return input_data
```

### Comparing `omop2poll-0.1.2/omop2poll/survey.csv` & `omop2poll-0.1.3/omop2poll/survey_healthcare.csv`

 * *Files 14% similar despite different names*

```diff
@@ -1,317 +1,317 @@
-survey,question_concept_id,question,answer_concept_id,answers,answer_numeric,answer_text
-Healthcare Access & Utilization,43528660,Health Advice: Spoken To General Doctor,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43528661,Health Advice: Spoken To Medical Specialist,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43528662,Can't Afford Care: Dental Care,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43528663,Can't Afford Care: Emergency Care,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43528664,Can't Afford Care: Healthcare Provider,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43528665,Can't Afford Care: Bought Rx From Other Country,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43528666,Can't Afford Care: Alternative Therapies,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43529899,Health Provider Race Religion: Delayed Or No Care,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43529901,Health Provider Race Religion: How Important,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43529902,Health Provider Race Religion: How Often,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43529903,Delayed Medical Care: Child Care,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43529904,Delayed Medical Care: Elderly Care,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43529905,Delayed Medical Care: Time Off Work,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43529906,Delayed Medical Care: Transportation,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530268,Delayed Medical Care: Rural Area,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530399,Health Advice: Spoken To Chiropractor,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530400,Health Advice: Spoken To Dentist or Orthodontist,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530401,Health Advice: Spoken To OB/GYN,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530402,Health Advice: Spoken To Mental Health Professional,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530403,Health Advice: Spoken To Eye Doctor,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530404,Health Advice: Spoken To Nurse Practitioner,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530405,"Health Advice: Spoken To Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist",903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530406,Health Advice: Spoken To Podiatrist,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530407,Health Advice: Spoken To Traditional Healer,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530408,Can't Afford Care: Eyeglasses,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530409,Can't Afford Care: Follow-up Care,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530410,Can't Afford Care: Mental Health Counseling,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530411,Can't Afford Care: Prescription Medicines,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530412,Can't Afford Care: Specialist,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530413,Can't Afford Care: Lower Cost Rx To Save Money,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530415,Can't Afford Care: Delayed Filling Rx To Save Money,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530416,Can't Afford Care: Skipped Med To Save Money,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530417,Can't Afford Care: Took Less Med To Save Money,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530418,Insurance: Insurance Accepted,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530437,Health Advice: Asked For Opinion,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530438,Health Advice: Ease of Understanding,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530439,Health Advice: Respected By Provider,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530557,Can't Afford Care: Worried About Paying,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530559,Insurance: Healthcare Coverage,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530562,Health Advice: Place for Health Advice,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530583,Delayed Medical Care: Can't Afford Co-pay,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530584,Delayed Medical Care: Had To Pay Out Of Pocket,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530585,Delayed Medical Care: Deductible Too High,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530593,Health Advice: What Kind Of Place,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530594,Delayed Medical Care: Nervous,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43530595,Health Advice: Spoken To Professional,903087,PMI: Dont Know,-99, Dont Know
-Healthcare Access & Utilization,43528660,Health Advice: Spoken To General Doctor,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43528661,Health Advice: Spoken To Medical Specialist,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43528662,Can't Afford Care: Dental Care,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43528663,Can't Afford Care: Emergency Care,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43528664,Can't Afford Care: Healthcare Provider,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43528665,Can't Afford Care: Bought Rx From Other Country,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43528666,Can't Afford Care: Alternative Therapies,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43529899,Health Provider Race Religion: Delayed Or No Care,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43529901,Health Provider Race Religion: How Important,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43529902,Health Provider Race Religion: How Often,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43529903,Delayed Medical Care: Child Care,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43529904,Delayed Medical Care: Elderly Care,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43529905,Delayed Medical Care: Time Off Work,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43529906,Delayed Medical Care: Transportation,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530268,Delayed Medical Care: Rural Area,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530399,Health Advice: Spoken To Chiropractor,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530400,Health Advice: Spoken To Dentist or Orthodontist,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530401,Health Advice: Spoken To OB/GYN,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530402,Health Advice: Spoken To Mental Health Professional,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530403,Health Advice: Spoken To Eye Doctor,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530404,Health Advice: Spoken To Nurse Practitioner,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530405,"Health Advice: Spoken To Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist",903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530406,Health Advice: Spoken To Podiatrist,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530407,Health Advice: Spoken To Traditional Healer,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530408,Can't Afford Care: Eyeglasses,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530409,Can't Afford Care: Follow-up Care,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530410,Can't Afford Care: Mental Health Counseling,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530411,Can't Afford Care: Prescription Medicines,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530412,Can't Afford Care: Specialist,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530413,Can't Afford Care: Lower Cost Rx To Save Money,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530415,Can't Afford Care: Delayed Filling Rx To Save Money,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530416,Can't Afford Care: Skipped Med To Save Money,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530417,Can't Afford Care: Took Less Med To Save Money,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530418,Insurance: Insurance Accepted,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530437,Health Advice: Asked For Opinion,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530438,Health Advice: Ease of Understanding,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530439,Health Advice: Respected By Provider,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530557,Can't Afford Care: Worried About Paying,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530559,Insurance: Healthcare Coverage,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530562,Health Advice: Place for Health Advice,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530583,Delayed Medical Care: Can't Afford Co-pay,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530584,Delayed Medical Care: Had To Pay Out Of Pocket,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530585,Delayed Medical Care: Deductible Too High,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530593,Health Advice: What Kind Of Place,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530594,Delayed Medical Care: Nervous,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43530595,Health Advice: Spoken To Professional,903096,PMI: Skip,-98, Skip
-Healthcare Access & Utilization,43528660,Health Advice: Spoken To General Doctor,43529549,Spoken To General Doctor: No,0, No
-Healthcare Access & Utilization,43528661,Health Advice: Spoken To Medical Specialist,43529550,Spoken To Medical Specialist: No,0, No
-Healthcare Access & Utilization,43528662,Can't Afford Care: Dental Care,43529335,Can't Afford Dental Care: No,0, No
-Healthcare Access & Utilization,43528663,Can't Afford Care: Emergency Care,43529341,Can't Afford Emergency Care: No,0, No
-Healthcare Access & Utilization,43528664,Can't Afford Care: Healthcare Provider,43529361,Can't Afford Healthcare Provider: No,0, No
-Healthcare Access & Utilization,43528665,Can't Afford Care: Bought Rx From Other Country,43529313,Bought Rx From Other Country: No,0, No
-Healthcare Access & Utilization,43528666,Can't Afford Care: Alternative Therapies,43529300,Alternative Therapies To Save Money: No,0, No
-Healthcare Access & Utilization,43529899,Health Provider Race Religion: Delayed Or No Care,43529576,Health Provider Race Religion Delayed Or No Care: None Of The Time,0, None Of The Time
-Healthcare Access & Utilization,43529901,Health Provider Race Religion: How Important,43529588,Health Provider Race Religion: Not Important,0, Not Important
-Healthcare Access & Utilization,43529902,Health Provider Race Religion: How Often,43529578,Health Provider Race Religion How Often: None Of The Time,0, None Of The Time
-Healthcare Access & Utilization,43529903,Delayed Medical Care: Child Care,43529321,Delayed Care Due to Child Care: No,0, No
-Healthcare Access & Utilization,43529904,Delayed Medical Care: Elderly Care,43529340,Delayed Care Due to Elderly Care: No,0, No
-Healthcare Access & Utilization,43529905,Delayed Medical Care: Time Off Work,43529560,Delayed Care Due to Time Off Work: No,0, No
-Healthcare Access & Utilization,43529906,Delayed Medical Care: Transportation,43529564,Delayed Care Due to Transportation: No,0, No
-Healthcare Access & Utilization,43530268,Delayed Medical Care: Rural Area,43529416,Delayed Care Rural Area: No,0, No
-Healthcare Access & Utilization,43530399,Health Advice: Spoken To Chiropractor,43529546,Spoken To Chiropractor: No,0, No
-Healthcare Access & Utilization,43530400,Health Advice: Spoken To Dentist or Orthodontist,43529547,Spoken To Dentist or Orthodontist: No,0, No
-Healthcare Access & Utilization,43530401,Health Advice: Spoken To OB/GYN,43529553,Spoken To OB/GYN: No,0, No
-Healthcare Access & Utilization,43530402,Health Advice: Spoken To Mental Health Professional,43529551,Spoken To Mental Health Professional: No,0, No
-Healthcare Access & Utilization,43530403,Health Advice: Spoken To Eye Doctor,43529548,Spoken To Eye Doctor: No,0, No
-Healthcare Access & Utilization,43530404,Health Advice: Spoken To Nurse Practitioner,43529552,Spoken To Nurse Practitioner: No,0, No
-Healthcare Access & Utilization,43530405,"Health Advice: Spoken To Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist",43529554,"Spoken To PT, ST, RT, Audiologist or OT: No",0, No
-Healthcare Access & Utilization,43530406,Health Advice: Spoken To Podiatrist,43529555,Spoken To Podiatrist: No,0, No
-Healthcare Access & Utilization,43530407,Health Advice: Spoken To Traditional Healer,43529556,Spoken To Traditional Healer: No,0, No
-Healthcare Access & Utilization,43530408,Can't Afford Care: Eyeglasses,43529348,Can't Afford Eyeglasses: No,0, No
-Healthcare Access & Utilization,43530409,Can't Afford Care: Follow-up Care,43529353,Can't Afford Follow-up Care: No,0, No
-Healthcare Access & Utilization,43530410,Can't Afford Care: Mental Health Counseling,43529389,Can't Afford Mental Health Counseling: No,0, No
-Healthcare Access & Utilization,43530411,Can't Afford Care: Prescription Medicines,43529411,Can't Afford Prescription Medicines: No,0, No
-Healthcare Access & Utilization,43530412,Can't Afford Care: Specialist,43529543,Can't Afford Specialist: No,0, No
-Healthcare Access & Utilization,43530413,Can't Afford Care: Lower Cost Rx To Save Money,43529384,Lower Cost Rx To Save Money: No,0, No
-Healthcare Access & Utilization,43530415,Can't Afford Care: Delayed Filling Rx To Save Money,43529333,Delayed Filling Rx To Save Money: No,0, No
-Healthcare Access & Utilization,43530416,Can't Afford Care: Skipped Med To Save Money,43529539,Skipped Med To Save Money: No,0, No
-Healthcare Access & Utilization,43530417,Can't Afford Care: Took Less Med To Save Money,43529562,Took Less Med To Save Money: No,0, No
-Healthcare Access & Utilization,43530418,Insurance: Insurance Accepted,43529377,Insurance Accepted: No,0, No
-Healthcare Access & Utilization,43530437,Health Advice: Asked For Opinion,43529575,Asked For Opinion: None Of The Time,0, None Of The Time
-Healthcare Access & Utilization,43530438,Health Advice: Ease of Understanding,43529577,Ease of Understanding: None Of The Time,0, None Of The Time
-Healthcare Access & Utilization,43530439,Health Advice: Respected By Provider,43529579,Respected By Provider: None Of The Time,0, None Of The Time
-Healthcare Access & Utilization,43530557,Can't Afford Care: Worried About Paying,43529586,Worried About Paying: Not At All Worried,0, Not At All Worried
-Healthcare Access & Utilization,43530559,Insurance: Healthcare Coverage,43529982,Healthcare Coverage: Worse,0, Worse
-Healthcare Access & Utilization,43530562,Health Advice: Place for Health Advice,43529908,Place for Health Advice: No,0, No
-Healthcare Access & Utilization,43530583,Delayed Medical Care: Can't Afford Co-pay,43529317,Delayed Care Due to Can't Afford Co-pay: No,0, No
-Healthcare Access & Utilization,43530584,Delayed Medical Care: Had To Pay Out Of Pocket,43529359,Delayed Care Due to Had To Pay Out Of Pocket: No,0, No
-Healthcare Access & Utilization,43530585,Delayed Medical Care: Deductible Too High,43529332,Delayed Care Due to Deductible Too High: No,0, No
-Healthcare Access & Utilization,43530594,Delayed Medical Care: Nervous,43529396,Delayed Care Nervous: No,0, No
-Healthcare Access & Utilization,43530595,Health Advice: Spoken To Professional,43529282,Spoken To Professional: Never,0, Never
-Healthcare Access & Utilization,43528660,Health Advice: Spoken To General Doctor,43530243,Spoken To General Doctor: Yes,1, Yes
-Healthcare Access & Utilization,43528661,Health Advice: Spoken To Medical Specialist,43530244,Spoken To Medical Specialist: Yes,1, Yes
-Healthcare Access & Utilization,43528662,Can't Afford Care: Dental Care,43530028,Can't Afford Dental Care: Yes,1, Yes
-Healthcare Access & Utilization,43528663,Can't Afford Care: Emergency Care,43530034,Can't Afford Emergency Care: Yes,1, Yes
-Healthcare Access & Utilization,43528664,Can't Afford Care: Healthcare Provider,43530054,Can't Afford Healthcare Provider: Yes,1, Yes
-Healthcare Access & Utilization,43528665,Can't Afford Care: Bought Rx From Other Country,43530007,Bought Rx From Other Country: Yes,1, Yes
-Healthcare Access & Utilization,43528666,Can't Afford Care: Alternative Therapies,43529994,Alternative Therapies To Save Money: Yes,1, Yes
-Healthcare Access & Utilization,43529899,Health Provider Race Religion: Delayed Or No Care,43529844,Health Provider Race Religion Delayed Or No Care: Some Of The Time,1, Some Of The Time
-Healthcare Access & Utilization,43529901,Health Provider Race Religion: How Important,43529840,Health Provider Race Religion: Slightly Important,1, Slightly Important
-Healthcare Access & Utilization,43529902,Health Provider Race Religion: How Often,43529846,Health Provider Race Religion How Often: Some Of The Time,1, Some Of The Time
-Healthcare Access & Utilization,43529903,Delayed Medical Care: Child Care,43530014,Delayed Care Due to Child Care: Yes,1, Yes
-Healthcare Access & Utilization,43529904,Delayed Medical Care: Elderly Care,43530033,Delayed Care Due to Elderly Care: Yes,1, Yes
-Healthcare Access & Utilization,43529905,Delayed Medical Care: Time Off Work,43530254,Delayed Care Due to Time Off Work: Yes,1, Yes
-Healthcare Access & Utilization,43529906,Delayed Medical Care: Transportation,43530258,Delayed Care Due to Transportation: Yes,1, Yes
-Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",43528263,"Nurse Practitioner, PA, or Midwife Visits: 1",1,1
-Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,43528258,Dentist or Orthodontist Visits: 1,1,1
-Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,43528264,OB/GYN Visits: 1,1,1
-Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,43528261,Medical Specialist Visits: 1,1,1
-Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,43528262,Mental Health Professional Visits: 1,1,1
-Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,43528267,Traditional Healer Visits: 1,1,1
-Healthcare Access & Utilization,43530268,Delayed Medical Care: Rural Area,43530110,Delayed Care Rural Area: Yes,1, Yes
-Healthcare Access & Utilization,43530399,Health Advice: Spoken To Chiropractor,43530240,Spoken To Chiropractor: Yes,1, Yes
-Healthcare Access & Utilization,43530400,Health Advice: Spoken To Dentist or Orthodontist,43530241,Spoken To Dentist or Orthodontist: Yes,1, Yes
-Healthcare Access & Utilization,43530401,Health Advice: Spoken To OB/GYN,43530247,Spoken To OB/GYN: Yes,1, Yes
-Healthcare Access & Utilization,43530402,Health Advice: Spoken To Mental Health Professional,43530245,Spoken To Mental Health Professional: Yes,1, Yes
-Healthcare Access & Utilization,43530403,Health Advice: Spoken To Eye Doctor,43530242,Spoken To Eye Doctor: Yes,1, Yes
-Healthcare Access & Utilization,43530404,Health Advice: Spoken To Nurse Practitioner,43530246,Spoken To Nurse Practitioner: Yes,1, Yes
-Healthcare Access & Utilization,43530405,"Health Advice: Spoken To Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist",43530248,"Spoken To PT, ST, RT, Audiologist or OT: Yes",1, Yes
-Healthcare Access & Utilization,43530406,Health Advice: Spoken To Podiatrist,43530249,Spoken To Podiatrist: Yes,1, Yes
-Healthcare Access & Utilization,43530407,Health Advice: Spoken To Traditional Healer,43530250,Spoken To Traditional Healer: Yes,1, Yes
-Healthcare Access & Utilization,43530408,Can't Afford Care: Eyeglasses,43530041,Can't Afford Eyeglasses: Yes,1, Yes
-Healthcare Access & Utilization,43530409,Can't Afford Care: Follow-up Care,43530046,Can't Afford Follow-up Care: Yes,1, Yes
-Healthcare Access & Utilization,43530410,Can't Afford Care: Mental Health Counseling,43530082,Can't Afford Mental Health Counseling: Yes,1, Yes
-Healthcare Access & Utilization,43530411,Can't Afford Care: Prescription Medicines,43530105,Can't Afford Prescription Medicines: Yes,1, Yes
-Healthcare Access & Utilization,43530412,Can't Afford Care: Specialist,43530237,Can't Afford Specialist: Yes,1, Yes
-Healthcare Access & Utilization,43530413,Can't Afford Care: Lower Cost Rx To Save Money,43530077,Lower Cost Rx To Save Money: Yes,1, Yes
-Healthcare Access & Utilization,43530415,Can't Afford Care: Delayed Filling Rx To Save Money,43530026,Delayed Filling Rx To Save Money: Yes,1, Yes
-Healthcare Access & Utilization,43530416,Can't Afford Care: Skipped Med To Save Money,43530233,Skipped Med To Save Money: Yes,1, Yes
-Healthcare Access & Utilization,43530417,Can't Afford Care: Took Less Med To Save Money,43530256,Took Less Med To Save Money: Yes,1, Yes
-Healthcare Access & Utilization,43530418,Insurance: Insurance Accepted,43530070,Insurance Accepted: Yes,1, Yes
-Healthcare Access & Utilization,43530437,Health Advice: Asked For Opinion,43529843,Asked For Opinion: Some Of The Time,1, Some Of The Time
-Healthcare Access & Utilization,43530438,Health Advice: Ease of Understanding,43529845,Ease of Understanding: Some Of The Time,1, Some Of The Time
-Healthcare Access & Utilization,43530439,Health Advice: Respected By Provider,43529847,Respected By Provider: Some Of The Time,1, Some Of The Time
-Healthcare Access & Utilization,43530557,Can't Afford Care: Worried About Paying,43529850,Worried About Paying: Somewhat Worried,1, Somewhat Worried
-Healthcare Access & Utilization,43530559,Insurance: Healthcare Coverage,43528346,Healthcare Coverage: About The Same,1, About The Same
-Healthcare Access & Utilization,43530562,Health Advice: Place for Health Advice,43530103,Place for Health Advice: Yes,1, Yes
-Healthcare Access & Utilization,43530583,Delayed Medical Care: Can't Afford Co-pay,43530010,Delayed Care Due to Can't Afford Co-pay: Yes,1, Yes
-Healthcare Access & Utilization,43530584,Delayed Medical Care: Had To Pay Out Of Pocket,43530052,Delayed Care Due to Had To Pay Out Of Pocket: Yes,1, Yes
-Healthcare Access & Utilization,43530585,Delayed Medical Care: Deductible Too High,43530025,Delayed Care Due to Deductible Too High: Yes,1, Yes
-Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,43528260,General Doctor Visits: 1,1,1
-Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,43528257,Chiropractor Visits: 1,1,1
-Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,43528266,Podiatrist Visits: 1,1,1
-Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,43528259,Eye Doctor Visits: 1,1,1
-Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",43528265,"PT, ST, RT, Audiologist or OT Visits: 1",1,1
-Healthcare Access & Utilization,43530593,Health Advice: What Kind Of Place,43528645,What Kind Of Place: Doctors Office,1, Doctors Office
-Healthcare Access & Utilization,43530594,Delayed Medical Care: Nervous,43530089,Delayed Care Nervous: Yes,1, Yes
-Healthcare Access & Utilization,43530595,Health Advice: Spoken To Professional,43528334,Spoken To Professional: 6mo Or Less,1, 6mo Or Less
-Healthcare Access & Utilization,43529899,Health Provider Race Religion: Delayed Or No Care,43529239,Health Provider Race Religion Delayed Or No Care: Most Of The Time,2, Most Of The Time
-Healthcare Access & Utilization,43529901,Health Provider Race Religion: How Important,43529849,Health Provider Race Religion: Somewhat Important,2, Somewhat Important
-Healthcare Access & Utilization,43529902,Health Provider Race Religion: How Often,43529241,Health Provider Race Religion How Often: Most Of The Time,2, Most Of The Time
-Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",43528307,"Nurse Practitioner, PA, or Midwife Visits: 2 to 3",2, 2 to 3
-Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,43528302,Dentist or Orthodontist Visits: 2 to 3,2, 2 to 3
-Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,43528308,OB/GYN Visits: 2 to 3,2, 2 to 3
-Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,43528305,Medical Specialist Visits: 2 to 3,2, 2 to 3
-Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,43528306,Mental Health Professional Visits: 2 to 3,2, 2 to 3
-Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,43528311,Traditional Healer Visits: 2 to 3,2, 2 to 3
-Healthcare Access & Utilization,43530437,Health Advice: Asked For Opinion,43529238,Asked For Opinion: Most Of The Time,2, Most Of The Time
-Healthcare Access & Utilization,43530438,Health Advice: Ease of Understanding,43529240,Ease of Understanding: Most Of The Time,2, Most Of The Time
-Healthcare Access & Utilization,43530439,Health Advice: Respected By Provider,43529242,Respected By Provider: Most Of The Time,2, Most Of The Time
-Healthcare Access & Utilization,43530557,Can't Afford Care: Worried About Paying,43529954,Worried About Paying: Very Worried,2, Very Worried
-Healthcare Access & Utilization,43530559,Insurance: Healthcare Coverage,43528458,Healthcare Coverage: Better,2, Better
-Healthcare Access & Utilization,43530562,Health Advice: Place for Health Advice,43529907,Place for Health Advice: More Than One,2, More Than One
-Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,43528304,General Doctor Visits: 2 to 3,2, 2 to 3
-Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,43528301,Chiropractor Visits: 2 to 3,2, 2 to 3
-Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,43528310,Podiatrist Visits: 2 to 3,2, 2 to 3
-Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,43528303,Eye Doctor Visits: 2 to 3,2, 2 to 3
-Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",43528309,"PT, ST, RT, Audiologist or OT: 2 to 3",2, 2 to 3
-Healthcare Access & Utilization,43530593,Health Advice: What Kind Of Place,43528646,What Kind Of Place: No One Place Most Often,2, No One Place Most Often
-Healthcare Access & Utilization,43530595,Health Advice: Spoken To Professional,43529237,Spoken To Professional: 6 Mo To 1 Year Ago,2, 6 Mo To 1 Year Ago
-Healthcare Access & Utilization,43529899,Health Provider Race Religion: Delayed Or No Care,43528387,Health Provider Race Religion Delayed Or No Care: Always,3, Always
-Healthcare Access & Utilization,43529901,Health Provider Race Religion: How Important,43529953,Health Provider Race Religion: Very Important,3, Very Important
-Healthcare Access & Utilization,43529902,Health Provider Race Religion: How Often,43528389,Health Provider Race Religion How Often: Always,3, Always
-Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",43528318,"Nurse Practitioner, PA, or Midwife Visits: 4 to 5",3, 4 to 5
-Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,43528313,Dentist or Orthodontist Visits: 4 to 5,3, 4 to 5
-Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,43528319,OB/GYN Visits: 4 to 5,3, 4 to 5
-Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,43528316,Medical Specialist Visits: 4 to 5,3, 4 to 5
-Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,43528317,Mental Health Professional Visits: 4 to 5,3, 4 to 5
-Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,43528322,Traditional Healer Visits: 4 to 5,3, 4 to 5
-Healthcare Access & Utilization,43530437,Health Advice: Asked For Opinion,43528386,Asked For Opinion: Always,3, Always
-Healthcare Access & Utilization,43530438,Health Advice: Ease of Understanding,43528388,Ease of Understanding: Always,3, Always
-Healthcare Access & Utilization,43530439,Health Advice: Respected By Provider,43528390,Respected By Provider: Always,3, Always
-Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,43528315,General Doctor Visits: 4 to 5,3, 4 to 5
-Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,43528312,Chiropractor Visits: 4 to 5,3, 4 to 5
-Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,43528321,Podiatrist Visits: 4 to 5,3, 4 to 5
-Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,43528314,Eye Doctor Visits: 4 to 5,3, 4 to 5
-Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",43528320,"PT, ST, RT, Audiologist or OT Visits: 4 to 5",3, 4 to 5
-Healthcare Access & Utilization,43530593,Health Advice: What Kind Of Place,43528803,What Kind Of Place: Emergency Room,3, Emergency Room
-Healthcare Access & Utilization,43530595,Health Advice: Spoken To Professional,43530564,Spoken To Professional: 1 To 2 Years Ago,3, 1 To 2 Years Ago
-Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",43528329,"Nurse Practitioner, PA, or Midwife Visits: 6 to 7",4, 6 to 7
-Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,43528324,Dentist or Orthodontist Visits: 6 to 7,4, 6 to 7
-Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,43528330,OB/GYN Visits: 6 to 7,4, 6 to 7
-Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,43528327,Medical Specialist Visits: 6 to 7,4, 6 to 7
-Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,43528328,Mental Health Professional Visits: 6 to 7,4, 6 to 7
-Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,43528333,Traditional Healer Visits: 6 to 7,4, 6 to 7
-Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,43528326,General Doctor Visits: 6 to 7,4, 6 to 7
-Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,43528323,Chiropractor Visits: 6 to 7,4, 6 to 7
-Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,43528332,Podiatrist Visits: 6 to 7,4, 6 to 7
-Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,43528325,Eye Doctor Visits: 6 to 7,4, 6 to 7
-Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",43528331,"PT, ST, RT, Audiologist or OT Visits: 6 to 7",4, 6 to 7
-Healthcare Access & Utilization,43530593,Health Advice: What Kind Of Place,43529848,What Kind Of Place: Some Other Place,4, Some Other Place
-Healthcare Access & Utilization,43530595,Health Advice: Spoken To Professional,43530565,Spoken To Professional: 2 To 5 Years Ago,4, 2 To 5 Years Ago
-Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",43528341,"Nurse Practitioner, PA, or Midwife Visits: 8 to 9",5, 8 to 9
-Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,43528336,Dentist or Orthodontist Visits: 8 to 9,5, 8 to 9
-Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,43528342,OB/GYN Visits: 8 to 9,5, 8 to 9
-Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,43528339,Medical Specialist Visits: 8 to 9,5, 8 to 9
-Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,43528340,Mental Health Professional Visits: 8 to 9,5, 8 to 9
-Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,43528345,Traditional Healer Visits: 8 to 9,5, 8 to 9
-Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,43528338,General Doctor Visits: 8 to 9,5, 8 to 9
-Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,43528335,Chiropractor Visits: 8 to 9,5, 8 to 9
-Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,43528344,Podiatrist Visits: 8 to 9,5, 8 to 9
-Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,43528337,Eye Doctor Visits: 8 to 9,5, 8 to 9
-Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",43528343,"PT, ST, RT, Audiologist or OT Visits: 8 to 9",5, 8 to 9
-Healthcare Access & Utilization,43530593,Health Advice: What Kind Of Place,43529948,What Kind Of Place: Urgent Care,5, Urgent Care
-Healthcare Access & Utilization,43530595,Health Advice: Spoken To Professional,43530566,Spoken To Professional: More Than 5 Years Ago,5, More Than 5 Years Ago
-Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",43528274,"Nurse Practitioner, PA, or Midwife Visits: 10 to 12",6, 10 to 12
-Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,43528269,Dentist or Orthodontist Visits: 10 to 12,6, 10 to 12
-Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,43528275,OB/GYN Visits: 10 to 12,6, 10 to 12
-Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,43528272,Medical Specialist Visits: 10 to 12,6, 10 to 12
-Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,43528273,Mental Health Professional Visits: 10 to 12,6, 10 to 12
-Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,43528278,Traditional Healer Visits: 10 to 12,6, 10 to 12
-Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,43528271,General Doctor Visits: 10 to 12,6, 10 to 12
-Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,43528268,Chiropractor Visits: 10 to 12,6, 10 to 12
-Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,43528277,Podiatrist Visits: 10 to 12,6, 10 to 12
-Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,43528270,Eye Doctor Visits: 10 to 12,6, 10 to 12
-Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",43528276,"PT, ST, RT, Audiologist or OT Visits: 10 to 12",6, 10 to 12
-Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",43528285,"Nurse Practitioner, PA, or Midwife Visits: 13 to 15",7, 13 to 15
-Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,43528280,Dentist or Orthodontist Visits: 13 to 15,7, 13 to 15
-Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,43528286,OB/GYN Visits: 13 to 15,7, 13 to 15
-Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,43528283,Medical Specialist Visits: 13 to 15,7, 13 to 15
-Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,43528284,Mental Health Professional Visits: 13 to 15,7, 13 to 15
-Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,43528289,Traditional Healer Visits: 13 to 15,7, 13 to 15
-Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,43528282,General Doctor Visits: 13 to 15,7, 13 to 15
-Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,43528279,Chiropractor Visits: 13 to 15,7, 13 to 15
-Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,43528288,Podiatrist Visits: 13 to 15,7, 13 to 15
-Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,43528281,Eye Doctor Visits: 13 to 15,7, 13 to 15
-Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",43528287,"PT, ST, RT, Audiologist or OT Visits: 13 to 15",7, 13 to 15
-Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",43528296,"Nurse Practitioner, PA, or Midwife Visits: 16 or More",8, 16 or More
-Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,43528291,Dentist or Orthodontist Visits: 16 or More,8, 16 or More
-Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,43528297,OB/GYN Visits: 16 or More,8, 16 or More
-Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,43528294,Medical Specialist Visits: 16 or More,8, 16 or More
-Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,43528295,Mental Health Professional Visits: 16 or More,8, 16 or More
-Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,43528300,Traditional Healer Visits: 16 or More,8, 16 or More
-Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,43528293,General Doctor Visits: 16 or M ore,8, 16 or M ore
-Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,43528290,Chiropractor Visits: 16 or M ore,8, 16 or M ore
-Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,43528299,Podiatrist Visits: 16 or More,8, 16 or More
-Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,43528292,Eye Doctor Visits: 16 or More,8, 16 or More
-Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",43528298,"PT, ST, RT, Audiologist or OT Visits: 16 or More",8, 16 or More
+﻿survey,question_concept_id,question,answer_concept_id,answer,answer_numeric,answer_text
+Healthcare Access & Utilization,43528660,Health Advice: Spoken To General Doctor,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43528660,Health Advice: Spoken To General Doctor,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43528660,Health Advice: Spoken To General Doctor,43529549,Spoken To General Doctor: No,2, No
+Healthcare Access & Utilization,43528660,Health Advice: Spoken To General Doctor,43530243,Spoken To General Doctor: Yes,1, Yes
+Healthcare Access & Utilization,43528661,Health Advice: Spoken To Medical Specialist,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43528661,Health Advice: Spoken To Medical Specialist,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43528661,Health Advice: Spoken To Medical Specialist,43529550,Spoken To Medical Specialist: No,2, No
+Healthcare Access & Utilization,43528661,Health Advice: Spoken To Medical Specialist,43530244,Spoken To Medical Specialist: Yes,1, Yes
+Healthcare Access & Utilization,43528662,Can't Afford Care: Dental Care,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43528662,Can't Afford Care: Dental Care,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43528662,Can't Afford Care: Dental Care,43529335,Can't Afford Dental Care: No,2, No
+Healthcare Access & Utilization,43528662,Can't Afford Care: Dental Care,43530028,Can't Afford Dental Care: Yes,1, Yes
+Healthcare Access & Utilization,43528663,Can't Afford Care: Emergency Care,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43528663,Can't Afford Care: Emergency Care,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43528663,Can't Afford Care: Emergency Care,43529341,Can't Afford Emergency Care: No,2, No
+Healthcare Access & Utilization,43528663,Can't Afford Care: Emergency Care,43530034,Can't Afford Emergency Care: Yes,1, Yes
+Healthcare Access & Utilization,43528664,Can't Afford Care: Healthcare Provider,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43528664,Can't Afford Care: Healthcare Provider,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43528664,Can't Afford Care: Healthcare Provider,43529361,Can't Afford Healthcare Provider: No,0, No
+Healthcare Access & Utilization,43528664,Can't Afford Care: Healthcare Provider,43530054,Can't Afford Healthcare Provider: Yes,1, Yes
+Healthcare Access & Utilization,43528665,Can't Afford Care: Bought Rx From Other Country,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43528665,Can't Afford Care: Bought Rx From Other Country,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43528665,Can't Afford Care: Bought Rx From Other Country,43529313,Bought Rx From Other Country: No,2, No
+Healthcare Access & Utilization,43528665,Can't Afford Care: Bought Rx From Other Country,43530007,Bought Rx From Other Country: Yes,1, Yes
+Healthcare Access & Utilization,43528666,Can't Afford Care: Alternative Therapies,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43528666,Can't Afford Care: Alternative Therapies,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43528666,Can't Afford Care: Alternative Therapies,43529300,Alternative Therapies To Save Money: No,2, No
+Healthcare Access & Utilization,43528666,Can't Afford Care: Alternative Therapies,43529994,Alternative Therapies To Save Money: Yes,1, Yes
+Healthcare Access & Utilization,43529899,Health Provider Race Religion: Delayed Or No Care,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43529899,Health Provider Race Religion: Delayed Or No Care,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43529899,Health Provider Race Religion: Delayed Or No Care,43529576,Health Provider Race Religion Delayed Or No Care: None Of The Time,1, None Of The Time
+Healthcare Access & Utilization,43529899,Health Provider Race Religion: Delayed Or No Care,43529844,Health Provider Race Religion Delayed Or No Care: Some Of The Time,2, Some Of The Time
+Healthcare Access & Utilization,43529899,Health Provider Race Religion: Delayed Or No Care,43529239,Health Provider Race Religion Delayed Or No Care: Most Of The Time,3, Most Of The Time
+Healthcare Access & Utilization,43529899,Health Provider Race Religion: Delayed Or No Care,43528387,Health Provider Race Religion Delayed Or No Care: Always,4, Always
+Healthcare Access & Utilization,43529901,Health Provider Race Religion: How Important,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43529901,Health Provider Race Religion: How Important,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43529901,Health Provider Race Religion: How Important,43529588,Health Provider Race Religion: Not Important,1, Not Important
+Healthcare Access & Utilization,43529901,Health Provider Race Religion: How Important,43529840,Health Provider Race Religion: Slightly Important,2, Slightly Important
+Healthcare Access & Utilization,43529901,Health Provider Race Religion: How Important,43529849,Health Provider Race Religion: Somewhat Important,3, Somewhat Important
+Healthcare Access & Utilization,43529901,Health Provider Race Religion: How Important,43529953,Health Provider Race Religion: Very Important,4, Very Important
+Healthcare Access & Utilization,43529902,Health Provider Race Religion: How Often,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43529902,Health Provider Race Religion: How Often,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43529902,Health Provider Race Religion: How Often,43529578,Health Provider Race Religion How Often: None Of The Time,1, None Of The Time
+Healthcare Access & Utilization,43529902,Health Provider Race Religion: How Often,43529846,Health Provider Race Religion How Often: Some Of The Time,2, Some Of The Time
+Healthcare Access & Utilization,43529902,Health Provider Race Religion: How Often,43529241,Health Provider Race Religion How Often: Most Of The Time,3, Most Of The Time
+Healthcare Access & Utilization,43529902,Health Provider Race Religion: How Often,43528389,Health Provider Race Religion How Often: Always,4, Always
+Healthcare Access & Utilization,43529903,Delayed Medical Care: Child Care,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43529903,Delayed Medical Care: Child Care,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43529903,Delayed Medical Care: Child Care,43529321,Delayed Care Due to Child Care: No,2, No
+Healthcare Access & Utilization,43529903,Delayed Medical Care: Child Care,43530014,Delayed Care Due to Child Care: Yes,1, Yes
+Healthcare Access & Utilization,43529904,Delayed Medical Care: Elderly Care,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43529904,Delayed Medical Care: Elderly Care,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43529904,Delayed Medical Care: Elderly Care,43529340,Delayed Care Due to Elderly Care: No,2, No
+Healthcare Access & Utilization,43529904,Delayed Medical Care: Elderly Care,43530033,Delayed Care Due to Elderly Care: Yes,1, Yes
+Healthcare Access & Utilization,43529905,Delayed Medical Care: Time Off Work,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43529905,Delayed Medical Care: Time Off Work,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43529905,Delayed Medical Care: Time Off Work,43529560,Delayed Care Due to Time Off Work: No,2, No
+Healthcare Access & Utilization,43529905,Delayed Medical Care: Time Off Work,43530254,Delayed Care Due to Time Off Work: Yes,1, Yes
+Healthcare Access & Utilization,43529906,Delayed Medical Care: Transportation,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43529906,Delayed Medical Care: Transportation,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43529906,Delayed Medical Care: Transportation,43529564,Delayed Care Due to Transportation: No,2, No
+Healthcare Access & Utilization,43529906,Delayed Medical Care: Transportation,43530258,Delayed Care Due to Transportation: Yes,1, Yes
+Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",43528263,"Nurse Practitioner, PA, or Midwife Visits: 1",1,1
+Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",43528307,"Nurse Practitioner, PA, or Midwife Visits: 2 to 3",2, 2 to 3
+Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",43528318,"Nurse Practitioner, PA, or Midwife Visits: 4 to 5",3, 4 to 5
+Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",43528329,"Nurse Practitioner, PA, or Midwife Visits: 6 to 7",4, 6 to 7
+Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",43528341,"Nurse Practitioner, PA, or Midwife Visits: 8 to 9",5, 8 to 9
+Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",43528274,"Nurse Practitioner, PA, or Midwife Visits: 10 to 12",6, 10 to 12
+Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",43528285,"Nurse Practitioner, PA, or Midwife Visits: 13 to 15",7, 13 to 15
+Healthcare Access & Utilization,43529973,"Health Advice: Nurse Practitioner, Physician Assistant, or Midwife Visits",43528296,"Nurse Practitioner, PA, or Midwife Visits: 16 or More",8, 16 or More
+Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,43528258,Dentist or Orthodontist Visits: 1,1,1
+Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,43528302,Dentist or Orthodontist Visits: 2 to 3,2, 2 to 3
+Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,43528313,Dentist or Orthodontist Visits: 4 to 5,3, 4 to 5
+Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,43528324,Dentist or Orthodontist Visits: 6 to 7,4, 6 to 7
+Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,43528336,Dentist or Orthodontist Visits: 8 to 9,5, 8 to 9
+Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,43528269,Dentist or Orthodontist Visits: 10 to 12,6, 10 to 12
+Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,43528280,Dentist or Orthodontist Visits: 13 to 15,7, 13 to 15
+Healthcare Access & Utilization,43529974,Health Advice: Dentist or Orthodontist Visits,43528291,Dentist or Orthodontist Visits: 16 or More,8, 16 or More
+Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,43528264,OB/GYN Visits: 1,1,1
+Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,43528308,OB/GYN Visits: 2 to 3,2, 2 to 3
+Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,43528319,OB/GYN Visits: 4 to 5,3, 4 to 5
+Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,43528330,OB/GYN Visits: 6 to 7,4, 6 to 7
+Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,43528342,OB/GYN Visits: 8 to 9,5, 8 to 9
+Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,43528275,OB/GYN Visits: 10 to 12,6, 10 to 12
+Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,43528286,OB/GYN Visits: 13 to 15,7, 13 to 15
+Healthcare Access & Utilization,43529975,Health Advice: OB/GYN Visits,43528297,OB/GYN Visits: 16 or More,8, 16 or More
+Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,43528261,Medical Specialist Visits: 1,1,1
+Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,43528305,Medical Specialist Visits: 2 to 3,2, 2 to 3
+Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,43528316,Medical Specialist Visits: 4 to 5,3, 4 to 5
+Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,43528327,Medical Specialist Visits: 6 to 7,4, 6 to 7
+Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,43528339,Medical Specialist Visits: 8 to 9,5, 8 to 9
+Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,43528272,Medical Specialist Visits: 10 to 12,6, 10 to 12
+Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,43528283,Medical Specialist Visits: 13 to 15,7, 13 to 15
+Healthcare Access & Utilization,43529976,Health Advice: Medical Specialist Visits,43528294,Medical Specialist Visits: 16 or More,8, 16 or More
+Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,43528262,Mental Health Professional Visits: 1,1,1
+Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,43528306,Mental Health Professional Visits: 2 to 3,2, 2 to 3
+Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,43528317,Mental Health Professional Visits: 4 to 5,3, 4 to 5
+Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,43528328,Mental Health Professional Visits: 6 to 7,4, 6 to 7
+Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,43528340,Mental Health Professional Visits: 8 to 9,5, 8 to 9
+Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,43528273,Mental Health Professional Visits: 10 to 12,6, 10 to 12
+Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,43528284,Mental Health Professional Visits: 13 to 15,7, 13 to 15
+Healthcare Access & Utilization,43529977,Health Advice: Mental Health Professional Visits,43528295,Mental Health Professional Visits: 16 or More,8, 16 or More
+Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,43528267,Traditional Healer Visits: 1,1,1
+Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,43528311,Traditional Healer Visits: 2 to 3,2, 2 to 3
+Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,43528322,Traditional Healer Visits: 4 to 5,3, 4 to 5
+Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,43528333,Traditional Healer Visits: 6 to 7,4, 6 to 7
+Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,43528345,Traditional Healer Visits: 8 to 9,5, 8 to 9
+Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,43528278,Traditional Healer Visits: 10 to 12,6, 10 to 12
+Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,43528289,Traditional Healer Visits: 13 to 15,7, 13 to 15
+Healthcare Access & Utilization,43529978,Health Advice: Traditional Healer Visits,43528300,Traditional Healer Visits: 16 or More,8, 16 or More
+Healthcare Access & Utilization,43530268,Delayed Medical Care: Rural Area,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530268,Delayed Medical Care: Rural Area,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530268,Delayed Medical Care: Rural Area,43529416,Delayed Care Rural Area: No,2, No
+Healthcare Access & Utilization,43530268,Delayed Medical Care: Rural Area,43530110,Delayed Care Rural Area: Yes,1, Yes
+Healthcare Access & Utilization,43530399,Health Advice: Spoken To Chiropractor,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530399,Health Advice: Spoken To Chiropractor,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530399,Health Advice: Spoken To Chiropractor,43529546,Spoken To Chiropractor: No,2, No
+Healthcare Access & Utilization,43530399,Health Advice: Spoken To Chiropractor,43530240,Spoken To Chiropractor: Yes,1, Yes
+Healthcare Access & Utilization,43530400,Health Advice: Spoken To Dentist or Orthodontist,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530400,Health Advice: Spoken To Dentist or Orthodontist,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530400,Health Advice: Spoken To Dentist or Orthodontist,43529547,Spoken To Dentist or Orthodontist: No,2, No
+Healthcare Access & Utilization,43530400,Health Advice: Spoken To Dentist or Orthodontist,43530241,Spoken To Dentist or Orthodontist: Yes,1, Yes
+Healthcare Access & Utilization,43530401,Health Advice: Spoken To OB/GYN,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530401,Health Advice: Spoken To OB/GYN,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530401,Health Advice: Spoken To OB/GYN,43529553,Spoken To OB/GYN: No,2, No
+Healthcare Access & Utilization,43530401,Health Advice: Spoken To OB/GYN,43530247,Spoken To OB/GYN: Yes,1, Yes
+Healthcare Access & Utilization,43530402,Health Advice: Spoken To Mental Health Professional,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530402,Health Advice: Spoken To Mental Health Professional,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530402,Health Advice: Spoken To Mental Health Professional,43529551,Spoken To Mental Health Professional: No,2, No
+Healthcare Access & Utilization,43530402,Health Advice: Spoken To Mental Health Professional,43530245,Spoken To Mental Health Professional: Yes,1, Yes
+Healthcare Access & Utilization,43530403,Health Advice: Spoken To Eye Doctor,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530403,Health Advice: Spoken To Eye Doctor,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530403,Health Advice: Spoken To Eye Doctor,43529548,Spoken To Eye Doctor: No,2, No
+Healthcare Access & Utilization,43530403,Health Advice: Spoken To Eye Doctor,43530242,Spoken To Eye Doctor: Yes,1, Yes
+Healthcare Access & Utilization,43530404,Health Advice: Spoken To Nurse Practitioner,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530404,Health Advice: Spoken To Nurse Practitioner,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530404,Health Advice: Spoken To Nurse Practitioner,43529552,Spoken To Nurse Practitioner: No,2, No
+Healthcare Access & Utilization,43530404,Health Advice: Spoken To Nurse Practitioner,43530246,Spoken To Nurse Practitioner: Yes,1, Yes
+Healthcare Access & Utilization,43530405,"Health Advice: Spoken To Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist",903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530405,"Health Advice: Spoken To Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist",903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530405,"Health Advice: Spoken To Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist",43529554,"Spoken To PT, ST, RT, Audiologist or OT: No",2, No
+Healthcare Access & Utilization,43530405,"Health Advice: Spoken To Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist",43530248,"Spoken To PT, ST, RT, Audiologist or OT: Yes",1, Yes
+Healthcare Access & Utilization,43530406,Health Advice: Spoken To Podiatrist,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530406,Health Advice: Spoken To Podiatrist,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530406,Health Advice: Spoken To Podiatrist,43529555,Spoken To Podiatrist: No,2, No
+Healthcare Access & Utilization,43530406,Health Advice: Spoken To Podiatrist,43530249,Spoken To Podiatrist: Yes,1, Yes
+Healthcare Access & Utilization,43530407,Health Advice: Spoken To Traditional Healer,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530407,Health Advice: Spoken To Traditional Healer,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530407,Health Advice: Spoken To Traditional Healer,43529556,Spoken To Traditional Healer: No,2, No
+Healthcare Access & Utilization,43530407,Health Advice: Spoken To Traditional Healer,43530250,Spoken To Traditional Healer: Yes,1, Yes
+Healthcare Access & Utilization,43530408,Can't Afford Care: Eyeglasses,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530408,Can't Afford Care: Eyeglasses,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530408,Can't Afford Care: Eyeglasses,43529348,Can't Afford Eyeglasses: No,2, No
+Healthcare Access & Utilization,43530408,Can't Afford Care: Eyeglasses,43530041,Can't Afford Eyeglasses: Yes,1, Yes
+Healthcare Access & Utilization,43530409,Can't Afford Care: Follow-up Care,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530409,Can't Afford Care: Follow-up Care,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530409,Can't Afford Care: Follow-up Care,43529353,Can't Afford Follow-up Care: No,2, No
+Healthcare Access & Utilization,43530409,Can't Afford Care: Follow-up Care,43530046,Can't Afford Follow-up Care: Yes,1, Yes
+Healthcare Access & Utilization,43530410,Can't Afford Care: Mental Health Counseling,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530410,Can't Afford Care: Mental Health Counseling,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530410,Can't Afford Care: Mental Health Counseling,43529389,Can't Afford Mental Health Counseling: No,2, No
+Healthcare Access & Utilization,43530410,Can't Afford Care: Mental Health Counseling,43530082,Can't Afford Mental Health Counseling: Yes,1, Yes
+Healthcare Access & Utilization,43530411,Can't Afford Care: Prescription Medicines,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530411,Can't Afford Care: Prescription Medicines,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530411,Can't Afford Care: Prescription Medicines,43529411,Can't Afford Prescription Medicines: No,2, No
+Healthcare Access & Utilization,43530411,Can't Afford Care: Prescription Medicines,43530105,Can't Afford Prescription Medicines: Yes,1, Yes
+Healthcare Access & Utilization,43530412,Can't Afford Care: Specialist,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530412,Can't Afford Care: Specialist,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530412,Can't Afford Care: Specialist,43529543,Can't Afford Specialist: No,2, No
+Healthcare Access & Utilization,43530412,Can't Afford Care: Specialist,43530237,Can't Afford Specialist: Yes,1, Yes
+Healthcare Access & Utilization,43530413,Can't Afford Care: Lower Cost Rx To Save Money,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530413,Can't Afford Care: Lower Cost Rx To Save Money,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530413,Can't Afford Care: Lower Cost Rx To Save Money,43529384,Lower Cost Rx To Save Money: No,2, No
+Healthcare Access & Utilization,43530413,Can't Afford Care: Lower Cost Rx To Save Money,43530077,Lower Cost Rx To Save Money: Yes,1, Yes
+Healthcare Access & Utilization,43530415,Can't Afford Care: Delayed Filling Rx To Save Money,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530415,Can't Afford Care: Delayed Filling Rx To Save Money,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530415,Can't Afford Care: Delayed Filling Rx To Save Money,43529333,Delayed Filling Rx To Save Money: No,2, No
+Healthcare Access & Utilization,43530415,Can't Afford Care: Delayed Filling Rx To Save Money,43530026,Delayed Filling Rx To Save Money: Yes,1, Yes
+Healthcare Access & Utilization,43530416,Can't Afford Care: Skipped Med To Save Money,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530416,Can't Afford Care: Skipped Med To Save Money,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530416,Can't Afford Care: Skipped Med To Save Money,43529539,Skipped Med To Save Money: No,2, No
+Healthcare Access & Utilization,43530416,Can't Afford Care: Skipped Med To Save Money,43530233,Skipped Med To Save Money: Yes,1, Yes
+Healthcare Access & Utilization,43530417,Can't Afford Care: Took Less Med To Save Money,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530417,Can't Afford Care: Took Less Med To Save Money,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530417,Can't Afford Care: Took Less Med To Save Money,43529562,Took Less Med To Save Money: No,2, No
+Healthcare Access & Utilization,43530417,Can't Afford Care: Took Less Med To Save Money,43530256,Took Less Med To Save Money: Yes,1, Yes
+Healthcare Access & Utilization,43530418,Insurance: Insurance Accepted,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530418,Insurance: Insurance Accepted,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530418,Insurance: Insurance Accepted,43529377,Insurance Accepted: No,2, No
+Healthcare Access & Utilization,43530418,Insurance: Insurance Accepted,43530070,Insurance Accepted: Yes,1, Yes
+Healthcare Access & Utilization,43530437,Health Advice: Asked For Opinion,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530437,Health Advice: Asked For Opinion,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530437,Health Advice: Asked For Opinion,43529575,Asked For Opinion: None Of The Time,1, None Of The Time
+Healthcare Access & Utilization,43530437,Health Advice: Asked For Opinion,43529843,Asked For Opinion: Some Of The Time,2, Some Of The Time
+Healthcare Access & Utilization,43530437,Health Advice: Asked For Opinion,43529238,Asked For Opinion: Most Of The Time,3, Most Of The Time
+Healthcare Access & Utilization,43530437,Health Advice: Asked For Opinion,43528386,Asked For Opinion: Always,4, Always
+Healthcare Access & Utilization,43530438,Health Advice: Ease of Understanding,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530438,Health Advice: Ease of Understanding,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530438,Health Advice: Ease of Understanding,43529577,Ease of Understanding: None Of The Time,1, None Of The Time
+Healthcare Access & Utilization,43530438,Health Advice: Ease of Understanding,43529845,Ease of Understanding: Some Of The Time,2, Some Of The Time
+Healthcare Access & Utilization,43530438,Health Advice: Ease of Understanding,43529240,Ease of Understanding: Most Of The Time,3, Most Of The Time
+Healthcare Access & Utilization,43530438,Health Advice: Ease of Understanding,43528388,Ease of Understanding: Always,4, Always
+Healthcare Access & Utilization,43530439,Health Advice: Respected By Provider,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530439,Health Advice: Respected By Provider,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530439,Health Advice: Respected By Provider,43529579,Respected By Provider: None Of The Time,0, None Of The Time
+Healthcare Access & Utilization,43530439,Health Advice: Respected By Provider,43529847,Respected By Provider: Some Of The Time,1, Some Of The Time
+Healthcare Access & Utilization,43530439,Health Advice: Respected By Provider,43529242,Respected By Provider: Most Of The Time,2, Most Of The Time
+Healthcare Access & Utilization,43530439,Health Advice: Respected By Provider,43528390,Respected By Provider: Always,3, Always
+Healthcare Access & Utilization,43530557,Can't Afford Care: Worried About Paying,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530557,Can't Afford Care: Worried About Paying,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530557,Can't Afford Care: Worried About Paying,43529586,Worried About Paying: Not At All Worried,1, Not At All Worried
+Healthcare Access & Utilization,43530557,Can't Afford Care: Worried About Paying,43529850,Worried About Paying: Somewhat Worried,2, Somewhat Worried
+Healthcare Access & Utilization,43530557,Can't Afford Care: Worried About Paying,43529954,Worried About Paying: Very Worried,3, Very Worried
+Healthcare Access & Utilization,43530559,Insurance: Healthcare Coverage,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530559,Insurance: Healthcare Coverage,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530559,Insurance: Healthcare Coverage,43529982,Healthcare Coverage: Worse,1, Worse
+Healthcare Access & Utilization,43530559,Insurance: Healthcare Coverage,43528346,Healthcare Coverage: About The Same,2, About The Same
+Healthcare Access & Utilization,43530559,Insurance: Healthcare Coverage,43528458,Healthcare Coverage: Better,3, Better
+Healthcare Access & Utilization,43530562,Health Advice: Place for Health Advice,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530562,Health Advice: Place for Health Advice,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530562,Health Advice: Place for Health Advice,43529908,Place for Health Advice: No,2, No
+Healthcare Access & Utilization,43530562,Health Advice: Place for Health Advice,43530103,Place for Health Advice: Yes,1, Yes
+Healthcare Access & Utilization,43530562,Health Advice: Place for Health Advice,43529907,Place for Health Advice: More Than One,2, More Than One
+Healthcare Access & Utilization,43530583,Delayed Medical Care: Can't Afford Co-pay,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530583,Delayed Medical Care: Can't Afford Co-pay,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530583,Delayed Medical Care: Can't Afford Co-pay,43529317,Delayed Care Due to Can't Afford Co-pay: No,2, No
+Healthcare Access & Utilization,43530583,Delayed Medical Care: Can't Afford Co-pay,43530010,Delayed Care Due to Can't Afford Co-pay: Yes,1, Yes
+Healthcare Access & Utilization,43530584,Delayed Medical Care: Had To Pay Out Of Pocket,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530584,Delayed Medical Care: Had To Pay Out Of Pocket,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530584,Delayed Medical Care: Had To Pay Out Of Pocket,43529359,Delayed Care Due to Had To Pay Out Of Pocket: No,2, No
+Healthcare Access & Utilization,43530584,Delayed Medical Care: Had To Pay Out Of Pocket,43530052,Delayed Care Due to Had To Pay Out Of Pocket: Yes,1, Yes
+Healthcare Access & Utilization,43530585,Delayed Medical Care: Deductible Too High,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530585,Delayed Medical Care: Deductible Too High,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530585,Delayed Medical Care: Deductible Too High,43529332,Delayed Care Due to Deductible Too High: No,2, No
+Healthcare Access & Utilization,43530585,Delayed Medical Care: Deductible Too High,43530025,Delayed Care Due to Deductible Too High: Yes,1, Yes
+Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,43528260,General Doctor Visits: 1,1,1
+Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,43528304,General Doctor Visits: 2 to 3,2, 2 to 3
+Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,43528315,General Doctor Visits: 4 to 5,3, 4 to 5
+Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,43528326,General Doctor Visits: 6 to 7,4, 6 to 7
+Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,43528338,General Doctor Visits: 8 to 9,5, 8 to 9
+Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,43528271,General Doctor Visits: 10 to 12,6, 10 to 12
+Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,43528282,General Doctor Visits: 13 to 15,7, 13 to 15
+Healthcare Access & Utilization,43530588,Health Advice: General Doctor Visits,43528293,General Doctor Visits: 16 or M ore,8, 16 or M ore
+Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,43528257,Chiropractor Visits: 1,1,1
+Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,43528301,Chiropractor Visits: 2 to 3,2, 2 to 3
+Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,43528312,Chiropractor Visits: 4 to 5,3, 4 to 5
+Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,43528323,Chiropractor Visits: 6 to 7,4, 6 to 7
+Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,43528335,Chiropractor Visits: 8 to 9,5, 8 to 9
+Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,43528268,Chiropractor Visits: 10 to 12,6, 10 to 12
+Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,43528279,Chiropractor Visits: 13 to 15,7, 13 to 15
+Healthcare Access & Utilization,43530589,Health Advice: Chiropractor Visits,43528290,Chiropractor Visits: 16 or M ore,8, 16 or M ore
+Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,43528266,Podiatrist Visits: 1,1,1
+Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,43528310,Podiatrist Visits: 2 to 3,2, 2 to 3
+Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,43528321,Podiatrist Visits: 4 to 5,3, 4 to 5
+Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,43528332,Podiatrist Visits: 6 to 7,4, 6 to 7
+Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,43528344,Podiatrist Visits: 8 to 9,5, 8 to 9
+Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,43528277,Podiatrist Visits: 10 to 12,6, 10 to 12
+Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,43528288,Podiatrist Visits: 13 to 15,7, 13 to 15
+Healthcare Access & Utilization,43530590,Health Advice: Podiatrist Visits,43528299,Podiatrist Visits: 16 or More,8, 16 or More
+Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,43528259,Eye Doctor Visits: 1,1,1
+Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,43528303,Eye Doctor Visits: 2 to 3,2, 2 to 3
+Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,43528314,Eye Doctor Visits: 4 to 5,3, 4 to 5
+Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,43528325,Eye Doctor Visits: 6 to 7,4, 6 to 7
+Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,43528337,Eye Doctor Visits: 8 to 9,5, 8 to 9
+Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,43528270,Eye Doctor Visits: 10 to 12,6, 10 to 12
+Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,43528281,Eye Doctor Visits: 13 to 15,7, 13 to 15
+Healthcare Access & Utilization,43530591,Health Advice: Eye Doctor Visits,43528292,Eye Doctor Visits: 16 or More,8, 16 or More
+Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",43528265,"PT, ST, RT, Audiologist or OT Visits: 1",1,1
+Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",43528309,"PT, ST, RT, Audiologist or OT: 2 to 3",2, 2 to 3
+Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",43528320,"PT, ST, RT, Audiologist or OT Visits: 4 to 5",3, 4 to 5
+Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",43528331,"PT, ST, RT, Audiologist or OT Visits: 6 to 7",4, 6 to 7
+Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",43528343,"PT, ST, RT, Audiologist or OT Visits: 8 to 9",5, 8 to 9
+Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",43528276,"PT, ST, RT, Audiologist or OT Visits: 10 to 12",6, 10 to 12
+Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",43528287,"PT, ST, RT, Audiologist or OT Visits: 13 to 15",7, 13 to 15
+Healthcare Access & Utilization,43530592,"Health Advice: Physical Therapist, Speech Therapist, Respiratory Therapist, Audiologist, or Occupational Therapist Visits",43528298,"PT, ST, RT, Audiologist or OT Visits: 16 or More",8, 16 or More
+Healthcare Access & Utilization,43530593,Health Advice: What Kind Of Place,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530593,Health Advice: What Kind Of Place,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530593,Health Advice: What Kind Of Place,43528645,What Kind Of Place: Doctors Office,1, Doctors Office
+Healthcare Access & Utilization,43530593,Health Advice: What Kind Of Place,43528646,What Kind Of Place: No One Place Most Often,2, No One Place Most Often
+Healthcare Access & Utilization,43530593,Health Advice: What Kind Of Place,43528803,What Kind Of Place: Emergency Room,3, Emergency Room
+Healthcare Access & Utilization,43530593,Health Advice: What Kind Of Place,43529848,What Kind Of Place: Some Other Place,4, Some Other Place
+Healthcare Access & Utilization,43530593,Health Advice: What Kind Of Place,43529948,What Kind Of Place: Urgent Care,5, Urgent Care
+Healthcare Access & Utilization,43530594,Delayed Medical Care: Nervous,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530594,Delayed Medical Care: Nervous,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530594,Delayed Medical Care: Nervous,43529396,Delayed Care Nervous: No,2, No
+Healthcare Access & Utilization,43530594,Delayed Medical Care: Nervous,43530089,Delayed Care Nervous: Yes,1, Yes
+Healthcare Access & Utilization,43530595,Health Advice: Spoken To Professional,903087,PMI: Dont Know,-99, Dont Know
+Healthcare Access & Utilization,43530595,Health Advice: Spoken To Professional,903096,PMI: Skip,-98, Skip
+Healthcare Access & Utilization,43530595,Health Advice: Spoken To Professional,43529282,Spoken To Professional: Never,1, Never
+Healthcare Access & Utilization,43530595,Health Advice: Spoken To Professional,43528334,Spoken To Professional: 6mo Or Less,2, 6mo Or Less
+Healthcare Access & Utilization,43530595,Health Advice: Spoken To Professional,43529237,Spoken To Professional: 6 Mo To 1 Year Ago,3, 6 Mo To 1 Year Ago
+Healthcare Access & Utilization,43530595,Health Advice: Spoken To Professional,43530564,Spoken To Professional: 1 To 2 Years Ago,4, 1 To 2 Years Ago
+Healthcare Access & Utilization,43530595,Health Advice: Spoken To Professional,43530565,Spoken To Professional: 2 To 5 Years Ago,5, 2 To 5 Years Ago
+Healthcare Access & Utilization,43530595,Health Advice: Spoken To Professional,43530566,Spoken To Professional: More Than 5 Years Ago,6, More Than 5 Years Ago
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `omop2poll-0.1.2/omop2poll/tests/test_load_data.py` & `omop2poll-0.1.3/omop2poll/tests/test_load_data.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import pytest
-from unittest.mock import patch, mock_open
-from omop2poll.load_data import load_survey_data
-import pandas as pd
-
-
-def test_load_survey_data_file_not_found():
-    with patch("os.path.exists", return_value=False):
-        with pytest.raises(FileNotFoundError):
-            load_survey_data("nonexistent_file.csv")
-
-
-def test_load_survey_data_reads_correctly():
-    data = "col1,col2\nval1,val2"
-    expected_df = pd.DataFrame({"col1": ["val1"], "col2": ["val2"]})
-
-    with patch('pandas.read_csv') as mock_read_csv:
-        mock_read_csv.return_value = expected_df
-        with patch("os.path.exists", return_value=True):
-            df = load_survey_data("dummy_file.csv")
-            mock_read_csv.assert_called_once()  # Ensures pandas.read_csv was called
-            pd.testing.assert_frame_equal(df, expected_df)
+import pytest
+from unittest.mock import patch, mock_open
+from omop2poll.load_data import load_survey_data
+import pandas as pd
+
+
+def test_load_survey_data_file_not_found():
+    with patch("os.path.exists", return_value=False):
+        with pytest.raises(FileNotFoundError):
+            load_survey_data("nonexistent_file.csv")
+
+
+def test_load_survey_data_reads_correctly():
+    data = "col1,col2\nval1,val2"
+    expected_df = pd.DataFrame({"col1": ["val1"], "col2": ["val2"]})
+
+    with patch('pandas.read_csv') as mock_read_csv:
+        mock_read_csv.return_value = expected_df
+        with patch("os.path.exists", return_value=True):
+            df = load_survey_data("dummy_file.csv")
+            mock_read_csv.assert_called_once()  # Ensures pandas.read_csv was called
+            pd.testing.assert_frame_equal(df, expected_df)
```

### Comparing `omop2poll-0.1.2/omop2poll/tests/test_map_responses.py` & `omop2poll-0.1.3/omop2poll/tests/test_map_responses.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from omop2poll.map_responses import map_responses
-from unittest.mock import patch
-import pandas as pd
-
-
-def test_map_responses_correctly_maps():
-    survey_data = pd.DataFrame({
-        'question_concept_id': [43528661, 43528660],
-        'answer_concept_id': [43529550, 903096],
-        'answer_numeric': [0, -98],
-        'answer_text': ['No', 'Skip']
-    })
-
-    input_data = pd.DataFrame({
-        'question_concept_id': [43528661, 43528660],
-        'answer_concept_id': [43529550, 903096],
-    })
-
-    with patch("omop2poll-a.load_data.load_survey_data", return_value=survey_data):
-        result = map_responses(input_data)
-        assert result['answer_numeric'].tolist() == [0, -98]
-        assert result['answer_text'].tolist() == ['No', 'Skip']
+from omop2poll.map_responses import map_responses
+from unittest.mock import patch
+import pandas as pd
+
+
+def test_map_responses_correctly_maps():
+    survey_data = pd.DataFrame({
+        'question_concept_id': [43528661, 43528660],
+        'answer_concept_id': [43529550, 903096],
+        'answer_numeric': [0, -98],
+        'answer_text': ['No', 'Skip']
+    })
+
+    input_data = pd.DataFrame({
+        'question_concept_id': [43528661, 43528660],
+        'answer_concept_id': [43529550, 903096],
+    })
+
+    with patch("omop2poll-a.load_data.load_survey_data", return_value=survey_data):
+        result = map_responses(input_data)
+        assert result['answer_numeric'].tolist() == [0, -98]
+        assert result['answer_text'].tolist() == ['No', 'Skip']
```

### Comparing `omop2poll-0.1.2/omop2poll/tests/test_pivot_data_numeric.py` & `omop2poll-0.1.3/omop2poll/tests/test_pivot_data_numeric.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import pytest
-from omop2poll.pivot_data import pivot_data_numeric
-import pandas as pd
-import os
-
-
-def test_pivot_data_numeric_creates_correct_output(tmp_path):
-    d = tmp_path / "sub"
-    d.mkdir()
-    sample_file = d / "test.csv"
-    sample_data = "respondent_id,question_concept_id,answer_numeric\n1,100,5\n2,100,6"
-    sample_file.write_text(sample_data)
-
-    expected_output_path = d / "pivot_n_test.csv"
-    expected_output_file = str(expected_output_path)
-
-    pivot_data_numeric(str(sample_file))
-
-    assert os.path.exists(expected_output_file), "The expected pivoted output file does not exist."
-
-    expected_df = pd.DataFrame({
-        'q100': [5, 6]
-    }, index=[1, 2])
-    expected_df.index.name = 'respondent_id'
-    output_df = pd.read_csv(expected_output_file, index_col='respondent_id')
-
-    pd.testing.assert_frame_equal(output_df, expected_df)
-
+import pytest
+from omop2poll.pivot_data import pivot_data_numeric
+import pandas as pd
+import os
+
+
+def test_pivot_data_numeric_creates_correct_output(tmp_path):
+    d = tmp_path / "sub"
+    d.mkdir()
+    sample_file = d / "test.csv"
+    sample_data = "respondent_id,question_concept_id,answer_numeric\n1,100,5\n2,100,6"
+    sample_file.write_text(sample_data)
+
+    expected_output_path = d / "pivot_n_test.csv"
+    expected_output_file = str(expected_output_path)
+
+    pivot_data_numeric(str(sample_file))
+
+    assert os.path.exists(expected_output_file), "The expected pivoted output file does not exist."
+
+    expected_df = pd.DataFrame({
+        'q100': [5, 6]
+    }, index=[1, 2])
+    expected_df.index.name = 'respondent_id'
+    output_df = pd.read_csv(expected_output_file, index_col='respondent_id')
+
+    pd.testing.assert_frame_equal(output_df, expected_df)
+
```

### Comparing `omop2poll-0.1.2/omop2poll/tests/test_pivot_data_text.py` & `omop2poll-0.1.3/omop2poll/tests/test_pivot_data_text.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import pytest
-from omop2poll.pivot_data import pivot_data_text
-import pandas as pd
-import os
-
-
-def test_pivot_data_text_creates_correct_output(tmp_path):
-    d = tmp_path / "sub"
-    d.mkdir()
-    sample_text_file = d / "test_text.csv"
-    sample_text_data = "respondent_id,question_concept_id,answer_text\n1,100,Yes\n2,100,No"
-    sample_text_file.write_text(sample_text_data)
-
-    expected_text_path = d / "pivot_t_test_text.csv"
-    expected_text_file = str(expected_text_path)
-
-    pivot_data_text(str(sample_text_file))
-
-    assert os.path.exists(expected_text_file), "The expected pivoted output file does not exist."
-
-    expected_text_df = pd.DataFrame({
-        'q100': ['Yes', 'No']
-    }, index=[1, 2])
-    expected_text_df.index.name = 'respondent_id'
-    output_text_df = pd.read_csv(expected_text_file, index_col='respondent_id')
-
-    pd.testing.assert_frame_equal(output_text_df, expected_text_df)
+import pytest
+from omop2poll.pivot_data import pivot_data_text
+import pandas as pd
+import os
+
+
+def test_pivot_data_text_creates_correct_output(tmp_path):
+    d = tmp_path / "sub"
+    d.mkdir()
+    sample_text_file = d / "test_text.csv"
+    sample_text_data = "respondent_id,question_concept_id,answer_text\n1,100,Yes\n2,100,No"
+    sample_text_file.write_text(sample_text_data)
+
+    expected_text_path = d / "pivot_t_test_text.csv"
+    expected_text_file = str(expected_text_path)
+
+    pivot_data_text(str(sample_text_file))
+
+    assert os.path.exists(expected_text_file), "The expected pivoted output file does not exist."
+
+    expected_text_df = pd.DataFrame({
+        'q100': ['Yes', 'No']
+    }, index=[1, 2])
+    expected_text_df.index.name = 'respondent_id'
+    output_text_df = pd.read_csv(expected_text_file, index_col='respondent_id')
+
+    pd.testing.assert_frame_equal(output_text_df, expected_text_df)
```

### Comparing `omop2poll-0.1.2/PKG-INFO` & `omop2poll-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: omop2poll
-Version: 0.1.2
+Version: 0.1.3
 Summary: The 'omop2poll' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis.
 Home-page: https://github.com/elifdy/omop2poll.git
 License: MIT
 Author: Elif Dede Yildirim
 Author-email: elifdy@auburn.edu
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/elifdy/omop2poll.git
 Description-Content-Type: text/markdown
```

