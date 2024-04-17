# Comparing `tmp/benchq-0.6.0-py3-none-any.whl.zip` & `tmp/benchq-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,67 +1,85 @@
-Zip file size: 105178 bytes, number of entries: 65
--rw-r--r--  2.0 unx      525 b- defN 23-Oct-26 13:52 benchq/__init__.py
--rw-r--r--  2.0 unx      541 b- defN 23-Oct-26 13:52 benchq/timing.py
--rw-r--r--  2.0 unx     5958 b- defN 23-Oct-26 13:52 benchq/vizualization_tools.py
--rw-r--r--  2.0 unx      137 b- defN 23-Oct-26 13:52 benchq/algorithms/__init__.py
--rw-r--r--  2.0 unx     1083 b- defN 23-Oct-26 13:52 benchq/algorithms/gsee.py
--rw-r--r--  2.0 unx     4415 b- defN 23-Oct-26 13:52 benchq/algorithms/ld_gsee.py
--rw-r--r--  2.0 unx    14027 b- defN 23-Oct-26 13:52 benchq/algorithms/lde_solver.py
--rw-r--r--  2.0 unx     5017 b- defN 23-Oct-26 13:52 benchq/algorithms/lin_and_dong_qsp.py
--rw-r--r--  2.0 unx     2586 b- defN 23-Oct-26 13:52 benchq/algorithms/qaoa.py
--rw-r--r--  2.0 unx     2788 b- defN 23-Oct-26 13:52 benchq/algorithms/time_evolution.py
--rw-r--r--  2.0 unx      537 b- defN 23-Oct-26 13:52 benchq/algorithms/utils/compression_gadget.py
--rw-r--r--  2.0 unx     4694 b- defN 23-Oct-26 13:52 benchq/algorithms/utils/convex_optimization.py
--rw-r--r--  2.0 unx    15067 b- defN 23-Oct-26 13:52 benchq/algorithms/utils/qsp_solver.py
--rw-r--r--  2.0 unx     3939 b- defN 23-Oct-26 13:52 benchq/block_encodings/block_encoding_utils.py
--rw-r--r--  2.0 unx     2040 b- defN 23-Oct-26 13:52 benchq/block_encodings/offset_tridiagonal.py
--rw-r--r--  2.0 unx      785 b- defN 23-Oct-26 13:52 benchq/compilation/__init__.py
--rw-r--r--  2.0 unx     4524 b- defN 23-Oct-26 13:52 benchq/compilation/graph_sim_data.jl
--rw-r--r--  2.0 unx     1855 b- defN 23-Oct-26 13:52 benchq/compilation/initialize_julia.py
--rw-r--r--  2.0 unx     3106 b- defN 23-Oct-26 13:52 benchq/compilation/jabalizer_wrapper.jl
--rw-r--r--  2.0 unx     2367 b- defN 23-Oct-26 13:52 benchq/compilation/julia_utils.py
--rw-r--r--  2.0 unx     3067 b- defN 23-Oct-26 13:52 benchq/compilation/pyliqtr_transpilation.py
--rw-r--r--  2.0 unx    17410 b- defN 23-Oct-26 13:52 benchq/compilation/rbs_hyperparam_tuning.py
--rw-r--r--  2.0 unx    22742 b- defN 23-Oct-26 13:52 benchq/compilation/ruby_slippers.jl
--rw-r--r--  2.0 unx     9497 b- defN 23-Oct-26 13:52 benchq/compilation/transpile_to_native_gates.py
--rw-r--r--  2.0 unx      367 b- defN 23-Oct-26 13:52 benchq/conversions/__init__.py
--rw-r--r--  2.0 unx     3170 b- defN 23-Oct-26 13:52 benchq/conversions/_circuit_translations.py
--rw-r--r--  2.0 unx     1266 b- defN 23-Oct-26 13:52 benchq/conversions/_openfermion_pyliqtr.py
--rw-r--r--  2.0 unx     1608 b- defN 23-Oct-26 13:52 benchq/data_structures/__init__.py
--rw-r--r--  2.0 unx      688 b- defN 23-Oct-26 13:52 benchq/data_structures/algorithm_implementation.py
--rw-r--r--  2.0 unx     4386 b- defN 23-Oct-26 13:52 benchq/data_structures/decoder.py
--rw-r--r--  2.0 unx     3511 b- defN 23-Oct-26 13:52 benchq/data_structures/error_budget.py
--rw-r--r--  2.0 unx      837 b- defN 23-Oct-26 13:52 benchq/data_structures/graph_partition.py
--rw-r--r--  2.0 unx     9203 b- defN 23-Oct-26 13:52 benchq/data_structures/hardware_architecture_models.py
--rw-r--r--  2.0 unx     3970 b- defN 23-Oct-26 13:52 benchq/data_structures/quantum_program.py
--rw-r--r--  2.0 unx     3751 b- defN 23-Oct-26 13:52 benchq/data_structures/resource_info.py
--rw-r--r--  2.0 unx      287 b- defN 23-Oct-26 13:52 benchq/mlflow/__init__.py
--rw-r--r--  2.0 unx     3543 b- defN 23-Oct-26 13:52 benchq/mlflow/data_logging.py
--rw-r--r--  2.0 unx      323 b- defN 23-Oct-26 13:52 benchq/problem_embeddings/__init__.py
--rw-r--r--  2.0 unx    10310 b- defN 23-Oct-26 13:52 benchq/problem_embeddings/_qsp.py
--rw-r--r--  2.0 unx    12616 b- defN 23-Oct-26 13:52 benchq/problem_embeddings/_taylorization_lcu.py
--rw-r--r--  2.0 unx     1170 b- defN 23-Oct-26 13:52 benchq/problem_embeddings/_trotter.py
--rw-r--r--  2.0 unx      496 b- defN 23-Oct-26 13:52 benchq/problem_ingestion/__init__.py
--rw-r--r--  2.0 unx     6941 b- defN 23-Oct-26 13:52 benchq/problem_ingestion/hamiltonian_from_file.py
--rw-r--r--  2.0 unx     6214 b- defN 23-Oct-26 13:52 benchq/problem_ingestion/hamiltonian_generation.py
--rw-r--r--  2.0 unx    22503 b- defN 23-Oct-26 13:52 benchq/problem_ingestion/molecule_instance_generation.py
--rw-r--r--  2.0 unx      886 b- defN 23-Oct-26 13:52 benchq/problem_ingestion/vlasov.py
--rw-r--r--  2.0 unx      392 b- defN 23-Oct-26 13:52 benchq/resource_estimation/__init__.py
--rw-r--r--  2.0 unx     2775 b- defN 23-Oct-26 13:52 benchq/resource_estimation/_compute_lambda.py
--rw-r--r--  2.0 unx    10220 b- defN 23-Oct-26 13:52 benchq/resource_estimation/_footprint_analysis.py
--rw-r--r--  2.0 unx     4846 b- defN 23-Oct-26 13:52 benchq/resource_estimation/azure.py
--rw-r--r--  2.0 unx     3692 b- defN 23-Oct-26 13:52 benchq/resource_estimation/decoder_resource_estimator.py
--rw-r--r--  2.0 unx    11887 b- defN 23-Oct-26 13:52 benchq/resource_estimation/default_pipelines.py
--rw-r--r--  2.0 unx     3188 b- defN 23-Oct-26 13:52 benchq/resource_estimation/magic_state_distillation.py
--rw-r--r--  2.0 unx    11021 b- defN 23-Oct-26 13:52 benchq/resource_estimation/openfermion_re.py
--rw-r--r--  2.0 unx      878 b- defN 23-Oct-26 13:52 benchq/resource_estimation/graph/__init__.py
--rw-r--r--  2.0 unx     3950 b- defN 23-Oct-26 13:52 benchq/resource_estimation/graph/customizable_pipelines.py
--rw-r--r--  2.0 unx     8240 b- defN 23-Oct-26 13:52 benchq/resource_estimation/graph/extrapolation_estimator.py
--rw-r--r--  2.0 unx    17630 b- defN 23-Oct-26 13:52 benchq/resource_estimation/graph/graph_estimator.py
--rw-r--r--  2.0 unx     4856 b- defN 23-Oct-26 13:52 benchq/resource_estimation/graph/transformers.py
--rw-r--r--  2.0 unx     5728 b- defN 23-Oct-26 13:52 benchq/resource_estimation/graph/worstcase_footprint_estimator.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Oct-26 13:52 benchq-0.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     6511 b- defN 23-Oct-26 13:52 benchq-0.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Oct-26 13:52 benchq-0.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Oct-26 13:52 benchq-0.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6204 b- defN 23-Oct-26 13:52 benchq-0.6.0.dist-info/RECORD
-65 files, 340227 bytes uncompressed, 95096 bytes compressed:  72.0%
+Zip file size: 108344 bytes, number of entries: 83
+-rw-r--r--  2.0 unx      349 b- defN 24-Apr-17 18:22 benchq/__init__.py
+-rw-r--r--  2.0 unx      541 b- defN 24-Apr-17 18:22 benchq/timing.py
+-rw-r--r--  2.0 unx     5990 b- defN 24-Apr-17 18:22 benchq/visualization_tools.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 18:22 benchq/algorithms/__init__.py
+-rw-r--r--  2.0 unx     1308 b- defN 24-Apr-17 18:22 benchq/algorithms/profolio_optimization.py
+-rw-r--r--  2.0 unx     2853 b- defN 24-Apr-17 18:22 benchq/algorithms/time_evolution.py
+-rw-r--r--  2.0 unx      431 b- defN 24-Apr-17 18:22 benchq/algorithms/data_structures/__init__.py
+-rw-r--r--  2.0 unx      730 b- defN 24-Apr-17 18:22 benchq/algorithms/data_structures/algorithm_implementation.py
+-rw-r--r--  2.0 unx     3511 b- defN 24-Apr-17 18:22 benchq/algorithms/data_structures/error_budget.py
+-rw-r--r--  2.0 unx      858 b- defN 24-Apr-17 18:22 benchq/algorithms/data_structures/graph_partition.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 18:22 benchq/algorithms/gsee/__init__.py
+-rw-r--r--  2.0 unx     4415 b- defN 24-Apr-17 18:22 benchq/algorithms/gsee/ld_gsee.py
+-rw-r--r--  2.0 unx     1151 b- defN 24-Apr-17 18:22 benchq/algorithms/gsee/qpe_gsee.py
+-rw-r--r--  2.0 unx      785 b- defN 24-Apr-17 18:22 benchq/compilation/__init__.py
+-rw-r--r--  2.0 unx     4524 b- defN 24-Apr-17 18:22 benchq/compilation/graph_sim_data.jl
+-rw-r--r--  2.0 unx     1855 b- defN 24-Apr-17 18:22 benchq/compilation/initialize_julia.py
+-rw-r--r--  2.0 unx     3106 b- defN 24-Apr-17 18:22 benchq/compilation/jabalizer_wrapper.jl
+-rw-r--r--  2.0 unx     2367 b- defN 24-Apr-17 18:22 benchq/compilation/julia_utils.py
+-rw-r--r--  2.0 unx     3268 b- defN 24-Apr-17 18:22 benchq/compilation/pyliqtr_transpilation.py
+-rw-r--r--  2.0 unx    17502 b- defN 24-Apr-17 18:22 benchq/compilation/rbs_hyperparam_tuning.py
+-rw-r--r--  2.0 unx    22742 b- defN 24-Apr-17 18:22 benchq/compilation/ruby_slippers.jl
+-rw-r--r--  2.0 unx     9527 b- defN 24-Apr-17 18:22 benchq/compilation/transpile_to_native_gates.py
+-rw-r--r--  2.0 unx      371 b- defN 24-Apr-17 18:22 benchq/conversions/__init__.py
+-rw-r--r--  2.0 unx     2169 b- defN 24-Apr-17 18:22 benchq/conversions/_circuit_translations.py
+-rw-r--r--  2.0 unx     1266 b- defN 24-Apr-17 18:22 benchq/conversions/_openfermion_pyliqtr.py
+-rw-r--r--  2.0 unx       34 b- defN 24-Apr-17 18:22 benchq/decoder_modeling/__init__.py
+-rw-r--r--  2.0 unx     4308 b- defN 24-Apr-17 18:22 benchq/decoder_modeling/decoder.py
+-rw-r--r--  2.0 unx     3746 b- defN 24-Apr-17 18:22 benchq/decoder_modeling/decoder_resource_estimator.py
+-rw-r--r--  2.0 unx      162 b- defN 24-Apr-17 18:22 benchq/magic_state_distillation/__init__.py
+-rw-r--r--  2.0 unx     4215 b- defN 24-Apr-17 18:22 benchq/magic_state_distillation/autoccz_factories.py
+-rw-r--r--  2.0 unx     2203 b- defN 24-Apr-17 18:22 benchq/magic_state_distillation/litinski_factories.py
+-rw-r--r--  2.0 unx      299 b- defN 24-Apr-17 18:22 benchq/magic_state_distillation/magic_state_factory.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 18:22 benchq/mlflow/__init__.py
+-rw-r--r--  2.0 unx     3650 b- defN 24-Apr-17 18:22 benchq/mlflow/data_logging.py
+-rw-r--r--  2.0 unx      397 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/__init__.py
+-rw-r--r--  2.0 unx     2286 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/_qaoa.py
+-rw-r--r--  2.0 unx     1169 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/_trotter.py
+-rw-r--r--  2.0 unx     5229 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/qpe.py
+-rw-r--r--  2.0 unx     4081 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/quantum_program.py
+-rw-r--r--  2.0 unx     3198 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/block_encodings/double_factorized_hamiltonian.py
+-rw-r--r--  2.0 unx     2044 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/block_encodings/offset_tridiagonal.py
+-rw-r--r--  2.0 unx     3939 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/block_encodings/offset_tridiagonal_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/qsp/__init__.py
+-rw-r--r--  2.0 unx     5017 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/qsp/_lin_and_dong_qsp.py
+-rw-r--r--  2.0 unx    10329 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/qsp/_qsp.py
+-rw-r--r--  2.0 unx    15077 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/qsp/get_qsp_phases.py
+-rw-r--r--  2.0 unx     4694 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/qsp/get_qsp_polynomial.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/time_marching/__init__.py
+-rw-r--r--  2.0 unx    11598 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/time_marching/_time_marching.py
+-rw-r--r--  2.0 unx      550 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/time_marching/compression_gadget.py
+-rw-r--r--  2.0 unx     2605 b- defN 24-Apr-17 18:22 benchq/problem_embeddings/time_marching/matrix_properties.py
+-rw-r--r--  2.0 unx      483 b- defN 24-Apr-17 18:22 benchq/problem_ingestion/__init__.py
+-rw-r--r--  2.0 unx     6942 b- defN 24-Apr-17 18:22 benchq/problem_ingestion/hamiltonian_from_file.py
+-rw-r--r--  2.0 unx      510 b- defN 24-Apr-17 18:22 benchq/problem_ingestion/molecular_hamiltonians/__init__.py
+-rw-r--r--  2.0 unx     3212 b- defN 24-Apr-17 18:22 benchq/problem_ingestion/molecular_hamiltonians/_common_molecules.py
+-rw-r--r--  2.0 unx     2775 b- defN 24-Apr-17 18:22 benchq/problem_ingestion/molecular_hamiltonians/_compute_lambda.py
+-rw-r--r--  2.0 unx    20976 b- defN 24-Apr-17 18:22 benchq/problem_ingestion/molecular_hamiltonians/_hamiltonian_generation.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 18:22 benchq/problem_ingestion/plasma_hamiltonians/__init__.py
+-rw-r--r--  2.0 unx      887 b- defN 24-Apr-17 18:22 benchq/problem_ingestion/plasma_hamiltonians/vlasov.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 18:22 benchq/problem_ingestion/solid_state_hamiltonians/__init__.py
+-rw-r--r--  2.0 unx      872 b- defN 24-Apr-17 18:22 benchq/problem_ingestion/solid_state_hamiltonians/fermi_hubbard.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-Apr-17 18:22 benchq/problem_ingestion/solid_state_hamiltonians/heisenberg.py
+-rw-r--r--  2.0 unx     4267 b- defN 24-Apr-17 18:22 benchq/problem_ingestion/solid_state_hamiltonians/ising.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Apr-17 18:22 benchq/quantum_hardware_modeling/__init__.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-Apr-17 18:22 benchq/quantum_hardware_modeling/devitt_surface_code.py
+-rw-r--r--  2.0 unx      892 b- defN 24-Apr-17 18:22 benchq/quantum_hardware_modeling/fowler_surface_code.py
+-rw-r--r--  2.0 unx     9024 b- defN 24-Apr-17 18:22 benchq/quantum_hardware_modeling/hardware_architecture_models.py
+-rw-r--r--  2.0 unx      204 b- defN 24-Apr-17 18:22 benchq/resource_estimators/__init__.py
+-rw-r--r--  2.0 unx     4985 b- defN 24-Apr-17 18:22 benchq/resource_estimators/azure_estimator.py
+-rw-r--r--  2.0 unx    12376 b- defN 24-Apr-17 18:22 benchq/resource_estimators/default_estimators.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-Apr-17 18:22 benchq/resource_estimators/resource_info.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-17 18:22 benchq/resource_estimators/footprint_estimators/__init__.py
+-rw-r--r--  2.0 unx     8985 b- defN 24-Apr-17 18:22 benchq/resource_estimators/footprint_estimators/openfermion_estimator.py
+-rw-r--r--  2.0 unx      707 b- defN 24-Apr-17 18:22 benchq/resource_estimators/graph_estimators/__init__.py
+-rw-r--r--  2.0 unx     3984 b- defN 24-Apr-17 18:22 benchq/resource_estimators/graph_estimators/customizable_pipelines.py
+-rw-r--r--  2.0 unx     8723 b- defN 24-Apr-17 18:22 benchq/resource_estimators/graph_estimators/extrapolation_estimator.py
+-rw-r--r--  2.0 unx    18493 b- defN 24-Apr-17 18:22 benchq/resource_estimators/graph_estimators/graph_estimator.py
+-rw-r--r--  2.0 unx     4908 b- defN 24-Apr-17 18:22 benchq/resource_estimators/graph_estimators/transformers.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-17 18:22 benchq-0.7.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7465 b- defN 24-Apr-17 18:22 benchq-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 18:22 benchq-0.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-17 18:22 benchq-0.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     8497 b- defN 24-Apr-17 18:22 benchq-0.7.0.dist-info/RECORD
+83 files, 330829 bytes uncompressed, 94292 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -1,50 +1,44 @@
 Filename: benchq/__init__.py
 Comment: 
 
 Filename: benchq/timing.py
 Comment: 
 
-Filename: benchq/vizualization_tools.py
+Filename: benchq/visualization_tools.py
 Comment: 
 
 Filename: benchq/algorithms/__init__.py
 Comment: 
 
-Filename: benchq/algorithms/gsee.py
+Filename: benchq/algorithms/profolio_optimization.py
 Comment: 
 
-Filename: benchq/algorithms/ld_gsee.py
-Comment: 
-
-Filename: benchq/algorithms/lde_solver.py
-Comment: 
-
-Filename: benchq/algorithms/lin_and_dong_qsp.py
+Filename: benchq/algorithms/time_evolution.py
 Comment: 
 
-Filename: benchq/algorithms/qaoa.py
+Filename: benchq/algorithms/data_structures/__init__.py
 Comment: 
 
-Filename: benchq/algorithms/time_evolution.py
+Filename: benchq/algorithms/data_structures/algorithm_implementation.py
 Comment: 
 
-Filename: benchq/algorithms/utils/compression_gadget.py
+Filename: benchq/algorithms/data_structures/error_budget.py
 Comment: 
 
-Filename: benchq/algorithms/utils/convex_optimization.py
+Filename: benchq/algorithms/data_structures/graph_partition.py
 Comment: 
 
-Filename: benchq/algorithms/utils/qsp_solver.py
+Filename: benchq/algorithms/gsee/__init__.py
 Comment: 
 
-Filename: benchq/block_encodings/block_encoding_utils.py
+Filename: benchq/algorithms/gsee/ld_gsee.py
 Comment: 
 
-Filename: benchq/block_encodings/offset_tridiagonal.py
+Filename: benchq/algorithms/gsee/qpe_gsee.py
 Comment: 
 
 Filename: benchq/compilation/__init__.py
 Comment: 
 
 Filename: benchq/compilation/graph_sim_data.jl
 Comment: 
@@ -75,122 +69,182 @@
 
 Filename: benchq/conversions/_circuit_translations.py
 Comment: 
 
 Filename: benchq/conversions/_openfermion_pyliqtr.py
 Comment: 
 
-Filename: benchq/data_structures/__init__.py
+Filename: benchq/decoder_modeling/__init__.py
 Comment: 
 
-Filename: benchq/data_structures/algorithm_implementation.py
+Filename: benchq/decoder_modeling/decoder.py
 Comment: 
 
-Filename: benchq/data_structures/decoder.py
+Filename: benchq/decoder_modeling/decoder_resource_estimator.py
 Comment: 
 
-Filename: benchq/data_structures/error_budget.py
+Filename: benchq/magic_state_distillation/__init__.py
 Comment: 
 
-Filename: benchq/data_structures/graph_partition.py
+Filename: benchq/magic_state_distillation/autoccz_factories.py
 Comment: 
 
-Filename: benchq/data_structures/hardware_architecture_models.py
+Filename: benchq/magic_state_distillation/litinski_factories.py
 Comment: 
 
-Filename: benchq/data_structures/quantum_program.py
-Comment: 
-
-Filename: benchq/data_structures/resource_info.py
+Filename: benchq/magic_state_distillation/magic_state_factory.py
 Comment: 
 
 Filename: benchq/mlflow/__init__.py
 Comment: 
 
 Filename: benchq/mlflow/data_logging.py
 Comment: 
 
 Filename: benchq/problem_embeddings/__init__.py
 Comment: 
 
-Filename: benchq/problem_embeddings/_qsp.py
+Filename: benchq/problem_embeddings/_qaoa.py
 Comment: 
 
-Filename: benchq/problem_embeddings/_taylorization_lcu.py
+Filename: benchq/problem_embeddings/_trotter.py
 Comment: 
 
