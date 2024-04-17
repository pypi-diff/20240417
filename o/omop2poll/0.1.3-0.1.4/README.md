# Comparing `tmp/omop2poll-0.1.3.tar.gz` & `tmp/omop2poll-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omop2poll-0.1.3.tar", max compression
+gzip compressed data, was "omop2poll-0.1.4.tar", max compression
```

## Comparing `omop2poll-0.1.3.tar` & `omop2poll-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      291 2024-04-16 17:33:06.142843 omop2poll-0.1.3/omop2poll/__init__.py
--rw-r--r--   0        0        0     3564 2024-04-16 17:28:40.040097 omop2poll-0.1.3/omop2poll/codebook.py
--rw-r--r--   0        0        0     1511 2024-04-16 16:37:21.487473 omop2poll-0.1.3/omop2poll/map_responses.py
--rw-r--r--   0        0        0     1553 2024-04-16 14:50:30.296363 omop2poll-0.1.3/omop2poll/pivot_data.py
--rw-r--r--   0        0        0      813 2024-04-16 15:10:20.536914 omop2poll-0.1.3/omop2poll/recode_missing.py
--rw-r--r--   0        0        0    42126 2024-04-16 16:25:24.495072 omop2poll-0.1.3/omop2poll/survey_healthcare.csv
--rw-r--r--   0        0        0        0 2024-04-16 14:50:30.298363 omop2poll-0.1.3/omop2poll/tests/__init__.py
--rw-r--r--   0        0        0       30 2024-04-16 14:50:30.298363 omop2poll-0.1.3/omop2poll/tests/pivot_n_test.csv
--rw-r--r--   0        0        0       37 2024-04-16 14:50:30.298363 omop2poll-0.1.3/omop2poll/tests/pivot_t_test_text.csv
--rw-r--r--   0        0        0      570 2024-04-16 14:50:30.299363 omop2poll-0.1.3/omop2poll/tests/test_codebook.py
--rw-r--r--   0        0        0      853 2024-04-16 14:50:30.300363 omop2poll-0.1.3/omop2poll/tests/test_load_data.py
--rw-r--r--   0        0        0      778 2024-04-16 14:50:30.300363 omop2poll-0.1.3/omop2poll/tests/test_map_responses.py
--rw-r--r--   0        0        0      894 2024-04-16 14:50:30.301363 omop2poll-0.1.3/omop2poll/tests/test_pivot_data_numeric.py
--rw-r--r--   0        0        0      940 2024-04-16 14:50:30.301363 omop2poll-0.1.3/omop2poll/tests/test_pivot_data_text.py
--rw-r--r--   0        0        0      233 2024-04-16 14:50:30.301363 omop2poll-0.1.3/omop2poll/tests/test_recode_missing.py
--rw-r--r--   0        0        0      527 2024-04-16 17:05:39.472430 omop2poll-0.1.3/omop2poll/tests/trial.py
--rw-r--r--   0        0        0      835 2024-04-16 17:45:53.231110 omop2poll-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4549 2024-04-16 14:50:30.293363 omop2poll-0.1.3/README.md
--rw-r--r--   0        0        0     5570 1970-01-01 00:00:00.000000 omop2poll-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-03-30 01:48:44.188378 omop2poll-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4515 2024-03-30 02:01:42.491653 omop2poll-0.1.4/README.md
+-rw-r--r--   0        0        0     6148 2024-04-16 23:53:52.630665 omop2poll-0.1.4/omop2poll/.DS_Store
+-rw-r--r--   0        0        0      289 2024-04-16 23:39:52.893808 omop2poll-0.1.4/omop2poll/__init__.py
+-rw-r--r--   0        0        0     3452 2024-04-16 23:47:54.624690 omop2poll-0.1.4/omop2poll/codebook.py
+-rw-r--r--   0        0        0     1473 2024-04-16 23:52:37.337631 omop2poll-0.1.4/omop2poll/map_responses.py
+-rw-r--r--   0        0        0     1190 2024-04-16 23:47:54.633321 omop2poll-0.1.4/omop2poll/pivot_data.py
+-rw-r--r--   0        0        0      795 2024-04-16 23:39:52.869164 omop2poll-0.1.4/omop2poll/recode_missing.py
+-rw-r--r--   0        0        0    42126 2024-04-16 23:50:27.759328 omop2poll-0.1.4/omop2poll/survey_healthcare.csv
+-rw-r--r--   0        0        0        0 2024-03-30 02:18:26.796265 omop2poll-0.1.4/omop2poll/tests/__init__.py
+-rw-r--r--   0        0        0       27 2024-03-30 02:01:46.517346 omop2poll-0.1.4/omop2poll/tests/pivot_n_test.csv
+-rw-r--r--   0        0        0       34 2024-03-30 02:01:46.519564 omop2poll-0.1.4/omop2poll/tests/pivot_t_test_text.csv
+-rw-r--r--   0        0        0   773302 2024-04-16 05:13:20.043992 omop2poll-0.1.4/omop2poll/tests/recoded_data.csv
+-rw-r--r--   0        0        0      547 2024-03-30 02:01:46.533897 omop2poll-0.1.4/omop2poll/tests/test_codebook.py
+-rw-r--r--   0        0        0     1528 2024-04-12 19:29:27.246356 omop2poll-0.1.4/omop2poll/tests/test_map_responses.py
+-rw-r--r--   0        0        0      866 2024-03-30 02:01:46.526224 omop2poll-0.1.4/omop2poll/tests/test_pivot_data_numeric.py
+-rw-r--r--   0        0        0      913 2024-03-30 02:01:46.521352 omop2poll-0.1.4/omop2poll/tests/test_pivot_data_text.py
+-rw-r--r--   0        0        0      226 2024-03-30 02:01:46.527845 omop2poll-0.1.4/omop2poll/tests/test_recode_missing.py
+-rw-r--r--   0        0        0      800 2024-04-17 01:23:26.590381 omop2poll-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5526 1970-01-01 00:00:00.000000 omop2poll-0.1.4/PKG-INFO
```

### Comparing `omop2poll-0.1.3/omop2poll/codebook.py` & `omop2poll-0.1.4/omop2poll/codebook.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-import pandas as pd
-
-
-def load_data(source):
-    if isinstance(source, pd.DataFrame):
-        return source
-    elif isinstance(source, str):
-        if source.endswith('.csv'):
-            return pd.read_csv(source)
-        elif source.endswith('.txt'):
-            return pd.read_csv(source, delimiter='\t')
-        elif source.endswith('.xlsx'):
-            return pd.read_excel(source)
-        else:
-            raise ValueError("Unsupported file type provided.")
-    else:
-        raise TypeError("Input source must be a pandas DataFrame or a filepath as a string.")
-
-
-def create_codebook(dataframe):
-
-    required_columns = ['question_concept_id', 'question']
-    response_columns = ['answer_concept_id', 'answer', 'answer_text', 'answer_numeric']
-
-    response_columns = [col for col in response_columns if col in dataframe.columns]
-
-    if not all(col in dataframe.columns for col in required_columns):
-        raise ValueError("Dataframe must contain the necessary columns: 'question_concept_id' and 'question'.")
-
-    dataframe['question_concept_id'] = dataframe['question_concept_id'].astype(str)
-
-    grouped = dataframe.groupby(required_columns).apply(
-        lambda x: x[response_columns].drop_duplicates().reset_index(drop=True)
-    )
-
-    codebook_df = grouped.reset_index(drop=False)
-
-    codebook_df = codebook_df[required_columns + response_columns].drop_duplicates()
-
-    return codebook_df
-
-
-def generate_codebook(source):
-
-    try:
-
-        data = load_data(source)
-
-        codebook_df = create_codebook(data)
-
-        return codebook_df
-    except ImportError:
-        print("Required module not installed.")
-    except Exception as e:
-        print(f"Error: {e}")
-
-
-def print_codebook(source):
-
-    try:
-
-        data = load_data(source)
-
-        codebook_df = create_codebook(data)
-
-
-        from tabulate import tabulate
-        print(tabulate(codebook_df, headers='keys', tablefmt='psql', showindex=False))
-    except ImportError:
-        print("Tabulate module not installed, using default print.")
-        print(codebook_df)
-    except Exception as e:
-        print(f"Error: {e}")
-
-
-def create_formatted_codebook(dataframe):
-
-    grouped = dataframe.groupby(['question_concept_id', 'question'], sort=False)
-
-    formatted_data = []
-
-    for (question_concept_id, question), group in grouped:
-
-        is_first = True
-
-        for idx, row in group.iterrows():
-            if is_first:
-                formatted_data.append({
-                    'question_concept_id': question_concept_id,
-                    'question': question,
-                    'answer_concept_id': row['answer_concept_id'],
-                    'answer_concept_id recoded as answer_numeric': row['answer_numeric'],
-                    'answer': row['answer'],
-                    'answer recoded as answer_text': row['answer_text']
-
-                })
-                is_first = False
-            else:
-                formatted_data.append({
-                    'question_concept_id': '',
-                    'question': '',
-                    'answer_concept_id': row['answer_concept_id'],
-                    'answer_concept_id recoded as answer_numeric': row['answer_numeric'],
-                    'answer': row['answer'],
-                    'answer recoded as answer_text': row['answer_text']
-
-                })
-
-    formatted_codebook_df = pd.DataFrame(formatted_data)
-
-    return formatted_codebook_df.to_html(index=False, escape=False)
-
+import pandas as pd
+
+
+def load_data(source):
+    if isinstance(source, pd.DataFrame):
+        return source
+    elif isinstance(source, str):
+        if source.endswith('.csv'):
+            return pd.read_csv(source)
+        elif source.endswith('.txt'):
+            return pd.read_csv(source, delimiter='\t')
+        elif source.endswith('.xlsx'):
+            return pd.read_excel(source)
+        else:
+            raise ValueError("Unsupported file type provided.")
+    else:
+        raise TypeError("Input source must be a pandas DataFrame or a filepath as a string.")
+
+
+def create_codebook(dataframe):
+
+    required_columns = ['question_concept_id', 'question']
+    response_columns = ['answer_concept_id', 'answer', 'answer_text', 'answer_numeric']
+
+    response_columns = [col for col in response_columns if col in dataframe.columns]
+
+    if not all(col in dataframe.columns for col in required_columns):
+        raise ValueError("Dataframe must contain the necessary columns: 'question_concept_id' and 'question'.")
+
+    dataframe['question_concept_id'] = dataframe['question_concept_id'].astype(str)
+
+    grouped = dataframe.groupby(required_columns).apply(
+        lambda x: x[response_columns].drop_duplicates().reset_index(drop=True)
+    )
+
+    codebook_df = grouped.reset_index(drop=False)
+
+    codebook_df = codebook_df[required_columns + response_columns].drop_duplicates()
+
+    return codebook_df
+
+
+def generate_codebook(source):
+
+    try:
+
+        data = load_data(source)
+
+        codebook_df = create_codebook(data)
+
+        return codebook_df
+    except ImportError:
+        print("Required module not installed.")
+    except Exception as e:
+        print(f"Error: {e}")
+
+
+def print_codebook(source):
+
+    try:
+
+        data = load_data(source)
+
+        codebook_df = create_codebook(data)
+
+
+        from tabulate import tabulate
+        print(tabulate(codebook_df, headers='keys', tablefmt='psql', showindex=False))
+    except ImportError:
+        print("Tabulate module not installed, using default print.")
+        print(codebook_df)
+    except Exception as e:
+        print(f"Error: {e}")
+
+
+def create_formatted_codebook(dataframe):
+
+    grouped = dataframe.groupby(['question_concept_id', 'question'], sort=False)
+
+    formatted_data = []
+
+    for (question_concept_id, question), group in grouped:
+
+        is_first = True
+
+        for idx, row in group.iterrows():
+            if is_first:
+                formatted_data.append({
+                    'question_concept_id': question_concept_id,
+                    'question': question,
+                    'answer_concept_id': row['answer_concept_id'],
+                    'answer_concept_id recoded as answer_numeric': row['answer_numeric'],
+                    'answer': row['answer'],
+                    'answer recoded as answer_text': row['answer_text']
+
+                })
+                is_first = False
+            else:
+                formatted_data.append({
+                    'question_concept_id': '',
+                    'question': '',
+                    'answer_concept_id': row['answer_concept_id'],
+                    'answer_concept_id recoded as answer_numeric': row['answer_numeric'],
+                    'answer': row['answer'],
+                    'answer recoded as answer_text': row['answer_text']
+
+                })
+
+    formatted_codebook_df = pd.DataFrame(formatted_data)
+
+    return formatted_codebook_df.to_html(index=False, escape=False)
+
```

### Comparing `omop2poll-0.1.3/omop2poll/map_responses.py` & `omop2poll-0.1.4/omop2poll/map_responses.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import pandas as pd
-import os
-
-
-def load_survey_data(filename='survey_healthcare.csv'):
-    current_dir = os.path.dirname(os.path.realpath(__file__))
-
-    file_path = os.path.join(current_dir, filename)
-    if not os.path.exists(file_path):
-        raise FileNotFoundError(f"File path {file_path} does not exist.")
-    return pd.read_csv(file_path)
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

### Comparing `omop2poll-0.1.3/omop2poll/survey_healthcare.csv` & `omop2poll-0.1.4/omop2poll/survey_healthcare.csv`

 * *Files identical despite different names*

### Comparing `omop2poll-0.1.3/omop2poll/tests/test_pivot_data_numeric.py` & `omop2poll-0.1.4/omop2poll/tests/test_pivot_data_numeric.py`

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

### Comparing `omop2poll-0.1.3/omop2poll/tests/test_pivot_data_text.py` & `omop2poll-0.1.4/omop2poll/tests/test_pivot_data_text.py`

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

### Comparing `omop2poll-0.1.3/README.md` & `omop2poll-0.1.4/README.md`

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

### Comparing `omop2poll-0.1.3/PKG-INFO` & `omop2poll-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: omop2poll
-Version: 0.1.3
+Version: 0.1.4
 Summary: The 'omop2poll' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis.
 Home-page: https://github.com/elifdy/omop2poll.git
 License: MIT
 Author: Elif Dede Yildirim
 Author-email: elifdy@auburn.edu
-Requires-Python: >=3.9
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/elifdy/omop2poll.git
```