-Filename: benchq/problem_embeddings/_trotter.py
+Filename: benchq/problem_embeddings/qpe.py
+Comment: 
+
+Filename: benchq/problem_embeddings/quantum_program.py
+Comment: 
+
+Filename: benchq/problem_embeddings/block_encodings/double_factorized_hamiltonian.py
+Comment: 
+
+Filename: benchq/problem_embeddings/block_encodings/offset_tridiagonal.py
+Comment: 
+
+Filename: benchq/problem_embeddings/block_encodings/offset_tridiagonal_utils.py
+Comment: 
+
+Filename: benchq/problem_embeddings/qsp/__init__.py
+Comment: 
+
+Filename: benchq/problem_embeddings/qsp/_lin_and_dong_qsp.py
+Comment: 
+
+Filename: benchq/problem_embeddings/qsp/_qsp.py
+Comment: 
+
+Filename: benchq/problem_embeddings/qsp/get_qsp_phases.py
+Comment: 
+
+Filename: benchq/problem_embeddings/qsp/get_qsp_polynomial.py
+Comment: 
+
+Filename: benchq/problem_embeddings/time_marching/__init__.py
+Comment: 
+
+Filename: benchq/problem_embeddings/time_marching/_time_marching.py
+Comment: 
+
+Filename: benchq/problem_embeddings/time_marching/compression_gadget.py
+Comment: 
+
+Filename: benchq/problem_embeddings/time_marching/matrix_properties.py
 Comment: 
 
 Filename: benchq/problem_ingestion/__init__.py
 Comment: 
 
 Filename: benchq/problem_ingestion/hamiltonian_from_file.py
 Comment: 
 
-Filename: benchq/problem_ingestion/hamiltonian_generation.py
+Filename: benchq/problem_ingestion/molecular_hamiltonians/__init__.py
+Comment: 
+
+Filename: benchq/problem_ingestion/molecular_hamiltonians/_common_molecules.py
+Comment: 
+
+Filename: benchq/problem_ingestion/molecular_hamiltonians/_compute_lambda.py
+Comment: 
+
+Filename: benchq/problem_ingestion/molecular_hamiltonians/_hamiltonian_generation.py
+Comment: 
+
+Filename: benchq/problem_ingestion/plasma_hamiltonians/__init__.py
+Comment: 
+
+Filename: benchq/problem_ingestion/plasma_hamiltonians/vlasov.py
+Comment: 
+
+Filename: benchq/problem_ingestion/solid_state_hamiltonians/__init__.py
+Comment: 
+
+Filename: benchq/problem_ingestion/solid_state_hamiltonians/fermi_hubbard.py
+Comment: 
+
+Filename: benchq/problem_ingestion/solid_state_hamiltonians/heisenberg.py
 Comment: 
 
-Filename: benchq/problem_ingestion/molecule_instance_generation.py
+Filename: benchq/problem_ingestion/solid_state_hamiltonians/ising.py
 Comment: 
 
-Filename: benchq/problem_ingestion/vlasov.py
+Filename: benchq/quantum_hardware_modeling/__init__.py
 Comment: 
 
-Filename: benchq/resource_estimation/__init__.py
+Filename: benchq/quantum_hardware_modeling/devitt_surface_code.py
 Comment: 
 
-Filename: benchq/resource_estimation/_compute_lambda.py
+Filename: benchq/quantum_hardware_modeling/fowler_surface_code.py
 Comment: 
 
-Filename: benchq/resource_estimation/_footprint_analysis.py
+Filename: benchq/quantum_hardware_modeling/hardware_architecture_models.py
 Comment: 
 
-Filename: benchq/resource_estimation/azure.py
+Filename: benchq/resource_estimators/__init__.py
 Comment: 
 
-Filename: benchq/resource_estimation/decoder_resource_estimator.py
+Filename: benchq/resource_estimators/azure_estimator.py
 Comment: 
 
-Filename: benchq/resource_estimation/default_pipelines.py
+Filename: benchq/resource_estimators/default_estimators.py
 Comment: 
 
-Filename: benchq/resource_estimation/magic_state_distillation.py
+Filename: benchq/resource_estimators/resource_info.py
 Comment: 
 
-Filename: benchq/resource_estimation/openfermion_re.py
+Filename: benchq/resource_estimators/footprint_estimators/__init__.py
 Comment: 
 
-Filename: benchq/resource_estimation/graph/__init__.py
+Filename: benchq/resource_estimators/footprint_estimators/openfermion_estimator.py
 Comment: 
 
-Filename: benchq/resource_estimation/graph/customizable_pipelines.py
+Filename: benchq/resource_estimators/graph_estimators/__init__.py
 Comment: 
 
-Filename: benchq/resource_estimation/graph/extrapolation_estimator.py
+Filename: benchq/resource_estimators/graph_estimators/customizable_pipelines.py
 Comment: 
 
-Filename: benchq/resource_estimation/graph/graph_estimator.py
+Filename: benchq/resource_estimators/graph_estimators/extrapolation_estimator.py
 Comment: 
 
-Filename: benchq/resource_estimation/graph/transformers.py
+Filename: benchq/resource_estimators/graph_estimators/graph_estimator.py
 Comment: 
 
-Filename: benchq/resource_estimation/graph/worstcase_footprint_estimator.py
+Filename: benchq/resource_estimators/graph_estimators/transformers.py
 Comment: 
 
-Filename: benchq-0.6.0.dist-info/LICENSE
+Filename: benchq-0.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: benchq-0.6.0.dist-info/METADATA
+Filename: benchq-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: benchq-0.6.0.dist-info/WHEEL
+Filename: benchq-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: benchq-0.6.0.dist-info/top_level.txt
+Filename: benchq-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: benchq-0.6.0.dist-info/RECORD
+Filename: benchq-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchq/__init__.py

```diff
@@ -1,14 +1,8 @@
 ################################################################################
 # © Copyright 2022 Zapata Computing Inc.
 ################################################################################
-from .data_structures import (
-    AlgorithmImplementation,
-    BasicArchitectureModel,
-    QuantumProgram,
-    get_algorithm_implementation_from_circuit,
-    get_program_from_circuit,
-)
-from .data_structures.hardware_architecture_models import (
+
+from .quantum_hardware_modeling.hardware_architecture_models import (
     BASIC_ION_TRAP_ARCHITECTURE_MODEL,
     BASIC_SC_ARCHITECTURE_MODEL,
 )
```

## benchq/algorithms/__init__.py

```diff
@@ -1,9 +0,0 @@
-00000000: 6672 6f6d 202e 7161 6f61 2069 6d70 6f72  from .qaoa impor
-00000010: 7420 7161 6f61 5f61 6c67 6f72 6974 686d  t qaoa_algorithm
-00000020: 0a66 726f 6d20 2e74 696d 655f 6576 6f6c  .from .time_evol
-00000030: 7574 696f 6e20 696d 706f 7274 2028 0a20  ution import (. 
-00000040: 2020 2071 7370 5f74 696d 655f 6576 6f6c     qsp_time_evol
-00000050: 7574 696f 6e5f 616c 676f 7269 7468 6d2c  ution_algorithm,
-00000060: 0a20 2020 2074 726f 7474 6572 5f74 696d  .    trotter_tim
-00000070: 655f 6576 6f6c 7574 696f 6e5f 616c 676f  e_evolution_algo
-00000080: 7269 7468 6d2c 0a29 0a                   rithm,.).
```

## benchq/algorithms/time_evolution.py

```diff
@@ -1,14 +1,16 @@
 import numpy as np
-from orquestra.integrations.cirq.conversions import to_openfermion
+from orquestra.integrations.cirq.conversions import (
+    to_openfermion,  # pyright: ignore[reportPrivateImportUsage]
+)
 from orquestra.quantum.operators import PauliRepresentation
 from pyLIQTR.QSP import gen_qsp
 
+from ..algorithms.data_structures import AlgorithmImplementation, ErrorBudget
 from ..conversions import openfermion_to_pyliqtr
-from ..data_structures import AlgorithmImplementation, ErrorBudget
 from ..problem_embeddings import get_qsp_program, get_trotter_program
 
 
 # TODO: This logic is copied from pyLIQTR, perhaps we want to change it to our own?
 def _get_steps(tau, req_prec):
     # have tau and epsilon, backtrack in order to get steps
     steps, closeval = gen_qsp.get_steps_from_logeps(np.log(req_prec), tau, 1)
```

## benchq/compilation/pyliqtr_transpilation.py

```diff
@@ -1,10 +1,11 @@
 ################################################################################
 # © Copyright 2022 Zapata Computing Inc.
 ################################################################################
+import warnings
 from typing import Optional, Union
 
 from cirq.circuits import Circuit as CirqCircuit
 from orquestra.quantum.circuits import Circuit as OrquestraCircuit
 from orquestra.quantum.circuits import GateOperation
 from pyLIQTR.gate_decomp.cirq_transforms import clifford_plus_t_direct_transform
 from qiskit.circuit import QuantumCircuit as QiskitCircuit
@@ -52,16 +53,20 @@
         raise ValueError(
             "Please supply precision either for the gates or for the circuit"
         )
     if circuit_precision is not None and gate_precision is not None:
         raise ValueError("Please supply gate or circuit precision not both")
 
     cirq_circuit = export_circuit(CirqCircuit, orquestra_circuit)
-    compiled_cirq_circuit = clifford_plus_t_direct_transform(
-        cirq_circuit,
-        precision=gate_precision,
-        circuit_precision=circuit_precision,
-        use_random_decomp=False,
-        num_rotation_gates=n_rotation_gates,
-    )
+    with warnings.catch_warnings():
+        warnings.filterwarnings(
+            "ignore", message=r".* is not a rotation gate, cannot decompose."
+        )
+        compiled_cirq_circuit = clifford_plus_t_direct_transform(
+            cirq_circuit,
+            precision=gate_precision,
+            circuit_precision=circuit_precision,
+            use_random_decomp=False,
+            num_rotation_gates=n_rotation_gates,
+        )
 
     return import_circuit(compiled_cirq_circuit, orquestra_circuit.n_qubits)
```

## benchq/compilation/rbs_hyperparam_tuning.py

```diff
@@ -1,19 +1,17 @@
 from math import ceil
 
 import networkx as nx
 import optuna
 from orquestra.quantum.circuits import Circuit, H
 
-from ..data_structures import (
-    BASIC_SC_ARCHITECTURE_MODEL,
-    GraphPartition,
-    QuantumProgram,
-)
-from ..resource_estimation.graph import GraphResourceEstimator
+from ..algorithms.data_structures import GraphPartition
+from ..problem_embeddings.quantum_program import QuantumProgram
+from ..quantum_hardware_modeling import BASIC_SC_ARCHITECTURE_MODEL
+from ..resource_estimators.graph_estimators import GraphResourceEstimator
 from . import jl, transpile_to_native_gates
 from .julia_utils import get_nx_graph_from_rbs_adj_list
 
 
 def space_time_cost_from_rbs(
     rbs_iteration_time: float,
     max_allowed_time: float,
```

## benchq/compilation/transpile_to_native_gates.py

```diff
@@ -125,15 +125,15 @@
         theta = operation.params[0]
 
         gate_decomposition = [H, RZ(theta), H]
 
         def preprocess_gate(gate):
             return (
                 gate.controlled(operation.gate.num_control_qubits)
-                if operation.gate.name == "Control"
+                if isinstance(operation.gate, ControlledGate)
                 else gate
             )
 
         gate_operation_decomposition = [
             preprocess_gate(gate)(*operation.qubit_indices)
             for gate in gate_decomposition
         ]
@@ -156,15 +156,15 @@
         theta = operation.params[0]
 
         gate_decomposition = [Dagger(S), H, RZ(theta), H, S]
 
         def preprocess_gate(gate):
             return (
                 gate.controlled(operation.gate.num_control_qubits)
-                if operation.gate.name == "Control"
+                if isinstance(operation.gate, ControlledGate)
                 else gate
             )
 
         gate_operation_decomposition = [
             preprocess_gate(gate)(*operation.qubit_indices)
             for gate in gate_decomposition
         ]
@@ -198,15 +198,15 @@
             SX,
             RZ(lam),
         ]
 
         def preprocess_gate(gate):
             return (
                 gate.controlled(operation.gate.num_control_qubits)
-                if operation.gate.name == "Control"
+                if isinstance(operation.gate, ControlledGate)
                 else gate
             )
 
         gate_operation_decomposition = [
             preprocess_gate(gate)(*operation.qubit_indices)
             for gate in gate_decomposition
         ]
```

## benchq/conversions/__init__.py

```diff
@@ -1,5 +1,5 @@
 ################################################################################
 # © Copyright 2022 Zapata Computing Inc.
 ################################################################################
-from ._circuit_translations import export_circuit, import_circuit, time_evolution
+from ._circuit_translations import SUPPORTED_CIRCUITS, export_circuit, import_circuit
 from ._openfermion_pyliqtr import openfermion_to_pyliqtr, pyliqtr_to_openfermion
```

## benchq/conversions/_circuit_translations.py

```diff
@@ -1,24 +1,24 @@
 ################################################################################
 # © Copyright 2022 Zapata Computing Inc.
 ################################################################################
 from functools import singledispatch
-from typing import Optional
+from typing import Optional, Union
 
 from cirq.circuits import Circuit as CirqCircuit
 from orquestra.integrations.cirq.conversions import export_to_cirq, import_from_cirq
 from orquestra.integrations.qiskit.conversions import (
     export_to_qiskit,
     import_from_qiskit,
 )
 from orquestra.quantum.circuits import Circuit as OrquestraCircuit
-from orquestra.quantum.evolution import time_evolution as old_time_evolution
-from orquestra.quantum.operators import PauliRepresentation
 from qiskit.circuit import QuantumCircuit as QiskitCircuit
 
+SUPPORTED_CIRCUITS = Union[QiskitCircuit, CirqCircuit, OrquestraCircuit]
+
 
 def _reset_n_qubits_if_needed(
     circuit: OrquestraCircuit, original_n_qubits: Optional[int] = None
 ):
     return (
         circuit
         if original_n_qubits is None
@@ -53,39 +53,7 @@
         return circuit
     elif circuit_type == QiskitCircuit:
         return export_to_qiskit(circuit)
     elif circuit_type == CirqCircuit:
         return export_to_cirq(circuit)
     else:
         raise NotImplementedError(f"Circuit type {circuit_type} not supported")
-
-
-def time_evolution(
-    hamiltonian: PauliRepresentation,
-    time: float,
-    method: str = "Trotter",
-    trotter_order: int = 1,
-    circuit_type: type = OrquestraCircuit,
-) -> OrquestraCircuit:
-    """Time evolution of a quantum circuit.
-
-    Args:
-        circuit: The quantum circuit to evolve.
-        hamiltonian: The Hamiltonian to evolve the circuit with.
-        time: The time to evolve the circuit for.
-        num_time_slices: The number of time slices to use.
-        evolution_type: The type of evolution to perform. Defaults to "unitary".
-        backend: The backend to use for the evolution. Defaults to None.
-        **kwargs: Additional keyword arguments to pass to the backend.
-
-    Returns:
-        The evolved quantum circuit.
-    """
-    return export_circuit(
-        circuit_type,
-        old_time_evolution(
-            hamiltonian,
-            time,
-            method,
-            trotter_order,
-        ),
-    )
```

## benchq/mlflow/__init__.py

```diff
@@ -1,18 +0,0 @@
-00000000: 6672 6f6d 202e 6461 7461 5f6c 6f67 6769  from .data_loggi
-00000010: 6e67 2069 6d70 6f72 7420 280a 2020 2020  ng import (.    
-00000020: 5f66 6c61 7474 656e 5f64 6963 742c 0a20  _flatten_dict,. 
-00000030: 2020 2063 7265 6174 655f 6d6c 666c 6f77     create_mlflow
-00000040: 5f73 6366 5f63 616c 6c62 6163 6b2c 0a20  _scf_callback,. 
-00000050: 2020 206c 6f67 5f69 6e70 7574 5f6f 626a     log_input_obj
-00000060: 6563 7473 5f74 6f5f 6d6c 666c 6f77 2c0a  ects_to_mlflow,.
-00000070: 2020 2020 6c6f 675f 7265 736f 7572 6365      log_resource
-00000080: 5f69 6e66 6f5f 746f 5f6d 6c66 6c6f 772c  _info_to_mlflow,
-00000090: 0a29 0a0a 5f5f 616c 6c5f 5f20 3d20 5b0a  .)..__all__ = [.
-000000a0: 2020 2020 226c 6f67 5f69 6e70 7574 5f6f      "log_input_o
-000000b0: 626a 6563 7473 5f74 6f5f 6d6c 666c 6f77  bjects_to_mlflow
-000000c0: 222c 0a20 2020 2022 6c6f 675f 7265 736f  ",.    "log_reso
-000000d0: 7572 6365 5f69 6e66 6f5f 746f 5f6d 6c66  urce_info_to_mlf
-000000e0: 6c6f 7722 2c0a 2020 2020 2263 7265 6174  low",.    "creat
-000000f0: 655f 6d6c 666c 6f77 5f73 6366 5f63 616c  e_mlflow_scf_cal
-00000100: 6c62 6163 6b22 2c0a 2020 2020 225f 666c  lback",.    "_fl
-00000110: 6174 7465 6e5f 6469 6374 222c 0a5d 0a    atten_dict",.].
```

## benchq/mlflow/data_logging.py

```diff
@@ -5,20 +5,18 @@
 from dataclasses import asdict
 from logging import getLogger
 from numbers import Number
 from typing import Any, Callable, Dict, Optional
 
 import mlflow  # type: ignore
 
-from ..data_structures import (
-    AlgorithmImplementation,
-    BasicArchitectureModel,
-    DecoderModel,
-    ResourceInfo,
-)
+from ..algorithms.data_structures import AlgorithmImplementation
+from ..decoder_modeling import DecoderModel
+from ..quantum_hardware_modeling import BasicArchitectureModel
+from ..resource_estimators.resource_info import ResourceInfo
 
 
 def log_input_objects_to_mlflow(
     algorithm_implementation: AlgorithmImplementation,
     algorithm_name: str,
     hardware_model: BasicArchitectureModel,
     decoder_model: Optional[DecoderModel] = None,
@@ -64,15 +62,15 @@
     """
     Callback function for pySCF calculations that also logs to mlflow
 
     In order to make logging to mlflow in parallel work (for instance, parallel
     Orquestra tasks), we need to have started an mlflow Client and a run associated
     with that client that can be passed in.
     For an example of creating the mlflow_client and run_id, see _run_pyscf()
-    in ChemistryApplicationInstance
+    in MolecularHamiltonianGenerator
     """
 
     def scf_callback(vars):
         logger = getLogger(__name__)
         data = {
             "last_hf_e": vars.get("last_hf_e"),
             "norm_gorb": vars.get("norm_gorb"),
```

## benchq/problem_embeddings/__init__.py

```diff
@@ -1,5 +1,6 @@
 ################################################################################
 # © Copyright 2022-2023 Zapata Computing Inc.
 ################################################################################
-from ._qsp import get_qsp_circuit, get_qsp_program
 from ._trotter import get_trotter_circuit, get_trotter_program
+from .qsp._qsp import get_qsp_circuit, get_qsp_program
+from .quantum_program import QuantumProgram, get_program_from_circuit
```

## benchq/problem_embeddings/_trotter.py

```diff
@@ -2,15 +2,15 @@
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 from typing import List
 
 from orquestra.quantum.evolution import time_evolution
 from orquestra.quantum.operators._pauli_operators import PauliRepresentation
 
-from ..data_structures import QuantumProgram
+from .quantum_program import QuantumProgram
 
 
 def get_trotter_circuit(hamiltonian, evolution_time, number_of_steps):
     return time_evolution(hamiltonian, time=evolution_time, n_steps=number_of_steps)
 
 
 def get_trotter_program(
```

## benchq/problem_ingestion/__init__.py

```diff
@@ -1,12 +1,11 @@
 ################################################################################
 # © Copyright 2022-2023 Zapata Computing Inc.
 ################################################################################
 from .hamiltonian_from_file import (
     get_all_hamiltonians_in_folder,
     get_hamiltonian_from_file,
 )
-from .hamiltonian_generation import (
+from .plasma_hamiltonians.vlasov import get_vlasov_hamiltonian
+from .solid_state_hamiltonians.fermi_hubbard import (
     generate_fermi_hubbard_jw_qubit_hamiltonian,
-    generate_jw_qubit_hamiltonian_from_mol_data,
 )
-from .vlasov import get_vlasov_hamiltonian
```

## benchq/problem_ingestion/hamiltonian_from_file.py

```diff
@@ -5,15 +5,15 @@
 import json
 import os
 from typing import List, Union
 
 import h5py
 import numpy as np
 import openfermion as of
-from openfermion import InteractionOperator, jordan_wigner
+from openfermion import InteractionOperator, QubitOperator, jordan_wigner
 from orquestra.integrations.cirq.conversions import from_openfermion
 from orquestra.quantum.operators import PauliSum, PauliTerm
 from orquestra.quantum.utils import ensure_open
 
 
 def get_hamiltonian_from_file(
     file_name: str, allow_unsupported_files=True
@@ -111,15 +111,15 @@
         ValueError: If the file format is not supported
     """
     data = h5py.File(file_name, "r")
 
     if "q_matrix" in data.keys():
         return _qaoa_hamiltonian_from_hdf5(data)
     elif "basis" in data.attrs:
-        return _molecule_hamiltonian_from_hdf5(data)
+        return from_openfermion(_molecule_hamiltonian_from_hdf5(data))
     else:
         raise ValueError(
             f"Hamiltonian extraction failed for {file_name}. "
             f"File format is not recognized. Please use formatting from either "
             f"Guoming Wang's QAOA implementation or Alex Kunitsa's molecule "
             f"implementation."
         )
@@ -161,28 +161,27 @@
             pauli_terms.append(off_diag_pauli_term3)
             pauli_terms.append(off_diag_pauli_term4)
 
     hamiltonian = PauliSum(pauli_terms).simplify()
     return hamiltonian
 
 
-def _molecule_hamiltonian_from_hdf5(data: h5py.File) -> PauliSum:
+def _molecule_hamiltonian_from_hdf5(data: h5py.File) -> QubitOperator:
     """Given a file with a hamiltonian, generate hamiltonian terms corresponding to it.
     This function only accepts hamiltonians in the format with one and two body terms as
     attributes of the hdf5 file.
 
     Args:
-        data (h5py.File): a file with a hamiltonian described by one and two body terms
+        data: A file with a hamiltonian described by one and two body terms.
 
     Returns:
-        PauliSum: the terms of the haimltonian
+        The Jordan-Wigner transformed Hamiltonian.
     """
     one_body_term = data["one_body_tensor"]
     two_body_term = data["two_body_tensor"]
 
     hamiltonian = InteractionOperator(
         constant=data.attrs["constant"],
         one_body_tensor=one_body_term,
         two_body_tensor=two_body_term,
     )
-    hamiltonian = jordan_wigner(hamiltonian)
-    return hamiltonian
+    return jordan_wigner(hamiltonian)
```

## Comparing `benchq/vizualization_tools.py` & `benchq/visualization_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 from typing import List, Optional
 
 import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
 from scipy.optimize import minimize
 
-from .data_structures import ExtrapolatedGraphResourceInfo, ResourceInfo
+from .resource_estimators.resource_info import (
+    ExtrapolatedGraphResourceInfo,
+    ResourceInfo,
+)
 
 
 def plot_graph_state_with_measurement_steps(
     graph_state_graph,
     measurement_steps,
     cmap=plt.cm.rainbow,
     name="extrapolation_plot",
@@ -49,15 +52,15 @@
     exact_info: Optional[ResourceInfo] = None,
 ):
     """Here we allow one to inspect the fits given by extrapolating a problem
     from a smaller number of steps. If exact_info is provided, we also plot the
     exact values for the problem size in green. The extrapolated point is plotted
     in black. The points used to extrapolate are plotted in blue. The fit is plotted
     in red. If the green or black dot is below the red line on the "n_nodes" plot,
-    then we are using a 20-to-4 magic state distillation widget and the "n_nodes"
+    then we are using a 20-to-4 magic state distillation factory and the "n_nodes"
     was cut in 4 to compensate. This is fine because the original number of nodes
     (without the division by 4) will always follow the red line.
     """
     figure, axis = plt.subplots(3, 1)
     figure.tight_layout(pad=1.5)
 
     for i, property in enumerate(
```

## Comparing `benchq/algorithms/gsee.py` & `benchq/algorithms/gsee/qpe_gsee.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import warnings
 
 import numpy as np
-from orquestra.integrations.cirq.conversions import to_openfermion
+from orquestra.integrations.cirq.conversions import (
+    to_openfermion,  # pyright: ignore[reportPrivateImportUsage]
+)
 from orquestra.quantum.operators import PauliRepresentation
 
-from ..conversions import openfermion_to_pyliqtr
-from ..data_structures import AlgorithmImplementation, ErrorBudget
-from ..problem_embeddings import get_qsp_program
+from ...algorithms.data_structures import AlgorithmImplementation, ErrorBudget
+from ...conversions import openfermion_to_pyliqtr
+from ...problem_embeddings import get_qsp_program
 
 
 def _n_block_encodings(hamiltonian: PauliRepresentation, precision: float):
     pyliqtr_operator = openfermion_to_pyliqtr(to_openfermion(hamiltonian))
 
     return int(np.ceil(np.pi * (pyliqtr_operator.alpha) / (precision)))
 
@@ -18,9 +20,9 @@
 def qpe_gsee_algorithm(
     hamiltonian: PauliRepresentation, precision: float, failure_tolerance: float
 ):
     warnings.warn("This is experimental implementation, use at your own risk.")
     n_block_encodings = _n_block_encodings(hamiltonian, precision)
     program = get_qsp_program(hamiltonian, n_block_encodings)
     error_budget = ErrorBudget.from_even_split(failure_tolerance)
-    n_calls = np.ceil(np.log(1 / error_budget.algorithm_failure_tolerance))
-    return AlgorithmImplementation(program, error_budget, n_calls)
+    n_shots = np.ceil(np.log(1 / error_budget.algorithm_failure_tolerance))
+    return AlgorithmImplementation(program, error_budget, n_shots)
```

## Comparing `benchq/algorithms/ld_gsee.py` & `benchq/algorithms/gsee/ld_gsee.py`

 * *Files identical despite different names*

## Comparing `benchq/algorithms/lde_solver.py` & `benchq/problem_embeddings/time_marching/_time_marching.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,86 +11,18 @@
 from orquestra.integrations.qiskit.conversions import (
     export_to_qiskit,
     import_from_qiskit,
 )
 from orquestra.quantum.circuits import PHASE, RZ, SX, Circuit, X
 from qiskit import QuantumCircuit, transpile
 
-from .lin_and_dong_qsp import build_qsp_circuit
-from .utils.compression_gadget import get_add_dagger, get_add_l
-
-
-def get_kappa(matrix_norm: float, time_interval: float) -> float:
-    """Bounds the value of the matrix Xi condition number.
-    kappa <= exp(2||p(A)||),
-    where ||p(A)|| <= time_interval * ||A|| for time independent matrix A.
-
-    Args:
-        matrix_norm (float): Frobenius norm of a matrix A.
-        time_interval (float): time interval of the differential equation.
-
-    Returns:
-        kappa (float): the condition number of Xi.
-    """
-    return np.exp(2 * time_interval * matrix_norm)
-
-
-def get_degree(kappa: float, epsilon: float) -> int:
-    """Calculates an estimation of the degree of an approximating polynomial
-    such that the polynomial is epsilon-close to the desired function f(x) = 1/x
-    (matrix inversion problems).
-
-    The formula is given by the equations (35)-(36) as described in the paper
-    by Y. Dong, X. Meng, K. B. Whaley, and L. Lin.
-    "Efficient Phase Factor Evaluation in Quantum Signal Processing".
-    https://arxiv.org/pdf/2002.11649.pdf
-
-    Note that in this implementation the degree of polynomial is divided
-    by the factor of 3 to reflect a result of a possible improvements
-    by Remez algorithm: https://en.wikipedia.org/wiki/Remez_algorithm
-
-    Args:
-        kappa (float): the condition number of a matrix to be approximated
-            by a polynomial.
-        epsilon (float): a desired precision of the approximation
-            (truncation error).
-
-    Returns:
-        degree (int): the degree of approximating polynomial.
-    """
-
-    b = ceil(kappa**2 * np.log(kappa / epsilon))
-    degree = 2 * ceil(np.sqrt(b * np.log(4 * b / epsilon))) + 1
-
-    return ceil(degree / 3)
-
-
-def get_num_of_grid_points(matrix_norm: float, epsilon: float, beta: float) -> int:
-    """Computes the bound for the number of grid points to approximate
-    the countour integral.
-
-    The formula is derived from the equation (62) as desribed in the paper
-    S. Takahira, A. Ohashi, T. Sogabe, and T. S. Usuda.
-    "Quantum algorithm for matrix functions by Cauchy’s integral formula."
-    https://www.rintonpress.com/journals/doi/QIC20.1-2-2.html
-
-    Args:
-        matrix_norm (float): Frobenius norm of a matrix A.
-        epsilon (float): a desired precision of the approximation.
-        beta (float): bounding parameter of the matrix.
-
-    Returns:
-        num_points (int): the number of grid points.
-    """
-
-    f = (1 - 1 / beta) * matrix_norm / np.exp(matrix_norm)
-    r = beta / matrix_norm
-    num_points = max(1 / (1 - 1 / beta), 1 / (1 - r)) * np.log(8 / f / epsilon + 1)
-
-    return int(num_points)
+from ..qsp._lin_and_dong_qsp import build_qsp_circuit
+from ..quantum_program import QuantumProgram
+from .compression_gadget import get_add_dagger, get_add_l
+from .matrix_properties import get_degree, get_kappa, get_num_of_grid_points
 
 
 def get_prep(grid_point: int, k: int, beta: float) -> Tuple[Circuit, Circuit]:
     """Constructs unitaries that prepare states COEF_k and COEF_k_prime
         corresponding to the z_k.
 
     Args:
@@ -167,15 +99,15 @@
         c_prep_prime += Circuit(
             [X(i) for i in range(n_controlled_qubits) if i not in ones]
         )
 
     return c_prep, c_prep_prime
 
 
-def inverse_blockencoding(
+def inverse_block_encoding(
     be_matrix: Circuit, matrix_norm: float, time: float, beta: float, epsilon: float
 ) -> Circuit:
     """Constructs SEL_inv, an inverse of the block encoding, utilizing the QSP.
     SEL_inv represents the inverse of a single time step evolution of the LDE,
     and is described by 1/(z-z0) as given in the Cauchy's formula for contour integral.
 
     Args:
@@ -291,15 +223,15 @@
         epsilon (float): an accuracy for the polynomial approximation.
 
     Returns:
         matrix_exp (Circuit): a quantum circuit corresponding to
             the approximation exp(A)=f(A).
     """
     prep_int, prep_int_prime = get_prep_int(matrix_norm, beta, epsilon)
-    sel_inverse = inverse_blockencoding(be_matrix, matrix_norm, time, beta, epsilon)
+    sel_inverse = inverse_block_encoding(be_matrix, matrix_norm, time, beta, epsilon)
     # shifting indices
     shifted_prep_int = Circuit(
         [
             op.gate(*[qubit + 1 for qubit in op.qubit_indices])
             for op in prep_int.operations
         ]
     )
@@ -314,24 +246,24 @@
     matrix_exp += shifted_prep_int
     matrix_exp += sel_inverse
     matrix_exp += shifted_prep_dag
 
     return matrix_exp
 
 
-def long_time_propagator(
+def get_time_marching_program(
     phases,
     L: int,
     n: int,
     be_matrix: Circuit,
     matrix_norm: float,
     time: float,
     beta: float,
     epsilon: float,
-) -> Circuit:
+) -> QuantumProgram:
     """Coherently multiply unitaries representing a single time step such that
     the result of the multiplication is the solution to the given differential equation.
     To propagate the differential equation in time with a high probability,
     use the compression gadget and the uniform singular value amplification as
     described in Sections (2.3-2.4) and Appendices (C-D) of the research paper
     (https://arxiv.org/abs/2208.06941).
 
@@ -343,19 +275,17 @@
         be_matrix (Circuit): the block encoding of a matrix.
         matrix_norm (float): the norm of the matrix that is to be block encoded.
         time (float): the time interval one seeks solution for a differntial equation.
         beta (float): an upper bound for the largest eigenvalue of the block encoding.
         epsilon (float): an accuracy for the polynomial approximation.
 
     Return:
-        long_time_propagator (Circuit): an Orquestra.circuit instance representing
+        long_time_propagator (QuantumProgram): an QuantumProgram instance representing
             a quantum circuit for the time-marching algorithm.
     """
-    long_time_propagator = Circuit()
-    long_time_propagator += get_add_l(L)
     qubits_to_shift = ceil(np.log2(L)) + 1
     add_dagger = get_add_dagger(L)
 
     # Assuming a uniform time interval.
     single_time_step = matrix_exponentiation(
         be_matrix, matrix_norm, time, beta, epsilon
     )
@@ -368,15 +298,17 @@
     amplified_shifted = Circuit(
         [
             op.gate(*[qubit + qubits_to_shift for qubit in op.qubit_indices])
             for op in amplified_single_time_step.operations
         ]
     )
 
-    for _ in range(L):
-        long_time_propagator += amplified_shifted
-        num_control_qubits = qsp_qubits - n
-        for q in range(num_control_qubits):
-            control_add_dag = add_dagger.controlled(qubits_to_shift + q)
-        long_time_propagator += control_add_dag
+    short_time_propagator = Circuit()
+    short_time_propagator += amplified_shifted
+    num_control_qubits = qsp_qubits - n
+    for q in range(num_control_qubits):
+        control_add_dag = add_dagger.controlled(qubits_to_shift + q)
+    short_time_propagator += control_add_dag
 
-    return long_time_propagator
+    return QuantumProgram(
+        [get_add_l(L), short_time_propagator], L, lambda x: [0] + [1] * x
+    )
```

## Comparing `benchq/algorithms/lin_and_dong_qsp.py` & `benchq/problem_embeddings/qsp/_lin_and_dong_qsp.py`

 * *Files identical despite different names*

## Comparing `benchq/algorithms/qaoa.py` & `benchq/problem_embeddings/_qaoa.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #####################################################################
 # © Copyright 2023 Zapata Computing Inc.
 ################################################################################
 
 import numpy as np
 from orquestra.quantum.circuits import Circuit
 from orquestra.quantum.operators import PauliSum
-from orquestra.vqa.algorithms import QAOA
+from orquestra.vqa.algorithms.qaoa import QAOA
 
-from ..data_structures import AlgorithmImplementation, ErrorBudget, QuantumProgram
+from .quantum_program import QuantumProgram
 
 
 def get_qaoa_circuit(hamiltonian: PauliSum, n_layers: int = 1) -> Circuit:
     """Given a hamiltonian, generate a QAOA circuit for it. All of the parameters
     describing rotations in the circuit are set to be random. Note: this function
     returns a circuit with different randomized values for each layer, whereas
     get_qaoa_program returns a circuit with the same randomized values for each layer.
@@ -44,16 +44,7 @@
           a QAOA circuit with random parameters for the QUBO instance
     """
 
     qaoa = QAOA.default(cost_hamiltonian=hamiltonian, n_layers=1)
     random_params = np.random.uniform(-np.pi, np.pi, 2)
     circuit = qaoa.get_circuit(random_params)
     return QuantumProgram([circuit], n_layers, lambda x: [0] * x)
-
-
-def qaoa_algorithm(
-    hamiltonian: PauliSum, n_layers: int = 1, failure_tolerance: float = 1e-3
-):
-    program = get_qaoa_program(hamiltonian, n_layers)
-    return AlgorithmImplementation(
-        program, ErrorBudget.from_even_split(failure_tolerance), 1
-    )
```

## Comparing `benchq/algorithms/utils/compression_gadget.py` & `benchq/problem_embeddings/time_marching/compression_gadget.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import math
 
-import numpy as np
 from orquestra.quantum.circuits import Circuit
 
-from benchq.block_encodings.block_encoding_utils import controlled_clock
+from benchq.problem_embeddings.block_encodings.offset_tridiagonal_utils import (
+    controlled_clock,
+)
 
 
 def get_add_l(L) -> Circuit:
     size = math.ceil(math.log2(L)) + 1
     add_l_circuit = Circuit(n_qubits=size)
     for _ in range(L):
         add_l_circuit += controlled_clock(size)
```

## Comparing `benchq/algorithms/utils/convex_optimization.py` & `benchq/problem_embeddings/qsp/get_qsp_polynomial.py`

 * *Files identical despite different names*

## Comparing `benchq/algorithms/utils/qsp_solver.py` & `benchq/problem_embeddings/qsp/get_qsp_phases.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,17 @@
 
             grad[i, 0] /= 2
             obj[i] = 0.5 * np.real(qsp_mat[0, 0] - targetx(x)) ** 2
 
     return grad, obj
 
 
-def qsp_solver(coeff: np.ndarray, parity: int, options: dict) -> Tuple[object, object]:
+def get_qsp_phases(
+    coeff: np.ndarray, parity: int, options: dict
+) -> Tuple[object, object]:
     """Given coefficients of a polynomial P, yield corresponding phase factors.
 
     The reference chose the first half of the phase factors as the
     optimization variables, while in the code we used the second half of the
     phase factors. These two formulations are equivalent.
 
     To simplify the representation, a constant pi/4 is added to both sides of
```

## Comparing `benchq/block_encodings/block_encoding_utils.py` & `benchq/problem_embeddings/block_encodings/offset_tridiagonal_utils.py`

 * *Files identical despite different names*

## Comparing `benchq/block_encodings/offset_tridiagonal.py` & `benchq/problem_embeddings/block_encodings/offset_tridiagonal.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from orquestra.quantum.circuits import RY, Circuit, H
 
-from .block_encoding_utils import controlled_clock, x_conj_gate
+from .offset_tridiagonal_utils import controlled_clock, x_conj_gate
 
 
 def get_offset_tridagonal_block_encoding(
     n: int, a: float, b: float, c: float
 ) -> Circuit:
     """Constructs the block-encoding of the offset tridiagonal matrix with
     parameters a, b, c. The offset tridagonal matrix M looks like:
```

## Comparing `benchq/data_structures/algorithm_implementation.py` & `benchq/algorithms/data_structures/algorithm_implementation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from dataclasses import dataclass
 from typing import Generic, TypeVar
 
-from orquestra.quantum.circuits import Circuit
-
+from ...conversions import SUPPORTED_CIRCUITS, import_circuit
+from ...problem_embeddings import QuantumProgram, get_program_from_circuit
 from .error_budget import ErrorBudget
 from .graph_partition import GraphPartition
-from .quantum_program import QuantumProgram, get_program_from_circuit
 
 T = TypeVar("T", QuantumProgram, GraphPartition)
 
 
 @dataclass
 class AlgorithmImplementation(Generic[T]):
     program: T
     error_budget: ErrorBudget
-    n_calls: int
-
+    n_shots: int
 
-def get_algorithm_implementation_from_circuit(
-    circuit: Circuit, error_budget: ErrorBudget, n_calls: int = 1
-):
-    quantum_program = get_program_from_circuit(circuit)
-    return AlgorithmImplementation(quantum_program, error_budget, n_calls)
+    @classmethod
+    def from_circuit(
+        cls, circuit: SUPPORTED_CIRCUITS, error_budget: ErrorBudget, n_shots: int = 1
+    ):
+        program = get_program_from_circuit(import_circuit(circuit))
+        return AlgorithmImplementation(program, error_budget, n_shots)
```

## Comparing `benchq/data_structures/decoder.py` & `benchq/decoder_modeling/decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,9 +114,8 @@
         if new_d in distances:
             return distances.index(new_d)
     raise ValueError("No higher distance found.")
 
 
 def invalid_code_distance():
     """Returns the delay for invalid code distance."""
-    warnings.warn("Code distance is too high to be decoded.", RuntimeWarning)
     return np.infty
```

## Comparing `benchq/data_structures/error_budget.py` & `benchq/algorithms/data_structures/error_budget.py`

 * *Files identical despite different names*

## Comparing `benchq/data_structures/graph_partition.py` & `benchq/algorithms/data_structures/graph_partition.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List, Union
 
 import networkx as nx
 from cirq.circuits.circuit import Circuit as CirqCircuit
 from orquestra.quantum.circuits import Circuit as OrquestraCircuit
 from qiskit.circuit import QuantumCircuit as QiskitCircuit
 
-from .quantum_program import QuantumProgram
+from ...problem_embeddings.quantum_program import QuantumProgram
 
 AnyCircuit = Union[OrquestraCircuit, CirqCircuit, QiskitCircuit]
 
 
 @dataclass
 class GraphPartition:
     program: QuantumProgram
```

## Comparing `benchq/data_structures/hardware_architecture_models.py` & `benchq/quantum_hardware_modeling/hardware_architecture_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 ################################################################################
 # © Copyright 2022 Zapata Computing Inc.
 ################################################################################
-# WARNING! SIMPLE MODELING AHEAD! ABANDON NUANCE ALL YE WHO ENTER HERE!
-
-
-import warnings
 from dataclasses import dataclass
 from typing import Protocol, runtime_checkable
 
-from .resource_info import DetailedIonTrapResourceInfo, ResourceInfo
+from ..resource_estimators.resource_info import (
+    DetailedIonTrapResourceInfo,
+    ResourceInfo,
+)
 
 
 class BasicArchitectureModel(Protocol):
     """Basic Architecture model meant to serve as a base class for the
     other basic architecture models. WARNING! Running a resource estimate
     with this architecture model will fail as, you need to choose an ION
-    based or SC based model in order to select a proper widget.
+    based or SC based model in order to select a proper factory.
 
     Attributes:
         physical_qubit_error_rate (float): The probability that any given physical
             qubit incurs a pauli error during SPAM, entangling gates, or idling.
             For entangling gates and idles, each physical qubit involved in the
             operation is depolarized with probability 2p/3. For SPAM, a pauli that
             brings the state to an orthogonal state is applied with probability p.
         surface_code_cycle_time_in_seconds (float): The time it takes to run a
             surface code cycle.
     """
 
     @property
     def physical_qubit_error_rate(self) -> float:
-        pass
+        ...
 
     @property
     def surface_code_cycle_time_in_seconds(self) -> float:
-        pass
+        ...
 
 
 @runtime_checkable
 class DetailedArchitectureModel(BasicArchitectureModel, Protocol):
     """DetailedArchitectureModel extends basic one, with the ability to
     calculate detailed hardware estimates."""
 
@@ -64,15 +63,14 @@
 class DetailedIonTrapModel:
     def __init__(
         self,
         physical_qubit_error_rate: float = 1e-4,
         surface_code_cycle_time_in_seconds: float = 1e-3,
     ):
         self.physical_qubit_error_rate = physical_qubit_error_rate
-        # TODO: PJ check with Simon about this number
         self.surface_code_cycle_time_in_seconds = surface_code_cycle_time_in_seconds
 
     def get_hardware_resource_estimates(self, resource_info: ResourceInfo):
         code_distance = resource_info.code_distance
 
         # Compute per-elu values
         (
@@ -98,23 +96,27 @@
         total_num_communication_qubits = num_elus * communication_qubits
         total_num_ions = (
             total_num_memory_qubits
             + total_num_computational_qubits
             + total_num_communication_qubits
         )
         total_num_communication_ports = num_elus * num_communication_ports_per_elu
-        total_elu_power_consumed_in_kW = num_elus * self.power_consumed_per_ELU_in_kW()
-        total_elu_energy_consumed_in_kJ = (
+        total_elu_power_consumed_in_kilowatts = (
+            num_elus * self.power_consumed_per_ELU_in_kilowatts()
+        )
+        total_elu_energy_in_kilojoules = (
             num_elus
-            * self.power_consumed_per_ELU_in_kW()
+            * self.power_consumed_per_ELU_in_kilowatts()
             * resource_info.total_time_in_seconds
         )
 
+        power = self.power_consumed_per_ELU_in_kilowatts()
+
         hardware_resource_estimates = DetailedIonTrapResourceInfo(
-            power_consumed_per_elu_in_kW=self.power_consumed_per_ELU_in_kW(),
+            power_consumed_per_elu_in_kilowatts=power,
             num_communication_ports_per_elu=num_communication_ports_per_elu,
             second_switch_per_elu_necessary=second_switch_per_elu_necessary,
             num_communication_qubits_per_elu=communication_qubits,
             num_memory_qubits_per_elu=memory_qubits,
             num_computational_qubits_per_elu=computational_qubits,
             num_optical_cross_connect_layers=self.num_optical_cross_connect_layers(
                 num_elus,
@@ -126,21 +128,21 @@
             ),
             total_num_ions=total_num_ions,
             total_num_communication_qubits=total_num_communication_qubits,
             total_num_memory_qubits=total_num_memory_qubits,
             total_num_computational_qubits=total_num_computational_qubits,
             total_num_communication_ports=total_num_communication_ports,
             num_elus=num_elus,
-            total_elu_power_consumed_in_kW=total_elu_power_consumed_in_kW,
-            total_elu_energy_consumed_in_kJ=total_elu_energy_consumed_in_kJ,
+            total_elu_power_consumed_in_kilowatts=total_elu_power_consumed_in_kilowatts,
+            total_elu_energy_consumed_in_kilojoules=total_elu_energy_in_kilojoules,
         )
 
         return hardware_resource_estimates
 
-    def power_consumed_per_ELU_in_kW(
+    def power_consumed_per_ELU_in_kilowatts(
         self,
     ):
         # Value reported by IonQ
         return 5.0
 
     def num_communication_qubits_per_ELU(self, code_distance: int):
         # Lookup table generated from simulations of the 3-3-9s protocol by
@@ -230,22 +232,19 @@
         # X - C - X - ... - X
         # Each group of ELU + neighbors needs to be serviced by a single switch
         # (e.g. A, B, C, D) Switches with common ELUs need to be connected by other
         # switches For switches that need to be connected, XXX many of their switches
         # must be used for connecting to connector switches
         # Each switch has 1000 ports
         # Each group of ELU + neighbor has at most 4 ELUs
-        warnings.warn("This output parameter has yet to be implemented.")
-
-        num_OXC_layers = None
 
-        return num_OXC_layers
+        # Not yet implemented
+        return -1
 
     def num_ELUs_per_optical_cross_connect(
         self, code_distance: int, num_communication_qubits: int
     ):
-        warnings.warn("This output parameter has yet to be implemented.")
-        num_ELUs_per_OXC = None
-        return num_ELUs_per_OXC
+        # Not yet implemented
+        return -1
 
 
 DETAILED_ION_TRAP_ARCHITECTURE_MODEL = DetailedIonTrapModel()
```

## Comparing `benchq/data_structures/quantum_program.py` & `benchq/problem_embeddings/quantum_program.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,18 @@
         return recreated_circuit
 
     @property
     def n_rotation_gates(self) -> int:
         return self.count_operations_in_program(["RX", "RY", "RZ"])
 
     @property
+    def n_c_gates(self) -> int:
+        return self.count_operations_in_program(["CZ", "CNOT"])
+
+    @property
     def n_t_gates(self) -> int:
         return self.count_operations_in_program(["T", "Tdag"])
 
     @property
     def min_n_nodes(self) -> int:
         return self.n_t_gates + self.n_rotation_gates + self.subroutines[0].n_qubits
```

## Comparing `benchq/data_structures/resource_info.py` & `benchq/resource_estimators/resource_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,41 +9,41 @@
 TExtra = TypeVar("TExtra")
 
 
 @dataclass
 class DecoderInfo:
     """Information relating the deceoder."""
 
-    total_energy_consumption_in_nanojoules: float
-    power_in_nanowatts: float
+    total_energy_in_joules: float
+    power_in_watts: float
     area_in_micrometers_squared: float
     max_decodable_distance: int = field(repr=False)
 
 
 @dataclass
 class DetailedIonTrapResourceInfo:
     """Info relating to detailed ion trap architecture model resources."""
 
-    power_consumed_per_elu_in_kW: float
+    power_consumed_per_elu_in_kilowatts: float
     num_communication_ports_per_elu: int
     second_switch_per_elu_necessary: bool
     num_communication_qubits_per_elu: int
     num_memory_qubits_per_elu: int
     num_computational_qubits_per_elu: int
     num_optical_cross_connect_layers: int
     num_ELUs_per_optical_cross_connect: int
 
     total_num_ions: int
     total_num_communication_qubits: int
     total_num_memory_qubits: int
     total_num_computational_qubits: int
     total_num_communication_ports: int
     num_elus: int
-    total_elu_power_consumed_in_kW: float
-    total_elu_energy_consumed_in_kJ: float
+    total_elu_power_consumed_in_kilowatts: float
+    total_elu_energy_consumed_in_kilojoules: float
 
 
 @dataclass
 class ResourceInfo(Generic[TExtra]):
     """Generic information about estimated resources with possible extras.
 
     The generic parameter of this class is a type of extra information stored
@@ -57,15 +57,15 @@
 
     code_distance: int
     logical_error_rate: float
     n_logical_qubits: int
     n_physical_qubits: int
     total_time_in_seconds: float
     decoder_info: Optional[DecoderInfo]
-    widget_name: str
+    magic_state_factory_name: str
     routing_to_measurement_volume_ratio: float
     extra: TExtra
     hardware_resource_info: Optional[DetailedIonTrapResourceInfo] = None
 
 
 @dataclass
 class GraphData:
```

## Comparing `benchq/problem_embeddings/_qsp.py` & `benchq/problem_embeddings/qsp/_qsp.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import pyLIQTR.QSP as QSP
 from orquestra.integrations.cirq.conversions import import_from_cirq, to_openfermion
 from orquestra.quantum.circuits import Circuit, GateOperation
 from orquestra.quantum.operators import PauliRepresentation
 from pyLIQTR.QSP import gen_qsp
 from pyLIQTR.QSP.qsp_helpers import qsp_decompose_once
 
-from ..conversions import openfermion_to_pyliqtr
-from ..data_structures import QuantumProgram
+from ...conversions import openfermion_to_pyliqtr
+from ..quantum_program import QuantumProgram
 
 TCircuit = TypeVar("TCircuit")
 
 
 @dataclass
 class QSPComponents(Generic[TCircuit]):
     """Structure to store QSP program components.
@@ -94,15 +94,15 @@
     )
 
 
 def get_qsp_program(
     operator: PauliRepresentation,
     n_block_encodings: int,
     decompose_select_v: bool = True,
-):
+) -> QuantumProgram:
     pyliqtr_operator = openfermion_to_pyliqtr(to_openfermion(operator))
     angles = np.random.random(3)
 
     qsp_generator = QSP.QSP.QSP(
         phis=angles,
         hamiltonian=pyliqtr_operator,
         target_size=pyliqtr_operator.problem_size,
```

## Comparing `benchq/problem_ingestion/molecule_instance_generation.py` & `benchq/problem_ingestion/molecular_hamiltonians/_hamiltonian_generation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,45 @@
 ################################################################################
 # © Copyright 2022 Zapata Computing Inc.
 ################################################################################
 import os
+import warnings
 from copy import deepcopy
 from dataclasses import asdict, dataclass
-from typing import Iterable, List, Optional, Tuple
+from typing import Any, Dict, Iterable, List, Optional, Tuple
 
-import numpy as np
 import openfermion
-import urllib3  # type: ignore
-from mlflow import MlflowClient  # type: ignore
+import urllib3
+from mlflow import MlflowClient
 from openfermion import MolecularData
-from openfermion.resource_estimates.molecule import (
-    avas_active_space,
-    localize,
-    stability,
-)
+
+with warnings.catch_warnings():
+    warnings.filterwarnings(
+        "ignore",
+        message="\n\n"
+        "  `numpy.distutils` is deprecated since NumPy 1.23.0, as a result\n",
+    )
+
+    # we need to disable pyscf GC as it throws around bunch of warnings
+    import pyscf
+
+    pyscf.gto.mole.DISABLE_GC = True
+
+    from openfermion.resource_estimates.molecule import (
+        avas_active_space,
+        localize,
+        stability,
+    )
+
 from openfermionpyscf import PyscfMolecularData
 from openfermionpyscf._run_pyscf import compute_integrals
 from orquestra import sdk
 from pyscf import gto, mp, scf
 
-from ..mlflow import _flatten_dict, create_mlflow_scf_callback
+from ...mlflow.data_logging import _flatten_dict, create_mlflow_scf_callback
 
 
 def truncate_with_avas(
     mean_field_object: scf.hf.SCF,
     ao_list: Optional[Iterable[str]] = None,
     minao: Optional[str] = None,
 ) -> Tuple[gto.Mole, scf.hf.SCF]:
@@ -39,19 +53,27 @@
     """
     mean_field_object.verbose = 4
 
     # make sure wave function is stable before we proceed
     mean_field_object = stability(mean_field_object)
 
     # localize before automatically selecting active space with AVAS
-    mean_field_object = localize(
-        mean_field_object, loc_type="pm"
-    )  # default is loc_type ='pm' (Pipek-Mezey)
 
-    return avas_active_space(mean_field_object, ao_list=ao_list, minao=minao)
+    with warnings.catch_warnings():
+        warnings.filterwarnings(
+            "ignore", message="The 'sym_pos' keyword is deprecated and should be"
+        )
+        mean_field_object = localize(
+            mean_field_object, loc_type="pm"
+        )  # default is loc_type ='pm' (Pipek-Mezey)
+        active_space = avas_active_space(
+            mean_field_object, ao_list=ao_list, minao=minao
+        )
+
+    return active_space
 
 
 def _create_mlflow_setup(
     mlflow_experiment_name: str, orq_workspace_id: str
 ) -> Tuple[MlflowClient, str]:
     client = MlflowClient(
         tracking_uri=sdk.mlflow.get_tracking_uri(workspace_id=orq_workspace_id)
@@ -87,32 +109,24 @@
     active_indices: Optional[Iterable[int]] = None
     freeze_core: Optional[bool] = None
     fno_percentage_occupation_number: Optional[float] = None
     fno_threshold: Optional[float] = None
     fno_n_virtual_natural_orbitals: Optional[int] = None
 
 
-@dataclass(frozen=True)
-class SCFInfo:
-    mol_spec: MoleculeSpecification
-    active_space_spec: ActiveSpaceSpecification
-    scf_options: Optional[dict] = None
-    mlflow_experiment_name: Optional[str] = None
-    orq_workspace_id: Optional[str] = None
-
-
 def _truncate_with_fno(
-    active_space_spec,
+    active_space_spec: ActiveSpaceSpecification,
     molecule: gto.Mole,
     mean_field_object: scf.hf.SCF,
 ) -> Tuple[gto.Mole, scf.hf.SCF]:
     """Truncates a meanfield object by reducing the virtual space using
     the frozen natural orbital (FNO) method.
 
     Args:
+        active_space_spec: The active space specification.
         molecule: The PySCF molecule object.
         mean_field_object: The meanfield object to be truncated.
 
     Returns:
         Tuple whose first element is the PySCF molecule object after FNO
         vertual space reduction and whose second is the meanfield object
         containing the SCF solution.
@@ -169,246 +183,269 @@
     pyscf_molecule.spin = mol_spec.multiplicity - 1
     pyscf_molecule.charge = mol_spec.charge
     pyscf_molecule.symmetry = False
     pyscf_molecule.build()
     return pyscf_molecule
 
 
-def _run_pyscf(scf_info: SCFInfo) -> Tuple[gto.Mole, scf.hf.SCF]:
+def _run_pyscf(
+    mol_spec: MoleculeSpecification,
+    active_space_spec: ActiveSpaceSpecification,
+    scf_options: Optional[Dict[str, Any]] = None,
+    mlflow_experiment_name: Optional[str] = None,
+    orq_workspace_id: Optional[str] = None,
+) -> Tuple[gto.Mole, scf.hf.SCF]:
     """Run an SCF calculation using PySCF and return the results as a meanfield
     object.
 
     Note that this method will apply AVAS but does not account for occupied_indices
     and active_indices.
 
     Args:
-        log_to_mlflow: if supplied, will log metrics from SCF calculation to mlflow
+        mol_spec: The molecule specification.
+        active_space_spec: The active space specification.
+        scf_options: Dictionary with optional parameters to pass to PySCF.
+        mlflow_experiment_name: See MolecularHamiltonianGenerator.
+        orq_workspace_id: See MolecularHamiltonianGenerator.
 
     Returns:
         Tuple whose first element is the PySCF molecule object after AVAS or FNO
             reduction and whose second is the meanfield object containing the SCF
             solution.
 
     Raises:
         SCFConvergenceError: If the SCF calculation does not converge.
+        ValueError: If mlflow_experiment_name is set but orq_workspace_id is not or
+            scf_options contains a "callback" key.
     """
-    molecule = _get_pyscf_molecule(scf_info.mol_spec)
-    mean_field_object = (scf.RHF if scf_info.mol_spec.multiplicity == 1 else scf.ROHF)(
-        molecule
-    )
+    molecule = _get_pyscf_molecule(mol_spec)
+    mean_field_object = (scf.RHF if mol_spec.multiplicity == 1 else scf.ROHF)(molecule)
     mean_field_object.max_memory = 1e6  # set allowed memory high so tests pass
 
-    run_id = None
+    updated_scf_options = {}
+    if scf_options is not None:
+        updated_scf_options.update(scf_options)
 
-    if scf_info.mlflow_experiment_name is not None:
+    if mlflow_experiment_name is not None:
+        if orq_workspace_id is None:
+            raise ValueError(
+                "orq_workspace_id must be set if mlflow_experiment_name is set."
+            )
         os.environ["MLFLOW_TRACKING_TOKEN"] = sdk.mlflow.get_tracking_token()
         urllib3.disable_warnings()
 
-        flat_mol_dict = _flatten_dict(asdict(scf_info.mol_spec))
-        flat_active_dict = _flatten_dict(asdict(scf_info.active_space_spec))
+        flat_mol_dict = _flatten_dict(asdict(mol_spec))
+        flat_active_dict = _flatten_dict(asdict(active_space_spec))
 
-        if scf_info.scf_options is not None:
-            if "callback" in scf_info.scf_options:
-                # we want to log to mlflow, AND we've defined the
-                # callback in scf_options
-                mean_field_object.run(**scf_info.scf_options)
-            else:
-                # we want to log to mlflow, BUT haven't defined the
-                # callback in scf_options
-                if not isinstance(scf_info.orq_workspace_id, str):
-                    raise TypeError(
-                        "orq_workspace_id is not a str, it is "
-                        + str(type(scf_info.orq_workspace_id))
-                        + " Did you remember to pass that in "
-                        "to the ChemistryApplicationInstance?"
-                    )
-                client, run_id = _create_mlflow_setup(
-                    scf_info.mlflow_experiment_name, scf_info.orq_workspace_id
-                )
-
-                for key, val in flat_mol_dict.items():
-                    client.log_param(run_id, key, val)
-                for key, val in flat_active_dict.items():
-                    client.log_param(run_id, key, val)
-                temp_options = deepcopy(scf_info.scf_options)
-                temp_options["callback"] = create_mlflow_scf_callback(client, run_id)
-                mean_field_object.run(**temp_options)
-        else:
-            # we want to log to mlflow, but haven't defined scf_options
-            if not isinstance(scf_info.orq_workspace_id, str):
-                raise TypeError(
-                    "orq_workspace_id is not a str, it is "
-                    + str(type(scf_info.orq_workspace_id))
-                    + " Did you remember to pass that in "
-                    "to the ChemistryApplicationInstance?"
-                )
-            client, run_id = _create_mlflow_setup(
-                scf_info.mlflow_experiment_name, scf_info.orq_workspace_id
+        if scf_options is not None and "callback" in scf_options:
+            raise ValueError(
+                "scf_options should not contain a 'callback' key if"
+                "mlflow_experiment_name is set."
             )
 
-            for key, val in flat_mol_dict.items():
-                client.log_param(run_id, key, val)
-            for key, val in flat_active_dict.items():
-                client.log_param(run_id, key, val)
-            temp_options = {"callback": create_mlflow_scf_callback(client, run_id)}
-            mean_field_object.run(**temp_options)
-    else:
-        if scf_info.scf_options is not None:
-            # we don't want to run on mlflow, but we've specified scf_options
-            mean_field_object.run(**scf_info.scf_options)
-        else:
-            # we don't want to run on mlflow, and haven't specified scf_options
-            mean_field_object.run()
+        client, run_id = _create_mlflow_setup(mlflow_experiment_name, orq_workspace_id)
+
+        for key, val in flat_mol_dict.items():
+            client.log_param(run_id, key, val)
+        for key, val in flat_active_dict.items():
+            client.log_param(run_id, key, val)
+
+        updated_scf_options["callback"] = create_mlflow_scf_callback(client, run_id)
+
+    with warnings.catch_warnings():
+        warnings.filterwarnings(
+            "ignore",
+            message="The 'sym_pos' keyword is deprecated and should be",
+        )
+        mean_field_object.run(**updated_scf_options)
 
     if not mean_field_object.converged:
         raise SCFConvergenceError()
 
-    if (
-        scf_info.active_space_spec.avas_atomic_orbitals
-        or scf_info.active_space_spec.avas_minao
-    ):
+    if active_space_spec.avas_atomic_orbitals or active_space_spec.avas_minao:
         molecule, mean_field_object = truncate_with_avas(
             mean_field_object,
-            scf_info.active_space_spec.avas_atomic_orbitals,
-            scf_info.active_space_spec.avas_minao,
+            active_space_spec.avas_atomic_orbitals,
+            active_space_spec.avas_minao,
         )
     if (
-        scf_info.active_space_spec.fno_percentage_occupation_number
-        or scf_info.active_space_spec.fno_threshold
-        or scf_info.active_space_spec.fno_n_virtual_natural_orbitals
+        active_space_spec.fno_percentage_occupation_number
+        or active_space_spec.fno_threshold
+        or active_space_spec.fno_n_virtual_natural_orbitals
     ):
         molecule, mean_field_object = _truncate_with_fno(
-            scf_info.active_space_spec, molecule, mean_field_object
+            active_space_spec, molecule, mean_field_object
         )
     return molecule, mean_field_object
 
 
-class ActiveSpaceGenerator:
-    def __init__(
-        self,
-        scf_info: SCFInfo,
-    ):
-        self.scf_info = scf_info
+def get_active_space_hamiltonian(
+    mol_spec: MoleculeSpecification,
+    active_space_spec: ActiveSpaceSpecification,
+    scf_options: Optional[Dict[str, Any]] = None,
+    mlflow_experiment_name: Optional[str] = None,
+    orq_workspace_id: Optional[str] = None,
+) -> openfermion.InteractionOperator:
+    """Generate the fermionic Hamiltonian corresponding to the instance's
+    active space.
+
+    The active space will be reduced with AVAS if the instance has AVAS
+    attributes set, and further reduced to the orbitals specified by
+    occupied_indices and active_indices attributes. Alternatively, the active
+    space will be reduced with FNO if the FNO attribute is set.
 
-    def get_active_space_hamiltonian(self) -> openfermion.InteractionOperator:
-        """Generate the fermionic Hamiltonian corresponding to the instance's
-        active space.
+    Args:
+        mol_spec: The molecule specification.
+        active_space_spec: The active space specification.
+        scf_options: Dictionary with optional parameters to pass to PySCF.
+        mlflow_experiment_name: See MolecularHamiltonianGenerator.
+        orq_workspace_id: See MolecularHamiltonianGenerator.
 
-        The active space will be reduced with AVAS if the instance has AVAS
-        attributes set, and further reduced to the orbitals specified by
-        occupied_indices and active_indices attributes. Alternatively, the active
-        space will be reduced with FNO if the FNO attribute is set.
-
-        Returns:
-            The fermionic Hamiltonian corresponding to the instance's active space. Note
-                that the active space will account for both AVAS and the
-                occupied_indices/active_indices attributes.
-
-        Raises:
-            SCFConvergenceError: If the SCF calculation does not converge.
-        """
-
-        molecular_data = self._get_molecular_data()
-        occupied_idx = self.scf_info.active_space_spec.occupied_indices
-
-        if self.scf_info.active_space_spec.freeze_core:
-            n_frozen_core = (
-                mp.MP2(molecular_data._pyscf_data["scf"]).set_frozen().frozen
-            )
-            if n_frozen_core > 0:
-                occupied_idx = list(range(n_frozen_core))
+    Returns:
+        The fermionic Hamiltonian corresponding to the instance's active space. Note
+            that the active space will account for both AVAS and the
+            occupied_indices/active_indices attributes.
 
-        return molecular_data.get_molecular_hamiltonian(
-            occupied_indices=occupied_idx,
-            active_indices=self.scf_info.active_space_spec.active_indices,
-        )
+    Raises:
+        SCFConvergenceError: If the SCF calculation does not converge.
+    """
 
-    def get_active_space_meanfield_object(
-        self,
-    ) -> scf.hf.SCF:
-        """Run an SCF calculation using PySCF and return the results as a meanfield
-        object.
-
-        Currently, this method does not support the occupied_indices and active_indices
-        attributes, as well as the FNO attributes and will raise an exception if they
-        are set.
-
-        Returns:
-            A meanfield object corresponding to the instance's active space, accounting
-                for AVAS.
-
-        Raises:
-            SCFConvergenceError: If the SCF calculation does not converge.
-        """
-        if (
-            self.scf_info.active_space_spec.active_indices
-            or self.scf_info.active_space_spec.occupied_indices
-            or self.scf_info.active_space_spec.fno_percentage_occupation_number
-            or self.scf_info.active_space_spec.fno_threshold
-            or self.scf_info.active_space_spec.fno_n_virtual_natural_orbitals
-        ):
-            raise ValueError(
-                "Generating the meanfield object for application instances with "
-                "active and occupied indices, as well as with the FNO approach  "
-                " is not currently supported."
-            )
-        return _run_pyscf(self.scf_info)[1]
+    molecular_data = _get_molecular_data(
+        mol_spec=mol_spec,
+        active_space_spec=active_space_spec,
+        scf_options=scf_options,
+        mlflow_experiment_name=mlflow_experiment_name,
+        orq_workspace_id=orq_workspace_id,
+    )
+    occupied_idx = active_space_spec.occupied_indices
+
+    if active_space_spec.freeze_core:
+        n_frozen_core = mp.MP2(molecular_data._pyscf_data["scf"]).set_frozen().frozen
+        if n_frozen_core > 0:
+            occupied_idx = list(range(n_frozen_core))
+
+    return molecular_data.get_molecular_hamiltonian(
+        occupied_indices=occupied_idx,
+        active_indices=active_space_spec.active_indices,
+    )
+
+
+def get_active_space_meanfield_object(
+    mol_spec: MoleculeSpecification,
+    active_space_spec: ActiveSpaceSpecification,
+    scf_options: Optional[Dict[str, Any]] = None,
+    mlflow_experiment_name: Optional[str] = None,
+    orq_workspace_id: Optional[str] = None,
+) -> scf.hf.SCF:
+    """Run an SCF calculation using PySCF and return the results as a meanfield
+    object.
+
+    Currently, this method does not support the occupied_indices and active_indices
+    attributes, as well as the FNO attributes and will raise an exception if they
+    are set.
 
-    def _get_molecular_data(self):
-        """Given a PySCF meanfield object and molecule, return a PyscfMolecularData
-        object.
+    Args:
+    mol_spec: The molecule specification.
+    active_space_spec: The active space specification.
+    scf_options: Dictionary with optional parameters to pass to PySCF.
+    mlflow_experiment_name: See MolecularHamiltonianGenerator.
+    orq_workspace_id: See MolecularHamiltonianGenerator.
 
-        Returns:
-            A PyscfMolecularData object corresponding to the meanfield object and
-                molecule.
+    Returns:
+        A meanfield object corresponding to the instance's active space, accounting
+            for AVAS.
 
-        Raises:
-            SCFConvergenceError: If the SCF calculation does not converge.
-        """
-        molecular_data = MolecularData(
-            geometry=self.scf_info.mol_spec.geometry,
-            basis=self.scf_info.mol_spec.basis,
-            multiplicity=self.scf_info.mol_spec.multiplicity,
-            charge=self.scf_info.mol_spec.charge,
+    Raises:
+        SCFConvergenceError: If the SCF calculation does not converge.
+    """
+    if (
+        active_space_spec.active_indices
+        or active_space_spec.occupied_indices
+        or active_space_spec.fno_percentage_occupation_number
+        or active_space_spec.fno_threshold
+        or active_space_spec.fno_n_virtual_natural_orbitals
+    ):
+        raise ValueError(
+            "Generating the meanfield object for application instances with "
+            "active and occupied indices, as well as with the FNO approach  "
+            " is not currently supported."
         )
+    return _run_pyscf(
+        mol_spec=mol_spec,
+        active_space_spec=active_space_spec,
+        scf_options=scf_options,
+        mlflow_experiment_name=mlflow_experiment_name,
+        orq_workspace_id=orq_workspace_id,
+    )[1]
+
+
+def _get_molecular_data(
+    mol_spec: MoleculeSpecification,
+    active_space_spec: ActiveSpaceSpecification,
+    scf_options: Optional[Dict[str, Any]] = None,
+    mlflow_experiment_name: Optional[str] = None,
+    orq_workspace_id: Optional[str] = None,
+) -> PyscfMolecularData:
+    """Given a PySCF meanfield object and molecule, return a PyscfMolecularData
+    object.
 
-        molecule, mean_field_object = _run_pyscf(self.scf_info)
-        molecular_data.n_orbitals = int(molecule.nao)
-        molecular_data.n_qubits = 2 * molecular_data.n_orbitals
-        molecular_data.nuclear_repulsion = float(molecule.energy_nuc())
+    Returns:
+        A PyscfMolecularData object corresponding to the meanfield object and
+            molecule.
 
-        molecular_data.hf_energy = float(mean_field_object.e_tot)
+    Raises:
+        SCFConvergenceError: If the SCF calculation does not converge.
+    """
+    molecular_data = MolecularData(
+        geometry=mol_spec.geometry,
+        basis=mol_spec.basis,
+        multiplicity=mol_spec.multiplicity,
+        charge=mol_spec.charge,
+    )
 
-        molecular_data._pyscf_data = pyscf_data = {}
-        pyscf_data["mol"] = molecule
-        pyscf_data["scf"] = mean_field_object
+    molecule, mean_field_object = _run_pyscf(
+        mol_spec=mol_spec,
+        active_space_spec=active_space_spec,
+        scf_options=scf_options,
+        orq_workspace_id=orq_workspace_id,
+        mlflow_experiment_name=mlflow_experiment_name,
+    )
+    molecular_data.n_orbitals = int(molecule.nao)
+    molecular_data.n_qubits = 2 * molecular_data.n_orbitals
+    molecular_data.nuclear_repulsion = float(molecule.energy_nuc())
+
+    molecular_data.hf_energy = float(mean_field_object.e_tot)
+
+    molecular_data._pyscf_data = {  # type: ignore
+        "mol": molecule,
+        "scf": mean_field_object,
+    }
 
-        molecular_data.canonical_orbitals = mean_field_object.mo_coeff.astype(float)
-        molecular_data.orbital_energies = mean_field_object.mo_energy.astype(float)
+    molecular_data.canonical_orbitals = mean_field_object.mo_coeff.astype(float)
+    molecular_data.orbital_energies = mean_field_object.mo_energy.astype(float)
 
-        one_body_integrals, two_body_integrals = compute_integrals(
-            mean_field_object._eri, mean_field_object
-        )
-        molecular_data.one_body_integrals = one_body_integrals
-        molecular_data.two_body_integrals = two_body_integrals
-        molecular_data.overlap_integrals = mean_field_object.get_ovlp()
+    one_body_integrals, two_body_integrals = compute_integrals(
+        mean_field_object._eri, mean_field_object
+    )
+    molecular_data.one_body_integrals = one_body_integrals
+    molecular_data.two_body_integrals = two_body_integrals
+    molecular_data.overlap_integrals = mean_field_object.get_ovlp()
 
-        pyscf_molecular_data = PyscfMolecularData.__new__(PyscfMolecularData)
-        pyscf_molecular_data.__dict__.update(molecule.__dict__)
+    pyscf_molecular_data = PyscfMolecularData.__new__(PyscfMolecularData)
+    pyscf_molecular_data.__dict__.update(molecule.__dict__)
 
-        return molecular_data
+    return molecular_data
 
 
-class ChemistryApplicationInstance:
-    """Class for representing chemistry application instances.
+class MolecularHamiltonianGenerator:
+    """Class for generating molecular Hamiltonians.
 
-    A chemistry application instance is a specification of how to generate a fermionic
-    Hamiltonian, including information such as the molecular geometry and choice of
-    active space. Note that the active space can be specified in one of the following
-    ways:
+    A class for generating a fermionic Hamiltonian for a given molecular geometry and
+    choice of active space. Note that the active space can be specified in one of the
+    following ways:
 
     1. the use of Atomic Valence Active Space (AVAS),
 
     2. by specifying the indices of the occupied and active orbitals,
 
         If freeze_core option is True, chemical frozen core orbitals
         are choosen for occuped_indicies.
@@ -419,14 +456,21 @@
             - fno_threshold
             - fno_n_virtual_natural_orbitals
         to decide how much virtual space will be kept for the active space.
 
         If freeze_core option is True, chemical frozen core orbitals
         are choosen for occuped_indicies.
 
+    To log PySCF progress after each SCF cycle to MLflow, set mlflow_experiment_name and
+    orq_workspace_id. The workspace must have MLflow enabled, and you must be either
+    logged in to the cluster or running a remote workflow on the cluster. See the
+    `Orquestra documentation <https://docs.orquestra.io/>`_ for more information. Also
+    note that scf_options must not have a "callback" key if mlflow_experiment_name and
+    orq_workspace_id are set.
+
 
     Args:
         geometry: A list of tuples of the form (atom, (x, y, z)) where atom is the
             atom type and (x, y, z) are the coordinates of the atom in Angstroms.
         basis: The basis set to use for the calculation.
         multiplicity: The spin multiplicity of the molecule.
         charge: The charge of the molecule.
@@ -436,24 +480,26 @@
             should be assumed to be fully occupied.
         active_indices: A list of molecular orbitals to include in the active space.
         freeze_core: A boolean specifying whether frozen core orbitals are selected
                     for calculations.
         fno_percentage_occupation_number: Percentage of total occupation number.
         fno_threshold: Threshold on NO occupation numbers.
         fno_n_virtual_natural_orbitals: Number of virtual NOs to keep.
-        scf_options: dictionary with parameters for pySCF calculations
-        mlflow_experiment_name: if supplied, pySCF calculations will be logged to
-            mlflow. See orq_workspace_id also
-        orq_workspace_id: orquestra workspace ID. Required to log mlflow info
+        scf_options: dictionary with parameters for PySCF calculations.
+        mlflow_experiment_name: The name of the MLflow experiment to log PySCF progress
+            to. If a value is provided, then orq_workspace_id also must be provided.
+        orq_workspace_id: The ID of the Orquestra workspace to log PySCF progress to.
+            If a value is provided, then mlflow_experiment_name also must be provided.
     """
 
     mol_spec: MoleculeSpecification
     active_space_spec: ActiveSpaceSpecification
-    scf_info: SCFInfo
-    active_space_gen: ActiveSpaceGenerator
+    scf_options: Optional[Dict[str, Any]]
+    mlflow_experiment_name: Optional[str]
+    orq_workspace_id: Optional[str]
 
     def __init__(
         self,
         geometry: List[Tuple[str, Tuple[float, float, float]]],
         basis: str,
         multiplicity: int,
         charge: int,
@@ -481,102 +527,31 @@
             occupied_indices=occupied_indices,
             active_indices=active_indices,
             freeze_core=freeze_core,
             fno_percentage_occupation_number=fno_percentage_occupation_number,
             fno_threshold=fno_threshold,
             fno_n_virtual_natural_orbitals=fno_n_virtual_natural_orbitals,
         )
-        self.scf_info = SCFInfo(
-            mol_spec=self.mol_spec,
-            active_space_spec=self.active_space_spec,
-            scf_options=scf_options,
-            mlflow_experiment_name=mlflow_experiment_name,
-            orq_workspace_id=orq_workspace_id,
-        )
-        self.active_space_gen = ActiveSpaceGenerator(scf_info=self.scf_info)
+        self.scf_options = scf_options
+        self.mlflow_experiment_name = mlflow_experiment_name
+        self.orq_workspace_id = orq_workspace_id
 
     def get_pyscf_molecule(self) -> gto.Mole:
         return _get_pyscf_molecule(self.mol_spec)
 
     def get_active_space_hamiltonian(self) -> openfermion.InteractionOperator:
-        return self.active_space_gen.get_active_space_hamiltonian()
+        return get_active_space_hamiltonian(
+            mol_spec=self.mol_spec,
+            active_space_spec=self.active_space_spec,
+            scf_options=self.scf_options,
+            mlflow_experiment_name=self.mlflow_experiment_name,
+            orq_workspace_id=self.orq_workspace_id,
+        )
 
     def get_active_space_meanfield_object(self) -> scf.hf.SCF:
-        return self.active_space_gen.get_active_space_meanfield_object()
-
-
-def generate_hydrogen_chain_instance(
-    number_of_hydrogens: int,
-    basis: str = "6-31g",
-    bond_distance: float = 1.3,
-    active_indices: Optional[List[int]] = None,
-    occupied_indices: Optional[List[int]] = None,
-    avas_atomic_orbitals: Optional[List[str]] = None,
-    avas_minao: Optional[str] = None,
-    scf_options: Optional[dict] = None,
-    mlflow_experiment_name: Optional[str] = None,
-    orq_workspace_id: Optional[str] = None,
-) -> ChemistryApplicationInstance:
-    """Generate a hydrogen chain application instance.
-
-    Args:
-        number_of_hydrogens: The number of hydrogen atoms in the chain.
-        basis: The basis set to use for the calculation.
-        bond_distance: The distance between the hydrogen atoms (Angstrom).
-        active_indices: A list of molecular orbitals to include in the active space.
-        occupied_indices: A list of molecular orbitals not in the active space that
-            should be assumed to be fully occupied.
-        avas_atomic_orbitals: A list of atomic orbitals to use for (AVAS).
-        avas_minao: The minimum active orbital to use for AVAS.
-        scf_options: dictionary with parameters for pySCF calculations
-        mlflow_experiment_name: if supplied, pySCF calculations will be logged to
-            mlflow. See orq_workspace_id also
-        orq_workspace_id: orquestra workspace ID. Required to log mlflow info
-    """
-    return ChemistryApplicationInstance(
-        geometry=[("H", (0, 0, i * bond_distance)) for i in range(number_of_hydrogens)],
-        basis=basis,
-        charge=0,
-        multiplicity=number_of_hydrogens % 2 + 1,
-        active_indices=active_indices,
-        occupied_indices=occupied_indices,
-        avas_atomic_orbitals=avas_atomic_orbitals,
-        avas_minao=avas_minao,
-        scf_options=scf_options,
-        mlflow_experiment_name=mlflow_experiment_name,
-        orq_workspace_id=orq_workspace_id,
-    )
-
-
-WATER_MOLECULE = ChemistryApplicationInstance(
-    geometry=[
-        ("O", (0.000000, -0.075791844, 0.000000)),
-        ("H", (0.866811829, 0.601435779, 0.000000)),
-        ("H", (-0.866811829, 0.601435779, 0.000000)),
-    ],
-    basis="6-31g",
-    charge=0,
-    multiplicity=1,
-    avas_atomic_orbitals=["H 1s", "O 2s", "O 2p", "O 3s", "O 3p"],
-    avas_minao="STO-3G",
-)
-
-
-def get_cyclic_ozone_geometry() -> List[Tuple[str, Tuple[float, float, float]]]:
-    """Get the geometry of a cyclic ozone molecule."""
-    bond_len = 1.465  # Angstroms
-    bond_angle = np.deg2rad(59.9)
-
-    x = bond_len * np.sin(bond_angle / 2)
-    y = bond_len * np.cos(bond_angle / 2)
-
-    return [("O", (x, -y / 2, 0)), ("O", (-x, -y / 2, 0)), ("O", (0, y / 2, 0))]
-
-
-CYCLIC_OZONE_MOLECULE = ChemistryApplicationInstance(
-    geometry=get_cyclic_ozone_geometry(),
-    basis="cc-pvtz",
-    multiplicity=3,
-    charge=0,
-    occupied_indices=range(3),
-    active_indices=range(3, 15),
-)
+        return get_active_space_meanfield_object(
+            mol_spec=self.mol_spec,
+            active_space_spec=self.active_space_spec,
+            scf_options=self.scf_options,
+            mlflow_experiment_name=self.mlflow_experiment_name,
+            orq_workspace_id=self.orq_workspace_id,
+        )
```

## Comparing `benchq/problem_ingestion/vlasov.py` & `benchq/problem_ingestion/plasma_hamiltonians/vlasov.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # © Copyright 2022-2023 Zapata Computing Inc.
 ################################################################################
 import pyLIQTR.model_simulators.vlasovsim as vs
 from orquestra.integrations.cirq.conversions import from_openfermion
 from orquestra.quantum.operators import PauliRepresentation
 from pyLIQTR.QSP.Hamiltonian import Hamiltonian as pyliqtrH
 
-from ..conversions import pyliqtr_to_openfermion
+from ...conversions import pyliqtr_to_openfermion
 
 
 def get_vlasov_hamiltonian(
     k: float, alpha: float, nu: float, N: int
 ) -> PauliRepresentation:
     ham_strings = vs.hamiltonian_wfn_vlasov_hermite_linear_sym_string(k, alpha, nu, N)
     qsp_H = pyliqtrH(ham_strings)
```

## Comparing `benchq/resource_estimation/_compute_lambda.py` & `benchq/problem_ingestion/molecular_hamiltonians/_compute_lambda.py`

 * *Files identical despite different names*

## Comparing `benchq/resource_estimation/azure.py` & `benchq/resource_estimators/azure_estimator.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 from typing import Dict, Optional
 
 from azure.quantum.qiskit import AzureQuantumProvider
 from orquestra.integrations.qiskit.conversions import export_to_qiskit
 from orquestra.quantum.circuits import Circuit
 from qiskit.tools.monitor import job_monitor
 
-from ..data_structures import AzureExtra, AzureResourceInfo, BasicArchitectureModel
+from ..algorithms.data_structures import AlgorithmImplementation
+from ..quantum_hardware_modeling import BasicArchitectureModel
+from .resource_info import AzureExtra, AzureResourceInfo
 
 
 def _azure_result_to_resource_info(job_results: dict) -> AzureResourceInfo:
     return AzureResourceInfo(
         n_physical_qubits=job_results["physicalCounts"]["physicalQubits"],
         n_logical_qubits=job_results["physicalCounts"]["breakdown"][
             "algorithmicLogicalQubits"
         ],
         total_time_in_seconds=job_results["physicalCounts"]["runtime_in_s"],
         code_distance=job_results["logicalQubit"]["codeDistance"],
         logical_error_rate=job_results["errorBudget"]["logical"],
         decoder_info=None,
-        widget_name="default",
+        magic_state_factory_name="default",
         routing_to_measurement_volume_ratio=0,
         extra=AzureExtra(
             cycle_time=job_results["logicalQubit"]["logicalCycleTime"],
             depth=job_results["physicalCounts"]["breakdown"]["algorithmicLogicalDepth"],
             raw_data=job_results,
         ),
     )
@@ -61,15 +63,15 @@
                 "currently broken."
             )
         self.hw_model = hw_model
         self.use_full_circuit = use_full_circuit
 
     def estimate(
         self,
-        algorithm,
+        algorithm: AlgorithmImplementation,
     ) -> AzureResourceInfo:
         azure_error_budget: Dict[str, float] = {}
         if algorithm.error_budget is not None:
             azure_error_budget = {}
             azure_error_budget[
                 "rotations"
             ] = algorithm.error_budget.transpilation_failure_tolerance
```

## Comparing `benchq/resource_estimation/decoder_resource_estimator.py` & `benchq/decoder_modeling/decoder_resource_estimator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import warnings
 from typing import Optional
 
-from benchq.data_structures.decoder import DecoderModel
-from benchq.data_structures.hardware_architecture_models import BasicArchitectureModel
-from benchq.data_structures.resource_info import DecoderInfo
+from benchq.decoder_modeling.decoder import DecoderModel
+from benchq.quantum_hardware_modeling.hardware_architecture_models import (
+    BasicArchitectureModel,
+)
+from benchq.resource_estimators.resource_info import DecoderInfo
 
 
 def get_decoder_info(
     hw_model,
     decoder_model: Optional[DecoderModel],
     code_distance: int,
     space_time_volume: float,
@@ -29,34 +31,36 @@
             warnings.warn(
                 f"Code distance {code_distance} is too high to be decoded "
                 "because the decoder is too slow.",
                 RuntimeWarning,
             )
             return None
         else:
-            decoder_total_energy_consumption = (
+            decoder_total_energy_in_joules = (
                 space_time_volume
                 * decoder_model.power_in_nanowatts(code_distance)
                 * decoder_model.delay_in_nanoseconds(code_distance)
-                * 1e-9
+                * 1e-18
             )
-            decoder_power = (
-                2 * n_logical_qubits * decoder_model.power_in_nanowatts(code_distance)
+            decoder_power_in_watts = (
+                n_logical_qubits
+                * decoder_model.power_in_nanowatts(code_distance)
+                * 1e-9
             )
             decoder_area = n_logical_qubits * decoder_model.area_in_micrometers_squared(
                 code_distance
             )
             max_decodable_distance = min(
                 speed_limit,
                 decoder_model.highest_calculated_distance,
             )
 
             return DecoderInfo(
-                total_energy_consumption_in_nanojoules=decoder_total_energy_consumption,
-                power_in_nanowatts=decoder_power,
+                total_energy_in_joules=decoder_total_energy_in_joules,
+                power_in_watts=decoder_power_in_watts,
                 area_in_micrometers_squared=decoder_area,
                 max_decodable_distance=max_decodable_distance,
             )
 
 
 def get_decoder_distance_limit_due_to_speed(
     hw_model: BasicArchitectureModel, decoder_model: DecoderModel, min_d=4, max_d=100
```

## Comparing `benchq/resource_estimation/default_pipelines.py` & `benchq/resource_estimators/default_estimators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 from functools import partial
-from typing import Any, List, Optional
+from typing import List, Optional
 
 import numpy as np
 
+from ..algorithms.data_structures import AlgorithmImplementation
 from ..compilation import get_algorithmic_graph_from_ruby_slippers
-from ..data_structures import (
-    AlgorithmImplementation,
-    DecoderModel,
-    ExtrapolatedGraphResourceInfo,
-    QuantumProgram,
-    ResourceInfo,
+from ..decoder_modeling import DecoderModel
+from ..problem_embeddings.quantum_program import QuantumProgram
+from ..quantum_hardware_modeling.hardware_architecture_models import (
+    BasicArchitectureModel,
 )
-from ..data_structures.hardware_architecture_models import BasicArchitectureModel
-from .graph.customizable_pipelines import (
-    run_custom_extrapolation_pipeline,
-    run_custom_resource_estimation_pipeline,
+from .footprint_estimators.openfermion_estimator import footprint_estimator
+from .graph_estimators.customizable_pipelines import (
+    get_custom_extrapolated_estimate,
+    get_custom_resource_estimation,
 )
-from .graph.extrapolation_estimator import ExtrapolationResourceEstimator
-from .graph.graph_estimator import GraphResourceEstimator
-from .graph.transformers import (
+from .graph_estimators.extrapolation_estimator import ExtrapolationResourceEstimator
+from .graph_estimators.graph_estimator import GraphResourceEstimator
+from .graph_estimators.transformers import (
     create_big_graph_from_subcircuits,
     synthesize_clifford_t,
     transpile_to_native_gates,
 )
-from .openfermion_re import get_physical_cost
+from .resource_info import ExtrapolatedGraphResourceInfo, ResourceInfo
 
-LARGEST_GRAPH_TOLERANCE = 1e8
 DEFAULT_STEPS_TO_EXTRAPOLATE_FROM = [1, 2, 3]
 
 
-def run_precise_graph_estimate(
+def get_precise_graph_estimate(
     algorithm_implementation: AlgorithmImplementation,
     hardware_model: BasicArchitectureModel,
     decoder_model: Optional[DecoderModel] = None,
 ) -> ResourceInfo:
     """Run a slow resource estimate with the lowest amount of resources.
 
     Run a resource estimate by creating a full graph of the full Clifford + T circuit
@@ -51,26 +49,26 @@
             that case.
 
     Returns:
         ResourceInfo: The resources required to run the algorithm.
     """
     estimator = GraphResourceEstimator(hardware_model, decoder_model=decoder_model)
 
-    return run_custom_resource_estimation_pipeline(
+    return get_custom_resource_estimation(
         algorithm_implementation,
         estimator,
         transformers=[
             transpile_to_native_gates,
             synthesize_clifford_t(algorithm_implementation.error_budget),
             create_big_graph_from_subcircuits(),
         ],
     )
 
 
-def run_fast_graph_estimate(
+def get_fast_graph_estimate(
     algorithm_implementation: AlgorithmImplementation,
     hardware_model: BasicArchitectureModel,
     decoder_model: Optional[DecoderModel] = None,
 ) -> ResourceInfo:
     """Run a slow resource estimate that's faster than the precise one.
 
     Run a resource estimate by creating a full graph of the full circuit which is
@@ -89,27 +87,27 @@
             that case.
 
     Returns:
         ResourceInfo: The resources required to run the algorithm.
     """
     estimator = GraphResourceEstimator(hardware_model, decoder_model=decoder_model)
 
-    return run_custom_resource_estimation_pipeline(
+    return get_custom_resource_estimation(
         algorithm_implementation,
         estimator,
         transformers=[
             transpile_to_native_gates,
             create_big_graph_from_subcircuits(
                 graph_production_method=get_algorithmic_graph_from_ruby_slippers,
             ),
         ],
     )
 
 
-def run_precise_extrapolation_estimate(
+def get_precise_extrapolation_estimate(
     algorithm_implementation: AlgorithmImplementation,
     hardware_model: BasicArchitectureModel,
     steps_to_extrapolate_from: List[int],
     decoder_model: Optional[DecoderModel] = None,
     n_measurement_steps_fit_type: str = "logarithmic",
 ) -> ExtrapolatedGraphResourceInfo:
     """Run a faster resource estimate that's based on extrapolating from smaller
@@ -134,26 +132,26 @@
     estimator = ExtrapolationResourceEstimator(
         hardware_model,
         steps_to_extrapolate_from,
         decoder_model=decoder_model,
         n_measurement_steps_fit_type=n_measurement_steps_fit_type,
     )
 
-    return run_custom_extrapolation_pipeline(
+    return get_custom_extrapolated_estimate(
         algorithm_implementation,
         estimator,
         transformers=[
             transpile_to_native_gates,
             synthesize_clifford_t(algorithm_implementation.error_budget),
             create_big_graph_from_subcircuits(),
         ],
     )
 
 
-def run_fast_extrapolation_estimate(
+def get_fast_extrapolation_estimate(
     algorithm_implementation: AlgorithmImplementation,
     hardware_model: BasicArchitectureModel,
     steps_to_extrapolate_from: List[int],
     decoder_model: Optional[DecoderModel] = None,
     n_measurement_steps_fit_type: str = "logarithmic",
 ) -> ExtrapolatedGraphResourceInfo:
     """The fastest resource estimate method, but also the least accurate one.
@@ -178,27 +176,27 @@
     estimator = ExtrapolationResourceEstimator(
         hardware_model,
         steps_to_extrapolate_from,
         decoder_model=decoder_model,
         n_measurement_steps_fit_type=n_measurement_steps_fit_type,
     )
 
-    return run_custom_extrapolation_pipeline(
+    return get_custom_extrapolated_estimate(
         algorithm_implementation,
         estimator,
         transformers=[
             transpile_to_native_gates,
             create_big_graph_from_subcircuits(
                 graph_production_method=get_algorithmic_graph_from_ruby_slippers,
             ),
         ],
     )
 
 
-def run_footprint_analysis_pipeline(
+def get_footprint_estimate(
     algorithm_implementation: AlgorithmImplementation,
     hardware_model: BasicArchitectureModel,
     decoder_model: Optional[DecoderModel] = None,
 ):
     dummy_estimator = GraphResourceEstimator(
         hardware_model, decoder_model=decoder_model
     )
@@ -213,15 +211,15 @@
         algorithm_implementation.error_budget.transpilation_failure_tolerance,
     )
 
     hardware_failure_tolerance = (
         algorithm_implementation.error_budget.hardware_failure_tolerance
     )
 
-    return get_physical_cost(
+    return footprint_estimator(
         algorithm_implementation.program.num_data_qubits,
         num_t=total_t_gates,
         architecture_model=hardware_model,
         hardware_failure_tolerance=hardware_failure_tolerance,
         decoder_model=decoder_model,
     )
 
@@ -229,95 +227,98 @@
 def automatic_resource_estimator(
     algorithm_implementation: AlgorithmImplementation,
     hardware_model: BasicArchitectureModel,
     decoder_model: Optional[DecoderModel] = None,
 ) -> ResourceInfo:
     """Pick the appropriate resource estimator based on the size of the program.
 
-    Currently chooses between GraphResourceEstimator and
-    ExtrapolationResourceEstimator and whether or not to use delayed gate synthesis
+    Currently, chooses between GraphResourceEstimator and
+    ExtrapolationResourceEstimator and whether to use delayed gate synthesis
     in the following order:
         1. GraphResourceEstimator without delayed gate synthesis
-        2. GraphResourceEstimator with delayed gate synthesis
-        3. ExtrapolationResourceEstimator without delayed gate synthesis
+        2. ExtrapolationResourceEstimator without delayed gate synthesis
+        3. GraphResourceEstimator with delayed gate synthesis
         4. ExtrapolationResourceEstimator with delayed gate synthesis
+        5. Footprint estimator as a last-ditch effort
 
+    Decision is based on graph complexity, which is roughly the number
+    of remove_sqs operations one needs to do. Check out Ruby slippers compiler
+    for more details on remove_sqs.
 
     Args:
-        program (QuantumProgram): program to estimate resources for
-        error_budget (ErrorBudget): budget for the error the program can tolerate
-        delayed_gate_synthesis (bool, optional): whether or not to decompose.
-            The gates into clifford + T before creating graph. Defaults to False.
-
-    Raises:
-        ValueError: if the problem is too big to estimate resources for
+        algorithm_implementation (AlgorithmImplementation): The algorithm to estimate
+            resources for.
+        hardware_model (BasicArchitectureModel): The hardware model to estimate
+            resources for.
+        decoder_model (Optional[DecoderModel], optional): The decoder model to
+            run the algorithm with. Defaults to None and returns no estimate in
+            that case.
 
     Returns:
-        GraphResourceEstimator: an appropriate resource estimator for the problem
+        ResourceInfo: The resources required to run the algorithm.
     """
-    pipeline: Any = None
     assert isinstance(algorithm_implementation.program, QuantumProgram)
+    initial_number_of_steps = algorithm_implementation.program.steps
 
-    prev_steps = algorithm_implementation.program.steps
+    graph_size = estimate_full_graph_size(algorithm_implementation, False)
+    reduced_graph_size = estimate_full_graph_size(algorithm_implementation, True)
+
+    # Changing number of steps impacts estimated graph size for extrapolation
     algorithm_implementation.program.steps = max(DEFAULT_STEPS_TO_EXTRAPOLATE_FROM)
-    if (
-        estimate_full_graph_size(algorithm_implementation, True)
-        < LARGEST_GRAPH_TOLERANCE
-    ):
+
+    extrapolaed_graph_size = estimate_full_graph_size(algorithm_implementation, False)
+    small_extrapolated_graph_size = estimate_full_graph_size(
+        algorithm_implementation, True
+    )
+
+    algorithm_implementation.program.steps = initial_number_of_steps
+
+    if graph_size < 1e7:
+        pipeline = get_precise_graph_estimate
+        print("Using precise graph estimator")
+    elif extrapolaed_graph_size < 1e7:
         pipeline = partial(
-            run_fast_extrapolation_estimate,
+            get_precise_extrapolation_estimate,
             steps_to_extrapolate_from=DEFAULT_STEPS_TO_EXTRAPOLATE_FROM,
         )
-    elif (
-        estimate_full_graph_size(algorithm_implementation, False)
-        < LARGEST_GRAPH_TOLERANCE
-    ):
+        print("Using precise extrapolation graph estimator")
+    elif reduced_graph_size < 1e7:
+        pipeline = get_fast_graph_estimate
+        print("Using fast graph estimator")
+    elif small_extrapolated_graph_size < 1e7:
         pipeline = partial(
-            run_precise_extrapolation_estimate,
+            get_fast_extrapolation_estimate,
             steps_to_extrapolate_from=DEFAULT_STEPS_TO_EXTRAPOLATE_FROM,
         )
-
-    algorithm_implementation.program.steps = prev_steps
-    if (
-        estimate_full_graph_size(algorithm_implementation, True)
-        < LARGEST_GRAPH_TOLERANCE
-    ):
-        pipeline = run_fast_graph_estimate
-    if (
-        estimate_full_graph_size(algorithm_implementation, False)
-        < LARGEST_GRAPH_TOLERANCE
-    ):
-        pipeline = run_precise_graph_estimate
-
-    if pipeline is not None:
-        return pipeline(
-            algorithm_implementation,
-            hardware_model,
-            decoder_model=decoder_model,
-        )
+        print("Using fast extrapolation graph estimator")
     else:
-        raise ValueError(
-            "Problem size too large for resource estimation. "
-            "Try reducing the size of each of your steps in the program. "
-            "If you are creating a program from a circuit, consider breaking "
-            "the program up into steps."
-        )
+        pipeline = get_footprint_estimate
+        print("Using footprint analysis estimator")
+
+    return pipeline(
+        algorithm_implementation,
+        hardware_model,
+        decoder_model=decoder_model,
+    )
 
 
 def estimate_full_graph_size(
     algorithm_implementation: AlgorithmImplementation, delayed_gate_synthesis=False
 ) -> int:
-    full_graph_size = algorithm_implementation.program.n_t_gates
+    graph_complexity = (
+        algorithm_implementation.program.n_t_gates
+        + algorithm_implementation.program.n_c_gates * 2
+    )
 
     if not delayed_gate_synthesis:
-        full_graph_size += (
+        graph_complexity += (
             algorithm_implementation.program.n_rotation_gates
             * GraphResourceEstimator.SYNTHESIS_SCALING
             * np.log2(
                 1
                 / algorithm_implementation.error_budget.transpilation_failure_tolerance
             )
         )
     else:
-        full_graph_size += algorithm_implementation.program.n_rotation_gates
+        graph_complexity += algorithm_implementation.program.n_rotation_gates
 
-    return full_graph_size
+    return graph_complexity
```

## Comparing `benchq/resource_estimation/graph/__init__.py` & `benchq/resource_estimators/graph_estimators/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-"""Initialization file for benchq.resource_estimation.v2 subpackage."""
 from .customizable_pipelines import (
-    run_custom_extrapolation_pipeline,
-    run_custom_resource_estimation_pipeline,
+    get_custom_extrapolated_estimate,
+    get_custom_resource_estimation,
 )
 from .extrapolation_estimator import ExtrapolationResourceEstimator
 from .graph_estimator import GraphResourceEstimator, substrate_scheduler
 from .transformers import (
     create_big_graph_from_subcircuits,
     create_graphs_for_subcircuits,
     remove_isolated_nodes,
     synthesize_clifford_t,
     transpile_to_native_gates,
 )
-from .worstcase_footprint_estimator import WorstCaseFootprintResourceEstimator
 
 __all__ = [
-    "run_custom_resource_estimation_pipeline",
-    "run_custom_extrapolation_pipeline",
+    "get_custom_resource_estimation",
+    "get_custom_extrapolated_estimate",
     "synthesize_clifford_t",
     "transpile_to_native_gates",
     "create_big_graph_from_subcircuits",
     "create_graphs_for_subcircuits",
     "GraphResourceEstimator",
 ]
```

## Comparing `benchq/resource_estimation/graph/customizable_pipelines.py` & `benchq/resource_estimators/graph_estimators/customizable_pipelines.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 from copy import deepcopy
 from dataclasses import replace
 from inspect import signature
 from typing import List
 
-from ...data_structures import (
+from ...algorithms.data_structures.algorithm_implementation import (
     AlgorithmImplementation,
-    ExtrapolatedGraphData,
-    ExtrapolatedGraphResourceInfo,
 )
-from ...data_structures.hardware_architecture_models import (
+from ...quantum_hardware_modeling.hardware_architecture_models import (
     BASIC_ION_TRAP_ARCHITECTURE_MODEL,
 )
+from ..resource_info import ExtrapolatedGraphData, ExtrapolatedGraphResourceInfo
 from .extrapolation_estimator import ExtrapolationResourceEstimator
 from .graph_estimator import GraphData, GraphPartition
 
 
-def run_custom_resource_estimation_pipeline(
+def get_custom_resource_estimation(
     algorithm_implementation: AlgorithmImplementation,
     estimator,
     transformers,
 ):
     for transformer in transformers:
         algorithm_implementation = replace(
             algorithm_implementation,
             program=transformer(algorithm_implementation.program),
         )
 
     return estimator.estimate(algorithm_implementation)
 
 
-def _create_extrapolated_graph_data(
+def _get_extrapolated_graph_data(
     algorithm_implementation: AlgorithmImplementation,
     estimator: ExtrapolationResourceEstimator,
     transformers,
 ) -> ExtrapolatedGraphData:
     synthesis_accuracy_for_each_rotation = 1 - (
         1 - algorithm_implementation.error_budget.transpilation_failure_tolerance
     ) ** (1 / algorithm_implementation.program.n_rotation_gates)
@@ -76,39 +75,39 @@
         )
 
     return estimator.get_extrapolated_graph_data(
         small_programs_graph_data, algorithm_implementation.program
     )
 
 
-def create_extrapolated_graph_data_pipeline(
+def get_extrapolated_graph_data(
     algorithm_implementation: AlgorithmImplementation,
     steps_to_extrapolate_from,
     decoder_model,
     transformers,
 ):
     # the architecture model doesn't matter for extrapolating graph data
     dummy_extrapolation_estimator = ExtrapolationResourceEstimator(
         BASIC_ION_TRAP_ARCHITECTURE_MODEL,
         steps_to_extrapolate_from,
         decoder_model=decoder_model,
     )
-    return _create_extrapolated_graph_data(
+    return _get_extrapolated_graph_data(
         algorithm_implementation,
         estimator=dummy_extrapolation_estimator,
         transformers=transformers,
     )
 
 
-def run_custom_extrapolation_pipeline(
+def get_custom_extrapolated_estimate(
     algorithm_implementation: AlgorithmImplementation,
     estimator: ExtrapolationResourceEstimator,
     transformers,
 ) -> ExtrapolatedGraphResourceInfo:
-    extrapolated_graph_data = _create_extrapolated_graph_data(
+    extrapolated_graph_data = _get_extrapolated_graph_data(
         algorithm_implementation, estimator, transformers
     )
 
     return estimator.estimate_given_extrapolation_data(
         algorithm_implementation,
         extrapolated_graph_data,
     )
```

## Comparing `benchq/resource_estimation/graph/extrapolation_estimator.py` & `benchq/resource_estimators/graph_estimators/extrapolation_estimator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from dataclasses import replace
 from math import ceil
 from typing import Iterable, List, Optional
 
 import numpy as np
 from scipy.optimize import minimize
 
-from ...data_structures import (
-    AlgorithmImplementation,
+from ...algorithms.data_structures import AlgorithmImplementation
+from ...decoder_modeling import DecoderModel
+from ...magic_state_distillation import MagicStateFactory
+from ...problem_embeddings.quantum_program import QuantumProgram
+from ...quantum_hardware_modeling.hardware_architecture_models import (
     BasicArchitectureModel,
-    DecoderModel,
+)
+from ...resource_estimators.resource_info import (
     ExtrapolatedGraphData,
     ExtrapolatedGraphResourceInfo,
-    QuantumProgram,
 )
-from ..magic_state_distillation import Widget
 from .graph_estimator import GraphData, GraphResourceEstimator
 
 
 class ExtrapolationResourceEstimator(GraphResourceEstimator):
     """Estimates resources needed to run an algorithm using graph state compilation
     via extrapolating on the number of steps in the algorithm.
 
@@ -35,20 +37,24 @@
     def __init__(
         self,
         hw_model: BasicArchitectureModel,
         steps_to_extrapolate_from: List[int],
         decoder_model: Optional[DecoderModel] = None,
         optimization: str = "space",
         substrate_scheduler_preset: str = "fast",
-        widgets: Optional[Iterable[Widget]] = None,
+        magic_state_factory_iterator: Optional[Iterable[MagicStateFactory]] = None,
         n_measurement_steps_fit_type: str = "logarithmic",
         max_graph_degree_fit_type: str = "logarithmic",
     ):
         super().__init__(
-            hw_model, decoder_model, optimization, substrate_scheduler_preset, widgets
+            hw_model,
+            decoder_model,
+            optimization,
+            substrate_scheduler_preset,
+            magic_state_factory_iterator,
         )
         self.steps_to_extrapolate_from = steps_to_extrapolate_from
         self.n_measurement_steps_fit_type = n_measurement_steps_fit_type
         self.max_graph_degree_fit_type = max_graph_degree_fit_type
 
     def get_extrapolated_graph_data(
         self,
@@ -139,15 +145,15 @@
             n_logical_qubits=resource_info.n_logical_qubits,
             extra=replace(extrapolated_info, n_nodes=resource_info.extra.n_nodes),
             code_distance=resource_info.code_distance,
             logical_error_rate=resource_info.logical_error_rate,
             total_time_in_seconds=resource_info.total_time_in_seconds,
             n_physical_qubits=resource_info.n_physical_qubits,
             decoder_info=resource_info.decoder_info,
-            widget_name=resource_info.widget_name,
+            magic_state_factory_name=resource_info.magic_state_factory_name,
             routing_to_measurement_volume_ratio=resource_info.routing_to_measurement_volume_ratio,  # noqa
         )
         return info
 
 
 def _get_logarithmic_extrapolation(x, y, steps_to_extrapolate_to):
     x = np.array(x)
@@ -163,15 +169,19 @@
 
     extrapolated_point = ceil(a_opt * np.log(steps_to_extrapolate_to) + b_opt)
 
     # Calculate R-squared value
     y_mean = np.mean(y)
     total_sum_of_squares = np.sum((y - y_mean) ** 2)
     residual_sum_of_squares = np.sum((y - (a_opt * np.log(x) + b_opt)) ** 2)
-    r_squared = 1 - (residual_sum_of_squares / total_sum_of_squares)
+
+    if total_sum_of_squares == 0:
+        r_squared = 1
+    else:
+        r_squared = 1 - (residual_sum_of_squares / total_sum_of_squares)
 
     return extrapolated_point, r_squared
 
 
 def _get_linear_extrapolation(x, y, steps_to_extrapolate_to):
     x = np.array(x)
     y = np.array(y)
@@ -186,15 +196,19 @@
 
     extrapolated_point = ceil(a_opt * steps_to_extrapolate_to + b_opt)
 
     # Calculate R-squared value
     y_mean = np.mean(y)
     total_sum_of_squares = np.sum((y - y_mean) ** 2)
     residual_sum_of_squares = np.sum((y - (a_opt * x + b_opt)) ** 2)
-    r_squared = 1 - (residual_sum_of_squares / total_sum_of_squares)
+
+    if total_sum_of_squares == 0:
+        r_squared = 1
+    else:
+        r_squared = 1 - (residual_sum_of_squares / total_sum_of_squares)
 
     return extrapolated_point, r_squared
 
 
 def _extrapolate(x, y, steps_to_extrapolate_to, objective):
     # Define the constraint that the slope (a) must be greater than zero
     def slope_constraint(params):
```

## Comparing `benchq/resource_estimation/graph/graph_estimator.py` & `benchq/resource_estimators/graph_estimators/graph_estimator.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,26 +8,30 @@
 import networkx as nx
 from graph_state_generation.optimizers import (
     fast_maximal_independent_set_stabilizer_reduction,
     greedy_stabilizer_measurement_scheduler,
 )
 from graph_state_generation.substrate_scheduler import TwoRowSubstrateScheduler
 
-from benchq.resource_estimation.decoder_resource_estimator import get_decoder_info
+from benchq.decoder_modeling.decoder_resource_estimator import get_decoder_info
 
-from ...data_structures import (
-    AlgorithmImplementation,
+from ...algorithms.data_structures import AlgorithmImplementation
+from ...algorithms.data_structures.graph_partition import GraphPartition
+from ...decoder_modeling import DecoderModel
+from ...magic_state_distillation import MagicStateFactory, iter_litinski_factories
+from ...quantum_hardware_modeling import (
     BasicArchitectureModel,
-    DecoderModel,
     DetailedArchitectureModel,
-    GraphData,
-    GraphPartition,
-    GraphResourceInfo,
 )
-from ..magic_state_distillation import Widget, default_widget_list
+from ...quantum_hardware_modeling.devitt_surface_code import (
+    get_total_logical_failure_rate,
+    logical_cell_error_rate,
+    physical_qubits_per_logical_qubit,
+)
+from ..resource_info import GraphData, GraphResourceInfo
 from .transformers import remove_isolated_nodes_from_graph
 
 INITIAL_SYNTHESIS_ACCURACY = 0.0001
 
 
 def substrate_scheduler(graph: nx.Graph, preset: str) -> TwoRowSubstrateScheduler:
     """A simple interface for running the substrate scheduler. Can be run quickly or
@@ -49,20 +53,24 @@
     print("starting substrate scheduler")
     start = time.time()
     if preset == "fast":
         compiler = TwoRowSubstrateScheduler(
             cleaned_graph,
             stabilizer_scheduler=greedy_stabilizer_measurement_scheduler,
         )
-    if preset == "optimized":
+    elif preset == "optimized":
         compiler = TwoRowSubstrateScheduler(
             cleaned_graph,
             pre_mapping_optimizer=fast_maximal_independent_set_stabilizer_reduction,
             stabilizer_scheduler=greedy_stabilizer_measurement_scheduler,
         )
+    else:
+        raise ValueError(
+            f"Unknown preset: {preset}. Should be either 'fast' or 'optimized'."
+        )
     compiler.run()
     end = time.time()
     print("substrate scheduler took", end - start, "seconds")
     return compiler
 
 
 class GraphResourceEstimator:
@@ -77,36 +85,40 @@
         optimization (str): The optimization to use for the estimate. Either estimate
             the resources needed to run the algorithm in the shortest time possible
             ("time") or the resources needed to run the algorithm with the smallest
             number of physical qubits ("space").
         substrate_scheduler_preset (str): Optimize for speed ("fast") so that it can
             be run on larger graphs or for lower resource estimates ("optimized"). For
             graphs of sizes in the thousands of nodes or higher, "fast" is recommended.
-        widgets (Optional[Iterable[Widget]]: Widgets to be used during estimation. If
-            not provided (or passed None) default_widget_list will select widgets based
+        magic_state_factory_iterator (Optional[Iterable[MagicStateFactory]]: iterator
+            over all magic_state_factories.
+            to be used during estimation. If not provided (or passed None)
+            litinski_factory_iterator will select magic_state_factory based
             on hw_model parameter.
     """
 
     # Assumes gridsynth scaling
     SYNTHESIS_SCALING = 4
 
     def __init__(
         self,
         hw_model: BasicArchitectureModel,
         decoder_model: Optional[DecoderModel] = None,
         optimization: str = "space",
         substrate_scheduler_preset: str = "fast",
-        widgets: Optional[Iterable[Widget]] = None,
+        magic_state_factory_iterator: Optional[Iterable[MagicStateFactory]] = None,
     ):
         self.hw_model = hw_model
         self.decoder_model = decoder_model
         self.optimization = optimization
         self.substrate_scheduler_preset = substrate_scheduler_preset
         getcontext().prec = 100  # need some extra precision for this calculation
-        self.widgets = widgets or default_widget_list(hw_model)
+        self.magic_state_factory_iterator = (
+            magic_state_factory_iterator or iter_litinski_factories(hw_model)
+        )
 
     def _get_n_measurement_steps(self, graph) -> int:
         compiler = substrate_scheduler(graph, self.substrate_scheduler_preset)
         n_measurement_steps = len(compiler.measurement_steps)
         return n_measurement_steps
 
     def _get_graph_data_for_single_graph(self, problem: GraphPartition) -> GraphData:
@@ -123,59 +135,33 @@
         )
 
     def _minimize_code_distance(
         self,
         n_total_t_gates: int,
         graph_data: GraphData,
         hardware_failure_tolerance: float,
-        widget: Widget,
+        magic_state_factory: MagicStateFactory,
         min_d: int = 4,
         max_d: int = 200,
     ) -> int:
         for code_distance in range(min_d, max_d):
-            ec_error_rate_at_this_distance = self._get_total_logical_failure_rate(
-                code_distance, n_total_t_gates, graph_data, widget
+            logical_st_volume = self.get_logical_st_volume(
+                n_total_t_gates, graph_data, code_distance, magic_state_factory
+            )
+            ec_error_rate_at_this_distance = get_total_logical_failure_rate(
+                self.hw_model,
+                logical_st_volume,
+                code_distance,
             )
 
             if ec_error_rate_at_this_distance < hardware_failure_tolerance:
                 return code_distance
 
-        raise RuntimeError(f"Required distance is greater than {max_d}.")
-
-    def _get_total_logical_failure_rate(
-        self, code_distance: int, n_total_t_gates: int, graph_data: GraphData, widget
-    ) -> float:
-        precise_logical_cell_failure_rate = Decimal(
-            self._logical_cell_error_rate(code_distance)
-        )
-        precise_logical_st_volume = Decimal(
-            self.get_logical_st_volume(
-                n_total_t_gates, graph_data, code_distance, widget
-            )
-        )
-
-        return float(
-            1 - (1 - precise_logical_cell_failure_rate) ** precise_logical_st_volume
-        )
-
-    def _logical_cell_error_rate(self, distance: int) -> float:
-        precise_physical_qubit_error_rate = Decimal(
-            self.hw_model.physical_qubit_error_rate
-        )
-        precise_distance = Decimal(distance)
-        precise_coefficent = Decimal(0.3)
-        return float(
-            1
-            - (
-                1
-                - precise_coefficent
-                * (70 * precise_physical_qubit_error_rate)
-                ** ((precise_distance + 1) / 2)
-            )
-            ** precise_distance
+        raise RuntimeError(
+            f"Required distance is greater than maximum allowable distance: {max_d}."
         )
 
     def _get_v_graph(
         self,
         graph_data: GraphData,
         code_distance: int,
     ):
@@ -198,46 +184,46 @@
         return V_graph
 
     def _get_v_measure(
         self,
         n_total_t_gates: int,
         graph_data: GraphData,
         code_distance: int,
-        widget: Widget,
+        magic_state_factory: MagicStateFactory,
     ):
         if self.optimization == "space":
             V_measure = (
                 2
                 * graph_data.max_graph_degree
                 * n_total_t_gates
-                * (widget.distillation_time_in_cycles + code_distance)
+                * (magic_state_factory.distillation_time_in_cycles + code_distance)
             )
         elif self.optimization == "time":
             V_measure = (
                 n_total_t_gates
-                * widget.space[1]
-                * (widget.distillation_time_in_cycles + code_distance)
+                * magic_state_factory.space[1]
+                * (magic_state_factory.distillation_time_in_cycles + code_distance)
                 / (2 ** (1 / 2) * code_distance + 1)
             )
         else:
             raise ValueError(
                 f"Unknown optimization: {self.optimization}. "
                 "Should be either 'time' or 'space'."
             )
         return V_measure
 
     def get_logical_st_volume(
         self,
         n_total_t_gates: int,
         graph_data: GraphData,
         code_distance: int,
-        widget: Widget,
+        magic_state_factory: MagicStateFactory,
     ):
         return self._get_v_graph(graph_data, code_distance) + self._get_v_measure(
-            n_total_t_gates, graph_data, code_distance, widget
+            n_total_t_gates, graph_data, code_distance, magic_state_factory
         )
 
     def get_n_total_t_gates(
         self,
         n_t_gates: int,
         n_rotation_gates: int,
         transpilation_failure_tolerance: float,
@@ -258,52 +244,60 @@
         return n_t_gates + n_t_gates_used_at_measurement
 
     def _get_time_per_circuit_in_seconds(
         self,
         graph_data: GraphData,
         code_distance: int,
         n_total_t_gates: float,
-        widget: Widget,
+        magic_state_factory: MagicStateFactory,
     ) -> float:
         if self.optimization == "space":
             return (
                 6
                 * self.hw_model.surface_code_cycle_time_in_seconds
                 * (
                     graph_data.n_measurement_steps * code_distance
-                    + (widget.distillation_time_in_cycles + code_distance)
+                    + (magic_state_factory.distillation_time_in_cycles + code_distance)
                     * n_total_t_gates
                 )
             )
         elif self.optimization == "time":
             return (
                 6
                 * self.hw_model.surface_code_cycle_time_in_seconds
                 * (
                     graph_data.n_measurement_steps * code_distance
-                    + widget.distillation_time_in_cycles
+                    + magic_state_factory.distillation_time_in_cycles
                     + code_distance
                 )
             )
         else:
             raise NotImplementedError(
                 "Must use either time or space optimal estimator."
             )
 
     def _get_n_physical_qubits(
-        self, graph_data: GraphData, code_distance: int, widget: Widget
+        self,
+        graph_data: GraphData,
+        code_distance: int,
+        magic_state_factory: MagicStateFactory,
     ) -> int:
-        patch_size = 2 * code_distance**2
+        patch_size = physical_qubits_per_logical_qubit(code_distance)
         if self.optimization == "space":
-            return 2 * graph_data.max_graph_degree * patch_size + widget.qubits
+            return (
+                2 * graph_data.max_graph_degree * patch_size
+                + magic_state_factory.qubits
+            )
         elif self.optimization == "time":
             return ceil(
                 graph_data.max_graph_degree * patch_size
-                + 2 ** (0.5) * graph_data.n_measurement_steps * widget.space[0]
-                + widget.qubits * graph_data.n_measurement_steps
+                + 2 ** (0.5)
+                * graph_data.n_measurement_steps
+                * magic_state_factory.space[0]
+                + magic_state_factory.qubits * graph_data.n_measurement_steps
             )
         else:
             raise NotImplementedError(
                 "Must use either time or space optimal estimator."
             )
 
     def estimate_resources_from_graph_data(
@@ -311,64 +305,75 @@
         graph_data: GraphData,
         algorithm_implementation: AlgorithmImplementation,
     ) -> GraphResourceInfo:
         this_transpilation_failure_tolerance = (
             algorithm_implementation.error_budget.transpilation_failure_tolerance
         )
 
-        widget_iterator = iter(self.widgets)
+        magic_state_factory_iterator = iter(self.magic_state_factory_iterator)
+
+        # Approximate the number of logical qubits for the bus architecture
+        # TODO: Update to accommodate the space vs time optimal compilation
+        # once we have the substrate scheduler properly implemented.
+        n_logical_qubits = 2 * graph_data.max_graph_degree
 
         while True:
-            widget_found = False
-            for widget in widget_iterator:
+            magic_state_factory_found = False
+            for magic_state_factory in magic_state_factory_iterator:
                 tmp_graph_data = replace(
                     graph_data,
                     n_nodes=ceil(
-                        graph_data.n_nodes / widget.n_t_gates_produced_per_distillation
+                        graph_data.n_nodes
+                        / magic_state_factory.n_t_gates_produced_per_distillation
                     ),
                     n_t_gates=ceil(
                         graph_data.n_t_gates
-                        / widget.n_t_gates_produced_per_distillation
+                        / magic_state_factory.n_t_gates_produced_per_distillation
                     ),
                 )
 
                 n_total_t_gates = self.get_n_total_t_gates(
                     tmp_graph_data.n_t_gates,
                     tmp_graph_data.n_rotation_gates,
                     this_transpilation_failure_tolerance,
                 )
                 code_distance = self._minimize_code_distance(
                     n_total_t_gates,
                     tmp_graph_data,
                     algorithm_implementation.error_budget.hardware_failure_tolerance,
-                    widget,
+                    magic_state_factory,
+                )
+                this_logical_cell_error_rate = logical_cell_error_rate(
+                    self.hw_model.physical_qubit_error_rate, code_distance
                 )
-                _logical_cell_error_rate = self._logical_cell_error_rate(code_distance)
 
                 # Ensure we can ignore errors from magic state distillation.
-                if widget.distilled_magic_state_error_rate < _logical_cell_error_rate:
-                    widget_found = True
+                if (
+                    magic_state_factory.distilled_magic_state_error_rate
+                    < this_logical_cell_error_rate
+                ):
+                    magic_state_factory_found = True
                     break
-            if not widget_found:
+            if not magic_state_factory_found:
                 warnings.warn(
-                    "No viable widget found! Returning null results.", RuntimeWarning
+                    "No viable magic_state_factory found! Returning null results.",
+                    RuntimeWarning,
                 )
                 return GraphResourceInfo(
                     code_distance=-1,
                     logical_error_rate=1.0,
-                    # estimate the number of logical qubits using max node degree
-                    n_logical_qubits=graph_data.max_graph_degree,
+                    n_logical_qubits=n_logical_qubits,
                     total_time_in_seconds=0.0,
                     n_physical_qubits=0,
-                    widget_name="No Widget Found",
+                    magic_state_factory_name="No MagicStateFactory Found",
                     decoder_info=None,
                     routing_to_measurement_volume_ratio=0.0,
                     extra=graph_data,
                 )
-            if this_transpilation_failure_tolerance < _logical_cell_error_rate:
+            if this_transpilation_failure_tolerance < this_logical_cell_error_rate:
                 # if the t gates typically do not come from rotation gates, then
                 # then you will have to restart the calculation from scratch.
                 if graph_data.n_t_gates < 0.01 * graph_data.n_nodes:
                     raise RuntimeError(
                         "Run estimate again with lower synthesis failure tolerance."
                     )
                 if this_transpilation_failure_tolerance < 1e-10:
@@ -379,65 +384,70 @@
                 this_transpilation_failure_tolerance /= 10
             else:
                 graph_data = tmp_graph_data
                 break
 
         # get error rate after correction
         space_time_volume = self.get_logical_st_volume(
-            n_total_t_gates, graph_data, code_distance, widget
+            n_total_t_gates, graph_data, code_distance, magic_state_factory
         )
 
         graph_measure_ratio = (
             self._get_v_graph(graph_data, code_distance) / space_time_volume
         )
 
-        total_logical_error_rate = self._get_total_logical_failure_rate(
-            code_distance, n_total_t_gates, graph_data, widget
+        logical_st_volume = self.get_logical_st_volume(
+            n_total_t_gates, graph_data, code_distance, magic_state_factory
+        )
+
+        total_logical_error_rate = get_total_logical_failure_rate(
+            self.hw_model,
+            logical_st_volume,
+            code_distance,
         )
 
         # get number of physical qubits needed for the computation
         n_physical_qubits = self._get_n_physical_qubits(
-            graph_data, code_distance, widget
+            graph_data, code_distance, magic_state_factory
         )
 
         # get total time to run algorithm
         time_per_circuit_in_seconds = self._get_time_per_circuit_in_seconds(
-            graph_data, code_distance, n_total_t_gates, widget
+            graph_data, code_distance, n_total_t_gates, magic_state_factory
         )
 
         # The total space time volume, prior to measurements is,
         # V_{graph}= 2\Delta S (where we measure each of the steps,
         # S in terms of tocks, corresponding to d cycle times.
         # d will be solved for later).  For each distilled T-state,
         # C-cycles are needed to prepare the state and 1-Tock is required
         # to interact the state with the graph node and measure it in
         # the X or Z-basis.  Hence for each node measurement (assuming
         # T-basis measurements), the volume increases to,
         # V = 2*Delta*S*d+ 2*Delta*(C+d).
 
         total_time_in_seconds = (
-            time_per_circuit_in_seconds * algorithm_implementation.n_calls
+            time_per_circuit_in_seconds * algorithm_implementation.n_shots
         )
 
         decoder_info = get_decoder_info(
             self.hw_model,
             self.decoder_model,
             code_distance,
             space_time_volume,
-            graph_data.max_graph_degree,
+            n_logical_qubits,
         )
 
         return GraphResourceInfo(
             code_distance=code_distance,
             logical_error_rate=total_logical_error_rate,
-            # estimate the number of logical qubits using max node degree
-            n_logical_qubits=graph_data.max_graph_degree,
+            n_logical_qubits=n_logical_qubits,
             total_time_in_seconds=total_time_in_seconds,
             n_physical_qubits=n_physical_qubits,
-            widget_name=widget.name,
+            magic_state_factory_name=magic_state_factory.name,
             decoder_info=decoder_info,
             routing_to_measurement_volume_ratio=graph_measure_ratio,
             extra=graph_data,
         )
 
     def estimate(
         self, algorithm_implementation: AlgorithmImplementation
```

## Comparing `benchq/resource_estimation/graph/transformers.py` & `benchq/resource_estimators/graph_estimators/transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import time
 from copy import copy
 from typing import Callable, Sequence, Tuple
 
 import networkx as nx
 
+from ...algorithms.data_structures import ErrorBudget, GraphPartition
 from ...compilation import (
     get_algorithmic_graph_from_ruby_slippers,
     pyliqtr_transpile_to_clifford_t,
 )
 from ...compilation import transpile_to_native_gates as _transpile_to_native_gates
-from ...data_structures import (
-    ErrorBudget,
-    GraphPartition,
+from ...problem_embeddings.quantum_program import (
     QuantumProgram,
     get_program_from_circuit,
 )
 
 
 def _distribute_transpilation_failure_tolerance(
     program: QuantumProgram, total_transpilation_failure_tolerance: float
```

## Comparing `benchq-0.6.0.dist-info/LICENSE` & `benchq-0.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `benchq-0.6.0.dist-info/METADATA` & `benchq-0.7.0.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,123 +1,141 @@
 Metadata-Version: 2.1
 Name: benchq
-Version: 0.6.0
+Version: 0.7.0
 Summary: "BenchQ platform for resource estimation"
 Home-page: https://github.com/zapatacomputing/benchq
 Author: Zapata Computing Inc.
 Author-email: info@zapatacomputing.com,
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: !=3.9.7,>=3.9
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 Requires-Dist: orquestra-quantum ==0.12.0
 Requires-Dist: orquestra-vqa ==0.9.0
-Requires-Dist: orquestra-qiskit ==0.13.0
-Requires-Dist: orquestra-cirq ==0.11.0
+Requires-Dist: orquestra-qiskit ==0.14.0
+Requires-Dist: orquestra-cirq ==0.12.0
+Requires-Dist: orquestra-opt ==0.10.0
 Requires-Dist: networkx >=2.8.7
 Requires-Dist: orquestra-sdk[all] >=0.46.0
 Requires-Dist: matplotlib >=3.6
 Requires-Dist: numpy >=1.20
 Requires-Dist: more-itertools ~=9.1.0
 Requires-Dist: pandas ==1.5.3
 Requires-Dist: pyLIQTR ==0.3.3
-Requires-Dist: openfermion ~=1.5.0
+Requires-Dist: openfermion[resources] ~=1.6.0
 Requires-Dist: pytest
 Requires-Dist: graph-state-generation ==0.2.0
 Requires-Dist: juliapkg ==0.1.10
 Requires-Dist: juliacall ~=0.9.10
 Requires-Dist: h5py ~=3.8.0
 Requires-Dist: mlflow ~=2.3.2
 Requires-Dist: stim ==1.10
 Requires-Dist: optuna ==3.3.0
 Requires-Dist: cvxpy ==1.3.2
+Requires-Dist: aiohttp ~=3.9.0
+Requires-Dist: setuptools <=65.6.3
 Provides-Extra: azure
 Requires-Dist: benchq[pyscf] ; extra == 'azure'
 Requires-Dist: azure-quantum ==0.28.262328b1 ; extra == 'azure'
 Requires-Dist: pyqir ==0.8.0 ; extra == 'azure'
 Requires-Dist: qiskit-qir ==0.3.1 ; extra == 'azure'
 Requires-Dist: qiskit-ionq ==0.3.10 ; extra == 'azure'
 Provides-Extra: dev
 Requires-Dist: orquestra-python-dev ; extra == 'dev'
 Requires-Dist: pytest-benchmark ~=4.0.0 ; extra == 'dev'
 Requires-Dist: numba ~=0.57.0 ; extra == 'dev'
 Requires-Dist: benchq[pyscf] ; extra == 'dev'
 Requires-Dist: benchq[azure] ; extra == 'dev'
+Requires-Dist: pyright ; extra == 'dev'
 Provides-Extra: pyscf
 Requires-Dist: pyscf ==2.2.1 ; extra == 'pyscf'
 Requires-Dist: scipy <1.11.0 ; extra == 'pyscf'
 Requires-Dist: openfermionpyscf ==0.5 ; extra == 'pyscf'
 
-# benchq
+# Bench-Q
+Bench-Q provides tools for estimating the hardware resources required for fault-tolerant quantum computation. It includes a graph-state compiler, distillation factory models, decoder performance models, an ion-trap architecture model, implementations of selected quantum algorithms, and more.
 
-## What is it?
-
-`benchq` estimates the required resources for performing a fault-tolerant computation using surface codes. It works with various inputs, such as circuits, openfermion QubitOperators, and pyscf files. Given correct input, `benchq` will return a list of resources required to perform the selected algorithm such as the required number of physical qubits, error rate, wall time, etc.
-
-`benchq` was developed as a part of [DARPA Quantum Benchmarking program](https://www.darpa.mil/program/quantum-benchmarking).
+Bench-Q was developed as a part of [DARPA Quantum Benchmarking program](https://www.darpa.mil/program/quantum-benchmarking).
 
 ## Installation
 
-To install `benchq` run `pip install .` from the main directory.
-It's been tested with Python 3.8-3.9 on macOS and Linux. Requires Jabalizer 0.4.3.
+To install the latest released version of Bench-Q run `pip install benchq`.
+It is tested with Python 3.9-3.11 on Linux and may or may not work with other Python versions or operating systems.
 
-Known limitation: installation can fail because of a problem with `pyscf`, one of our transitive dependencies.
-If you're a Windows user, please consider using [WSL](https://learn.microsoft.com/en-us/windows/wsl/install). On other systems you can try installing `pyscf` directly from its git repo: `pip install git+https://github.com/pyscf/pyscf@v2.0.1`.
+To use the development version of Bench-Q, clone this repository and run `pip install .` from the top-level directory.
 
 ### Extra dependencies
 
 #### Julia
-If you want to run the Graph State Compilation pipeline, you'll have to install Julia. Fortunately, benchq will install Julia automatically for you whenever it is needed if your current Julia installation is not compatible with the version of Julia that benchq requires. To avoid issues with conflicting versions, `juliapkg` do not install Julia in the typical {home}/.julia directory. We instead install julia within the python version you are using (if you are using a virtualenv, it will be installed in the file containing your virtualenv).
+Although the Graph State Compilation pipeline requires Julia, you do not need to manually install it: benchq will install Julia automatically whenever it is needed if you do not already have a version of Julia that is compatible with Bench-Q installed.
 
-Note that running `julia` from the terminal may not give you access to the version of Julia that BenchQ installs. This is to prevent conflicts with other Julia installations you may have on your system. See the `juliapkg` documentation for more information.
+Note that running `julia` from the terminal may not give you access to the version of Julia installed by Bench-Q. This is because JuliaPkg will install Julia in an isolated environment in order to avoid any potential conflicts with other versions of Julia that are already installed. See the [JuliaPkg documentation](https://github.com/JuliaPy/pyjuliapkg/blob/main/README.md) for more information about how Bench-Q installs Julia.
 
 #### PySCF
 If you plan to use PySCF to generate Hamiltonians, use the `pyscf` install extra:
 ```bash
 pip install '.[pyscf]'
 ```
 
+On some systems, the installation of PySCF can be problematic. If you're a Windows user, consider using [WSL](https://learn.microsoft.com/en-us/windows/wsl/install). You might also consider installing PySCF directly from its git repo: `pip install git+https://github.com/pyscf/pyscf@v2.2.1`.
+
+
 #### Azure Quantum Resource Estimation
-To run resource estimation using Azure Quantum Resource Estimation (QRE) tool, one needs to have Azure QRE package configured, please see [this tutorial](https://learn.microsoft.com/en-us/azure/quantum/intro-to-resource-estimation).
+To run resource estimation using Azure Quantum Resource Estimation (QRE) tool, one needs to have Azure QRE package configure. See [this tutorial](https://learn.microsoft.com/en-us/azure/quantum/intro-to-resource-estimation) for more information.
 
 ## Usage
+See the [`examples`](examples) directory to learn more about how to use Bench-Q.
+
+### Terminology Disambiguation
+
+As fault-tolerant quantum computing is a relatively new field, there is no for several concepts which are crucial for resource estimation. We will try to clarify them here.
+
+#### Problem Ingestion vs Problem Embedding vs Algorithm Implementation
+
+`benchq` splits up the process of specifying a problem into three steps. The purpose of this is to split up the more complex parts of the process into more digestable, modular parts. The three steps are:
+
+##### Problem ingestion
+
+Take an input representing a problem instance and outputs data that needs to be loaded into the quantum computer. (e.g. the Hamiltonian we are simulating)
+
+##### Problem embedding
+Take the data from the problem ingestion step and embed it into a quantum circuit. (e.g. the block encoding circuit.) This can be a complicated process involving arithmetic and specialized compilation.
+
+##### Algorithm implementation
+Take the circuit from the problem embedding step and implement the algorithm. Also requires information from the problem instance to determine how to budget errors throughout the computation. (e.g. the required accuracy of the algorithm.)
 
-Please take a look at the `examples` directory.
-We have multiple examples there:
-- `h_chain_trotter.py` shows how to use graph state compilation on a simple hydrogen chain example. (Requires `pyscf` install extra.)
-- `resource_estimate_from_qasm.py` shows how to use graph state compilation when the circuit is loaded from QASM.
-- `qsp_vlasov.py` shows how to perform resource estimation.
 
 ## Running benchmarks
 
-To run the benchmarks run
+Because quantum compilation and resource estimation can be compute intensive, Bench-Q includes tools for benchmarking components that are potential bottlenecks. To run the benchmarks, execute the command
 
 ``` bash
 pytest benchmarks/
 ```
 
-from the top-level directory of this repo. By default, this will skip some benchmarks that run extremely low. If you want to run
+from the top-level directory of this repo.
+
+By default, this will skip some benchmarks that are extremely slow. If you want to run
 those too, set environmental variable `SLOW_BENCHMARKS` to any value, e.g.:
 
 ``` bash
 SLOW_BENCHMARKS=1 pytest benchmarks/
 ```
 
-Our benchmarks are run automatically on each release. You can see the performance of benchq over time on [benchq's benchmark page](https://zapatacomputing.github.io/benchq/dev/bench/).
+These benchmarks are run automatically on each release. You can see the performance of benchq over time on [benchq's benchmark page](https://zapatacomputing.github.io/benchq/dev/bench/).
 
 ## Development and Contribution
 
-To install the development version, run `pip install -e '.[dev]'` from the main directory. (if using MacOS, you will need single quotes around the []. If using windows, or Linux, you might not need the quotes).
-
-We use [Google-style](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html) docstring format. If you'd like to specify types please use [PEP 484](https://www.python.org/dev/peps/pep-0484/) type hints instead adding them to docstrings.
+To install the development version, run `pip install -e '.[dev]'` from the main directory.
 
-There are codestyle-related [Github Actions](.github/workflows/style.yml) running for PRs. (TODO)
+We use [Google-style](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html) docstring format. If you'd like to specify types, please use [PEP 484](https://www.python.org/dev/peps/pep-0484/) type hints instead adding them to docstrings.
+[Style checks](.github/workflows/style.yml) will automatically be run on pull requests.
 
 - If you'd like to report a bug/issue please create a new issue in this repository.
 - If you'd like to contribute, please create a pull request to `main`.
 
 ### Running tests
 
 Unit tests for this project can be run using `make coverage` command from the main directory.
```

## Comparing `benchq-0.6.0.dist-info/RECORD` & `benchq-0.7.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,83 @@
-benchq/__init__.py,sha256=aGY15JbU_l3B8r2dbxz1f5Tji15ZjptahufehTRVmNE,525
+benchq/__init__.py,sha256=VACI-MDgOGPLPcC2MrRAgcellmt7g5J7jkc4LSg2FCg,349
 benchq/timing.py,sha256=ePyIur0NbG83rK7HffNT4DZDT8msgUmYYCS3xWG2udc,541
-benchq/vizualization_tools.py,sha256=ZBdatIn9VTXYnLF4qhlb82h5ldlUDbGDXNl_N0zPQAs,5958
-benchq/algorithms/__init__.py,sha256=t8HXdvQAq7bzde432jF_KcwtVlNLCXxJEY602CKpi2c,137
-benchq/algorithms/gsee.py,sha256=UaPDApgwpw-dV1kMHI7y4GvOUWC6eSJZvv4_SEEI38I,1083
-benchq/algorithms/ld_gsee.py,sha256=I1hMgky1DcVeelTyXW7GNApjUtLS_drG8DFOdZLH60o,4415
-benchq/algorithms/lde_solver.py,sha256=vc2SEI2XB1Zb_IJRxusnOgX8pKsllAEkYkVPAF4B5oE,14027
-benchq/algorithms/lin_and_dong_qsp.py,sha256=KB_gZkaYJEw9U0elMjuKankxXgBsnjqnZW6pg6PQGUQ,5017
-benchq/algorithms/qaoa.py,sha256=1PP046OWa3_VlLZuaWvyL7khytZszBMlyvQIMlA_ap0,2586
-benchq/algorithms/time_evolution.py,sha256=x9EXmhO_BNrdx4twnUz5cUJgd5kbd4DKxvjmRH40OAY,2788
-benchq/algorithms/utils/compression_gadget.py,sha256=WxSa3EIt2ITbNuIr3NJu53oV2ZnaDkcNJDjqDHpwuvc,537
-benchq/algorithms/utils/convex_optimization.py,sha256=4GwXDfRr0iRGy6lhVx7K34YzQfzygVnayXXzjm0IQhk,4694
-benchq/algorithms/utils/qsp_solver.py,sha256=0YO7K4xLxtRqFK1zD226bbANhWqR3_969UM_HLwM1QQ,15067
-benchq/block_encodings/block_encoding_utils.py,sha256=LatM2MJSulYkPTsfwa8fFfqassAAs0x_7FOcA_W8TZg,3939
-benchq/block_encodings/offset_tridiagonal.py,sha256=hgCc5VB9anx1qwiq0p69uP7EKNGrvbf2rh46ZaXwzE0,2040
+benchq/visualization_tools.py,sha256=y5qEGNhVgIi3ZLo4RI7-AwtxNM65fpiSmTtsVLZeJ6o,5990
+benchq/algorithms/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+benchq/algorithms/profolio_optimization.py,sha256=Mc5sHc3JfImLqBBuhWtPlbpuYLkHMTtmaMRQAmJB0CY,1308
+benchq/algorithms/time_evolution.py,sha256=-ru22dvb0Ut0Waalld04rKetJnhi0uvEvIfp_i9g2AE,2853
+benchq/algorithms/data_structures/__init__.py,sha256=1PzsxfShyWBlbYjesK8uGX-mW1DAt_kDcvTynKbCgqE,431
+benchq/algorithms/data_structures/algorithm_implementation.py,sha256=4QWeqAGJNi-uz2qWQDAl5h2A5hja-tW2SUvyvp7CikA,730
+benchq/algorithms/data_structures/error_budget.py,sha256=zR4rjpoUeGsNwlpWvnzR2p7-M1LJG1HWiNLsBDWsmb8,3511
+benchq/algorithms/data_structures/graph_partition.py,sha256=LoVAoLUGU5RnAwx4h13BZsq81ktNEy8I4OTYLbJl9Pc,858
+benchq/algorithms/gsee/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+benchq/algorithms/gsee/ld_gsee.py,sha256=I1hMgky1DcVeelTyXW7GNApjUtLS_drG8DFOdZLH60o,4415
+benchq/algorithms/gsee/qpe_gsee.py,sha256=aMzVAWb59tefweOwi4eY9yk6BQryCfKNJFShyGMhiMQ,1151
 benchq/compilation/__init__.py,sha256=nY_iW2lYYi-pfi5xXYimMaC1vexLaSztKc9-Lsm9cyg,785
 benchq/compilation/graph_sim_data.jl,sha256=TD8EKdMMEDMisutaGCAH7mCkxihNKUUdMcUfcbU1s8s,4524
 benchq/compilation/initialize_julia.py,sha256=GDft1Isa2OregKxwaSJTKoKjWEStr2wo5DRnpLSZHxI,1855
 benchq/compilation/jabalizer_wrapper.jl,sha256=q83msw4EXQQzbfRF2qEFmiYsAI22w_DT1lmIrs0IR3Q,3106
 benchq/compilation/julia_utils.py,sha256=jVgsU37g-Q0ur-n6ZLE9-8OAeFvbEhxULUD10VTw3Qs,2367
-benchq/compilation/pyliqtr_transpilation.py,sha256=7DEgZkPGiPid9JArBIUWGNi9yXA-Gb3l0H3S0KTwLYs,3067
-benchq/compilation/rbs_hyperparam_tuning.py,sha256=WC3uGY4_d6zecCTjU_YWqqBnwn9v9DG0vZM0eSgDH6w,17410
+benchq/compilation/pyliqtr_transpilation.py,sha256=2a3VbJyCiQ5lxQTCuS2jGWRfDGA1j9s0Ff5NMIn_wxo,3268
+benchq/compilation/rbs_hyperparam_tuning.py,sha256=Klz898NmVt_tKbPNu2MfeDG5i3U-H6GmWh9NQjreqpQ,17502
 benchq/compilation/ruby_slippers.jl,sha256=MMfXMiX37lllmvexf6bIcYzlUHcG3Q3nBvwslNYhuAY,22742
-benchq/compilation/transpile_to_native_gates.py,sha256=b-UUgvUB3Z-5_Gb2SbxP-iZ_-mFHIYE1_tAQItW4OmA,9497
-benchq/conversions/__init__.py,sha256=Stn41mu1kxrF2Tbi3EnFEaynsEpEyAL6YTFMlxdt7IY,367
-benchq/conversions/_circuit_translations.py,sha256=L9CG2katEWDNmfF_-u1uT7viTBWxFNqhpPS_i2EbzNI,3170
+benchq/compilation/transpile_to_native_gates.py,sha256=SJh66nbiKZi0ZWJWnbR0a3P6RukwOw2vsjPhubm3XbI,9527
+benchq/conversions/__init__.py,sha256=P7ufq9iSncdt4G5goq4FyKEBP2437gFC570z_Yo04Fc,371
+benchq/conversions/_circuit_translations.py,sha256=-WaW5h8cWCOxkD-Bfc3yWvo49VBievY-48sqyiYkeN8,2169
 benchq/conversions/_openfermion_pyliqtr.py,sha256=FATkz_tX-N2jUUTLZeZTnTXi27Dxr2_Sw2GeONOSKaQ,1266
-benchq/data_structures/__init__.py,sha256=tun0_-4V0i-7crHrwjUc9xh39-37TkUnyNz_qcewSsg,1608
-benchq/data_structures/algorithm_implementation.py,sha256=KZ1nQrHRMkJ0Md_iB_DQwr3NO2h4bYZtIV3fvBjKOaw,688
-benchq/data_structures/decoder.py,sha256=VL5Lxv0O5qOlSszahe6-CaowsIDE2TBPM6Bs7hBu-Fk,4386
-benchq/data_structures/error_budget.py,sha256=zR4rjpoUeGsNwlpWvnzR2p7-M1LJG1HWiNLsBDWsmb8,3511
-benchq/data_structures/graph_partition.py,sha256=CDycgKv35xpzfMewju9-cM6jz3mVJofecSQeenyLUjQ,837
-benchq/data_structures/hardware_architecture_models.py,sha256=iT2Nh-TMkjgQuRGrfuhbEHURCabGpuPXdrnw2i6VOPA,9203
-benchq/data_structures/quantum_program.py,sha256=G8FgMl-v9x0A_BIC-BvGLh0THiJ0N2fR-uCkwmf9eKI,3970
-benchq/data_structures/resource_info.py,sha256=mQNxylhUm7OZG1lIMDCXQVfHg2cb-MEi34rFM0ywVlE,3751
-benchq/mlflow/__init__.py,sha256=bDQWkB-Ap7hHacahs9Anj3pQJMl6WMtaO54mSpH_Gf0,287
-benchq/mlflow/data_logging.py,sha256=Uwm7wgtlYYIM0n5e70PlkKfEs_5OiNVXeubyXmSBOp0,3543
-benchq/problem_embeddings/__init__.py,sha256=n329WFeQwg94-7pPLrti6PokzCFwL_XXQ0m4Vd2wWOA,323
-benchq/problem_embeddings/_qsp.py,sha256=w6oarvuIZMJk31N9Xb8_MmoPpQktM3XR5HplVYX-MVQ,10310
-benchq/problem_embeddings/_taylorization_lcu.py,sha256=qh_AhzcXPXbdGZTlt46Q3SIlC-SRnuuFY2w2koskVlU,12616
-benchq/problem_embeddings/_trotter.py,sha256=FrptntFd9GrQ4AQxJ-vpjyPLSGe5CmmnSWInCALctxU,1170
-benchq/problem_ingestion/__init__.py,sha256=XBHtodUBeu5X7kwG_WDt-H_yJRzOZ8TyV1QWeJVLmfg,496
-benchq/problem_ingestion/hamiltonian_from_file.py,sha256=BsEj0lGLV_W36Zl1VcIc-ssHgBdZqaeE6gf03Dew05o,6941
-benchq/problem_ingestion/hamiltonian_generation.py,sha256=JOnCop2BNdvgJKjPzrepKpepaNdqKZ7Db9a-LV4YNB0,6214
-benchq/problem_ingestion/molecule_instance_generation.py,sha256=JzX0Bq3F6xx9EmEndWPrpR0GfYF_yr3laFgEdTbLiNw,22503
-benchq/problem_ingestion/vlasov.py,sha256=vlpyN-gOYLGuUPx9z4hhIuXUhD4vvqBaA0T2XtLgHy8,886
-benchq/resource_estimation/__init__.py,sha256=dmaqVMrKDFGl8jNeu4G1sHtdNAq3tRpL7fKU8v9fiU0,392
-benchq/resource_estimation/_compute_lambda.py,sha256=jGH5YBTvXCk7ezLaD52TkMGYUenpG7CwCFDkoj9XFRk,2775
-benchq/resource_estimation/_footprint_analysis.py,sha256=ohBUrUh4pPb0PqmGhRGCfmJ02C6FTuVwzhvlZOzsYJ8,10220
-benchq/resource_estimation/azure.py,sha256=bInu5M15-6h-K-ApPqOjE8avzZCET72xiyC06gTZn7c,4846
-benchq/resource_estimation/decoder_resource_estimator.py,sha256=fZImplRQCm29A2THmegU9Fb44SA6u3CI4NYMg0OsZYo,3692
-benchq/resource_estimation/default_pipelines.py,sha256=_haTDqh2dMVeMK-AlF8BsxraK4DbZWxb2o6qQHJ8PKI,11887
-benchq/resource_estimation/magic_state_distillation.py,sha256=qfKfaBTkFPLTam3XuqLhuUWMmywJQSZuqjFyLNruvyA,3188
-benchq/resource_estimation/openfermion_re.py,sha256=DHQPA2IedeL7aPpBCwkULAj2XKHuSDDiJwgtiTameTA,11021
-benchq/resource_estimation/graph/__init__.py,sha256=VViOp_APJzkCghrrDXzOhQOu4T6ihzI2I4OuWy8hipU,878
-benchq/resource_estimation/graph/customizable_pipelines.py,sha256=2l_gQk3cbVs8WZL-gJ7fu1eKdWm1_HDCMVBy-jKw6aQ,3950
-benchq/resource_estimation/graph/extrapolation_estimator.py,sha256=gHc3YYZXnXEJMMpK7qboQOUat4kn0WNGbjY-WipEd3g,8240
-benchq/resource_estimation/graph/graph_estimator.py,sha256=BIJPREV3wKoToTLi6_wxqfcEuLrD3uC1QsZPAqBhBr8,17630
-benchq/resource_estimation/graph/transformers.py,sha256=2M1Yros1UVR1fXnHaX5dF501Dgq6L4vbC8LJaZqLQ2c,4856
-benchq/resource_estimation/graph/worstcase_footprint_estimator.py,sha256=7JKpiaB17iYg5Sq7cySgjKAa0czkY5svM5pxkWrMvis,5728
-benchq-0.6.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-benchq-0.6.0.dist-info/METADATA,sha256=88RwDDdAkAjUfjmCePoUasIG2sbmDaKNWJEqqf2lpsU,6511
-benchq-0.6.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-benchq-0.6.0.dist-info/top_level.txt,sha256=RGAPdCRmbLQ_m241jwm5Q75qzuaWjICnIa16V6jkerE,7
-benchq-0.6.0.dist-info/RECORD,,
+benchq/decoder_modeling/__init__.py,sha256=2xz3SDdoeRW6pa4BtjJ8kQCu51WpBtQVBf9Ht_PENGA,34
+benchq/decoder_modeling/decoder.py,sha256=PJym7DEorSPpkzI6IXVcUzRAkB7cBBCpLNKM1TZYKaE,4308
+benchq/decoder_modeling/decoder_resource_estimator.py,sha256=khgaWFomeF5BivZED1gpaWwDK9IsJGVry37PDeYT-U8,3746
+benchq/magic_state_distillation/__init__.py,sha256=SBjLF3Mm3KiybHe6ee_X6PgBTEFt0hm445vATVbZddc,162
+benchq/magic_state_distillation/autoccz_factories.py,sha256=L26Nnq_ZBnOWbdz9dVB2vepGv7DdBv8EovJI3vlT7-E,4215
+benchq/magic_state_distillation/litinski_factories.py,sha256=QoCR_SxC23Sa_hnNPRuY8IJfp-4er2CnUCkluKdeSYo,2203
+benchq/magic_state_distillation/magic_state_factory.py,sha256=OpJRdt1MZtykXgcxXGpt9IvHYVHYowiNLp3xOzFId2w,299
+benchq/mlflow/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+benchq/mlflow/data_logging.py,sha256=DiJMwYHyYuQtkcaKRUbzWeOBeT21QpwQKGCDSegXPhY,3650
+benchq/problem_embeddings/__init__.py,sha256=RUxALOy-vbf9rza3Bf76Kk7nR1iK54yhY9IJvjaQMfU,397
+benchq/problem_embeddings/_qaoa.py,sha256=lv3ZGlGKT5ckCVAvUA7govQFdDa55L7vgZKcf_lP1oU,2286
+benchq/problem_embeddings/_trotter.py,sha256=e2odiL9YYWJFPCd85pg2HXkemCgjpglaxQ8Iv5EtCNo,1169
+benchq/problem_embeddings/qpe.py,sha256=_HDfL2nekrCZYWlhlImzME2bGIUGYuI7_yp3slCedIA,5229
+benchq/problem_embeddings/quantum_program.py,sha256=u9n74XNav3khsOG2ndm08nlzQlcdx0LeNarcQUlEC-4,4081
+benchq/problem_embeddings/block_encodings/double_factorized_hamiltonian.py,sha256=uTiwVtKPCTCGiIuB-PRaJAv7fB8ENGK8rDEBjMCNnYA,3198
+benchq/problem_embeddings/block_encodings/offset_tridiagonal.py,sha256=-13PgLKkCS29z4DQheftZ77HnpmEtydREUgI8cWm5wk,2044
+benchq/problem_embeddings/block_encodings/offset_tridiagonal_utils.py,sha256=LatM2MJSulYkPTsfwa8fFfqassAAs0x_7FOcA_W8TZg,3939
+benchq/problem_embeddings/qsp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+benchq/problem_embeddings/qsp/_lin_and_dong_qsp.py,sha256=KB_gZkaYJEw9U0elMjuKankxXgBsnjqnZW6pg6PQGUQ,5017
+benchq/problem_embeddings/qsp/_qsp.py,sha256=c16qT8r81yokmn6SsFNaqsfBtuM57Js5t04E0mxfCvA,10329
+benchq/problem_embeddings/qsp/get_qsp_phases.py,sha256=giz4KV7_xwL3C6G6LT1aXkl459ZJ7DbiWB0RqxnYkDI,15077
+benchq/problem_embeddings/qsp/get_qsp_polynomial.py,sha256=4GwXDfRr0iRGy6lhVx7K34YzQfzygVnayXXzjm0IQhk,4694
+benchq/problem_embeddings/time_marching/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+benchq/problem_embeddings/time_marching/_time_marching.py,sha256=1napy-ni2dYElyM3kWMRqay2wC0QQwSFr_mIxd8FmeM,11598
+benchq/problem_embeddings/time_marching/compression_gadget.py,sha256=nhZWzF9puOpxp3FRkHKKriCFKP8F45xpiiZZT2Qwxtk,550
+benchq/problem_embeddings/time_marching/matrix_properties.py,sha256=pOqJEq53YaHczMUfePYeiawayBLf0IS3fXcsmyEkGR8,2605
+benchq/problem_ingestion/__init__.py,sha256=6OQQegLTQk7AxTOU6IKbvRh3l0f-u0hfG2tuXtT6Vh8,483
+benchq/problem_ingestion/hamiltonian_from_file.py,sha256=LKROxMrWJdgC1rB-ZQzkWuQYrAj8llDoO0bmfbyYoX4,6942
+benchq/problem_ingestion/molecular_hamiltonians/__init__.py,sha256=NiijW5syHClkBta6BoPP4FNW8P3s8F1XRsrONadvnvE,510
+benchq/problem_ingestion/molecular_hamiltonians/_common_molecules.py,sha256=4tu-T_givN-UWue1VJdMaZqxwJvDoDwGev5X4Q66w9M,3212
+benchq/problem_ingestion/molecular_hamiltonians/_compute_lambda.py,sha256=jGH5YBTvXCk7ezLaD52TkMGYUenpG7CwCFDkoj9XFRk,2775
+benchq/problem_ingestion/molecular_hamiltonians/_hamiltonian_generation.py,sha256=hnZQR3_EtghGiHdjkZkwGMec0fCdvZjW5F9TS8nWeQw,20976
+benchq/problem_ingestion/plasma_hamiltonians/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+benchq/problem_ingestion/plasma_hamiltonians/vlasov.py,sha256=V4BFt_tqU8UtRLiTMKD-jyiGW14WiGnWL6egYggn_Uw,887
+benchq/problem_ingestion/solid_state_hamiltonians/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+benchq/problem_ingestion/solid_state_hamiltonians/fermi_hubbard.py,sha256=Cx9d9EGwVRsKOUSuBTXsKYmgxECL_Vmb0vNR8WJA_EY,872
+benchq/problem_ingestion/solid_state_hamiltonians/heisenberg.py,sha256=DYn0pnMpGQFrV6d4wAiklozmO-E_N-CALSp1G0Tuso0,1429
+benchq/problem_ingestion/solid_state_hamiltonians/ising.py,sha256=jCiBWnk1raQfXwIAvKFxkQwtHHS-iKXpbHNcVc7Cnj8,4267
+benchq/quantum_hardware_modeling/__init__.py,sha256=Vc7GjOXkWoL1U0PiWLEtha3gl-xbB1pN4cYIF0i2hvs,245
+benchq/quantum_hardware_modeling/devitt_surface_code.py,sha256=iFxLYYYfvm-ORHw_0XgK6n3xLluLWqHwGPp5SCiL5bg,1317
+benchq/quantum_hardware_modeling/fowler_surface_code.py,sha256=Ngy6190HBaRDxrWerdMic2rRWhaVgHG1MbTf946RlZ4,892
+benchq/quantum_hardware_modeling/hardware_architecture_models.py,sha256=ZuTPvEVyktDjUhFcS1LUdCRBr9hJ59QfZUTdRsRKucg,9024
+benchq/resource_estimators/__init__.py,sha256=ydDH-h6FdSuwZqFndB5SMkTE9dY0ysU7KHtxSFefnbs,204
+benchq/resource_estimators/azure_estimator.py,sha256=EATS3KVdYuiNugD_papLEPZVqrBjZDG7sQVH4TupAVA,4985
+benchq/resource_estimators/default_estimators.py,sha256=1e_MIeNJGMkO2mB6U4r0oCKCy5LqMLtm0_ZB0RSsnUw,12376
+benchq/resource_estimators/resource_info.py,sha256=vfTWhp2tSlgOgBVfnA8xeW8saHW9gQgW3WuzSbyj-EU,3766
+benchq/resource_estimators/footprint_estimators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+benchq/resource_estimators/footprint_estimators/openfermion_estimator.py,sha256=xnakoC0SNNxkuAPZzKAV7BjXf4r8Ar1JMODLJPpxSS4,8985
+benchq/resource_estimators/graph_estimators/__init__.py,sha256=Y-HjaZoRlOh1PE5koFMSkTjq_Jts5c-saYm45M5gjuI,707
+benchq/resource_estimators/graph_estimators/customizable_pipelines.py,sha256=iRFZHHJenQ472DUvExmyEp9WBEWZXq8DjadvWrX7OTo,3984
+benchq/resource_estimators/graph_estimators/extrapolation_estimator.py,sha256=Sgg741KS93H9Ix8WLwAY-b02aL3AMH-txeF3Qb7-7hw,8723
+benchq/resource_estimators/graph_estimators/graph_estimator.py,sha256=zpgAtnxUmDeXQ70Uru9jsFvXXn0MMBfHro9mDG6yDWw,18493
+benchq/resource_estimators/graph_estimators/transformers.py,sha256=BQDoGS1C7vB1ZeUmSb2fuWu7RvC0bs1OtjvZszgSanM,4908
+benchq-0.7.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+benchq-0.7.0.dist-info/METADATA,sha256=vM6MpD7SzOEb46ej0CMMcL_S73NFUOnSgNSULWvUIcs,7465
+benchq-0.7.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+benchq-0.7.0.dist-info/top_level.txt,sha256=RGAPdCRmbLQ_m241jwm5Q75qzuaWjICnIa16V6jkerE,7
+benchq-0.7.0.dist-info/RECORD,,
```

