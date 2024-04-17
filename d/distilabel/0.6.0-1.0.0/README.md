# Comparing `tmp/distilabel-0.6.0.tar.gz` & `tmp/distilabel-1.0.0.tar.gz`

## Comparing `distilabel-0.6.0.tar` & `distilabel-1.0.0.tar`

### file list

```diff
@@ -1,211 +1,253 @@
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 distilabel-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 distilabel-0.6.0/Makefile
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 distilabel-0.6.0/mkdocs.yml
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 distilabel-0.6.0/.github/ISSUE_TEMPLATE/blank-issue-template.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 distilabel-0.6.0/.github/ISSUE_TEMPLATE/🆕-feature-request.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 distilabel-0.6.0/.github/ISSUE_TEMPLATE/🐛-bug-report.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 distilabel-0.6.0/.github/ISSUE_TEMPLATE/📚-documentation-update.md
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 distilabel-0.6.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 distilabel-0.6.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 distilabel-0.6.0/.github/workflows/test.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/CNAME
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/concepts.md
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/index.md
--rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/assets/distilabel-badge-dark.png
--rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/assets/distilabel-badge-light.png
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/assets/distilabel-icon.svg
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/assets/logo.svg
--rw-r--r--   0        0        0    47284 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/assets/images/distilabel-diagram-dark.svg
--rw-r--r--   0        0        0    47244 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/assets/images/distilabel-diagram.svg
--rw-r--r--   0        0        0   173971 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png
--rw-r--r--   0        0        0   356586 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/assets/tutorials-assets/preference_dataset_notus_ui.png
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/scripts/gen_ref_pages.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/quick-example.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/concepts/llm.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/concepts/pipeline-only-generator.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/concepts/pipeline-only-labeller.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/concepts/pipeline.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/concepts/task.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/guides/self-instruct.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/llm/anyscale_generate.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/llm/inference_endpoint_generate.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/llm/llamacpp_generate.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/llm/llmpool.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/llm/mistralai_generate.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/llm/ollama_generate.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/llm/openai_generate.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/llm/openai_json_generate.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/llm/processllm.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/llm/together_inference_generate.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/llm/transformers_generate.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/llm/validate_prompts_1.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/llm/validate_prompts_2.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/llm/vertexaiendpointllm_generate.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/llm/vertexaillm_generate.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/llm/vllm_generate.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/argilla.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/load_dataset.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipe_1.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipe_2.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipe_3.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_dataset_checkpoint_1.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_dataset_checkpoint_2.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_dataset_checkpoint_3.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_dataset_checkpoint_4.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_generator_1.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_generator_2.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_generator_3.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_labeller_1.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_labeller_2.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_labeller_3.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_labeller_generator_1.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_labeller_generator_2.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_labeller_generator_3.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_llmpool_processllm_1.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_llmpool_processllm_2.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_llmpool_processllm_3.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_llmpool_processllm_4.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/pipeline_llmpool_processllm_5.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/prepare_dataset_binarize_random.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/prepare_dataset_binarize_worst.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/pipeline/push_to_hub.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/complexity_scorer_example.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/custom_task_selfinstruct_haikus_docs.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/custom_task_text_generation_oss.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/custom_task_text_generation_wizardlm.py
--rw-r--r--   0        0        0     7488 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/evol_quality_example.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/generic_openai_complexity_scorer.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/generic_openai_evol_complexity.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/generic_openai_evol_instruct.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/generic_openai_evol_quality.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/generic_openai_quality_scorer.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/generic_openai_quality_scorer_custom.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/generic_openai_self_instruct.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/generic_transformersllm.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/openai_for_helpfulness.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/openai_for_honesty.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/openai_for_instruction_following.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/openai_for_overall_quality.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/openai_for_truthfulness.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/openai_judgelm.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/openai_ultrajudge.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/prometheus.py
--rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/quality_scorer_example.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/ultracm.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/ultrafeedback.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/snippets/technical-reference/tasks/ultrajudge.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/technical-reference/index.md
--rw-r--r--   0        0        0    14180 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/technical-reference/llms.md
--rw-r--r--   0        0        0    21913 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/technical-reference/pipeline.md
--rw-r--r--   0        0        0    20610 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/technical-reference/tasks.md
--rw-r--r--   0        0        0  2658957 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/tutorials/clean-preference-dataset-judgelm-gpt.ipynb
--rw-r--r--   0        0        0   173441 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/tutorials/create-a-math-preference-dataset.ipynb
--rw-r--r--   0        0        0   311286 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/tutorials/create-evol-instruct-dataset.ipynb
--rw-r--r--   0        0        0   156174 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/tutorials/improving-text-embeddings-with-llms.ipynb
--rw-r--r--   0        0        0    50698 2020-02-02 00:00:00.000000 distilabel-0.6.0/docs/tutorials/pipeline-notus-instructions-preferences-legal.ipynb
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/inference-endpoints-llm-custom-task.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-accelerate-and-openai.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-anyscale-endpoints.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-evol-instruct-alpaca.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-fn-ultrafeedback-labeller.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-fn-ultrafeedback.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-llamacpp-and-openai-process.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-llamacpp-and-openai.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-ollama.py
--rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-openai-wizardlm-equal-prompts.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-pool-llm.py
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-preference-dataset-llmpool.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-prometheus.py
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-selfinstruct-math-openai.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-together-inference.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-transformers-and-openai.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-ultracm.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 distilabel-0.6.0/examples/pipeline-vllm-and-openai.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/__init__.py
--rw-r--r--   0        0        0    18141 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/dataset.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/logger.py
--rw-r--r--   0        0        0    36720 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/pipeline.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/progress_bar.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/llm/__init__.py
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/llm/anyscale.py
--rw-r--r--   0        0        0    34515 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/llm/base.py
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/llm/llama_cpp.py
--rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/llm/mistralai.py
--rw-r--r--   0        0        0    11401 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/llm/ollama.py
--rw-r--r--   0        0        0    14556 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/llm/openai.py
--rw-r--r--   0        0        0    10360 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/llm/together.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/llm/utils.py
--rw-r--r--   0        0        0     6834 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/llm/vllm.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/llm/google/__init__.py
--rw-r--r--   0        0        0    20029 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/llm/google/vertexai.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/llm/huggingface/__init__.py
--rw-r--r--   0        0        0    10335 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/llm/huggingface/inference_endpoints.py
--rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/llm/huggingface/transformers.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/__init__.py
--rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/base.py
--rw-r--r--   0        0        0    10085 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/mixins.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/prompt.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/_internal/stopwords_en.txt
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/_templates/complexity-scorer.jinja2
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/_templates/evol-instruct.jinja2
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/_templates/evol-quality.jinja2
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/_templates/judgelm.jinja2
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/_templates/prometheus.jinja2
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/_templates/quality-scorer.jinja2
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/_templates/self-instruct.jinja2
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/_templates/ultracm.jinja2
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/_templates/ultrafeedback.jinja2
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/_templates/ultrajudge.jinja2
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/critique/__init__.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/critique/base.py
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/critique/prometheus.py
--rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/critique/ultracm.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/preference/__init__.py
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/preference/base.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/preference/complexity_scorer.py
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/preference/judgelm.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/preference/quality_scorer.py
--rw-r--r--   0        0        0    17756 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/preference/ultrafeedback.py
--rw-r--r--   0        0        0     7785 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/preference/ultrajudge.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/text_generation/__init__.py
--rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/text_generation/base.py
--rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/text_generation/evol_complexity.py
--rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/text_generation/evol_instruct.py
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/text_generation/evol_quality.py
--rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/text_generation/mixins.py
--rw-r--r--   0        0        0    10098 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/text_generation/principles.py
--rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/tasks/text_generation/self_instruct.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/utils/__init__.py
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/utils/argilla.py
--rw-r--r--   0        0        0    13511 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/utils/dataset.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/utils/dicts.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/utils/futures.py
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/utils/imports.py
--rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/utils/serialization.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 distilabel-0.6.0/src/distilabel/utils/types.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0    31217 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/test_dataset.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/test_pipeline.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/llm/__init__.py
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/llm/test_anyscale.py
--rw-r--r--   0        0        0    10380 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/llm/test_base.py
--rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/llm/test_mistralai.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/llm/test_ollama.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/llm/test_openai.py
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/llm/test_together.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/llm/google/__init__.py
--rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/llm/google/test_vertexai.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/tasks/__init__.py
--rw-r--r--   0        0        0     8927 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/tasks/test_serialization.py
--rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/tasks/preference/test_evol_scorer.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/tasks/text_generation/__init__.py
--rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/tasks/text_generation/test_base.py
--rw-r--r--   0        0        0    12475 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/tasks/text_generation/test_evol_tasks.py
--rw-r--r--   0        0        0    14507 2020-02-02 00:00:00.000000 distilabel-0.6.0/tests/tasks/text_generation/test_self_instruct.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 distilabel-0.6.0/.gitignore
--rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 distilabel-0.6.0/LICENSE
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 distilabel-0.6.0/LICENSE_HEADER
--rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 distilabel-0.6.0/README.md
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 distilabel-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     9063 2020-02-02 00:00:00.000000 distilabel-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 distilabel-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 distilabel-1.0.0/Makefile
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 distilabel-1.0.0/mkdocs.yml
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 distilabel-1.0.0/.github/ISSUE_TEMPLATE/blank-issue-template.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 distilabel-1.0.0/.github/ISSUE_TEMPLATE/🆕-feature-request.md
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 distilabel-1.0.0/.github/ISSUE_TEMPLATE/🐛-bug-report.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 distilabel-1.0.0/.github/ISSUE_TEMPLATE/📚-documentation-update.md
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 distilabel-1.0.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 distilabel-1.0.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 distilabel-1.0.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/CNAME
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/index.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/overview.md
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/cli.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/anthropic.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/anyscale.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/azure.md
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/huggingface.md
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/litellm.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/llamacpp.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/mistral.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/ollama.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/openai.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/together.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/vertexai.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/llms/vllm.md
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/pipeline/pipeline.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/argilla.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/decorator.md
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/extra.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/steps.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/generator_steps/generator_steps.md
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/global_steps/global_steps.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/tasks/embeddings.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/tasks/preference_tasks.md
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/api/steps/tasks/text_generation.md
+-rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/distilabel-badge-dark.png
+-rw-r--r--   0        0        0    15551 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/distilabel-badge-light.png
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/distilabel-icon.svg
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/logo.svg
+-rw-r--r--   0        0        0    47284 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/distilabel-diagram-dark.svg
+-rw-r--r--   0        0        0    47244 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/distilabel-diagram.svg
+-rw-r--r--   0        0        0   301103 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/sections/caching/caching_pipe_1.png
+-rw-r--r--   0        0        0   329256 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/sections/caching/caching_pipe_2.png
+-rw-r--r--   0        0        0   129190 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/sections/caching/caching_pipe_3.png
+-rw-r--r--   0        0        0    24695 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/sections/caching/caching_pipe_4.png
+-rw-r--r--   0        0        0   368245 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/sections/cli/cli_pipe.png
+-rw-r--r--   0        0        0  1290074 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/sections/learn/steps/argilla/preference.png
+-rw-r--r--   0        0        0  1014081 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/images/sections/learn/steps/argilla/text_generation.png
+-rw-r--r--   0        0        0   173971 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png
+-rw-r--r--   0        0        0   356586 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/tutorials-assets/preference_dataset_notus_ui.png
+-rw-r--r--   0        0        0    19151 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/tutorials-assets/deita/datasets.png
+-rw-r--r--   0        0        0    96338 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/tutorials-assets/deita/diversity.png
+-rw-r--r--   0        0        0   191403 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/tutorials-assets/deita/overview.png
+-rw-r--r--   0        0        0    94813 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/assets/tutorials-assets/deita/results.png
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/scripts/gen_ref_pages.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/caching.md
+-rw-r--r--   0        0        0     7963 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/cli.md
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/distiset.md
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/index.md
+-rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/llms/index.md
+-rw-r--r--   0        0        0    14338 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/pipelines/index.md
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/steps/argilla.md
+-rw-r--r--   0        0        0     8669 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/steps/general_steps.md
+-rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/steps/generator_steps.md
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/steps/global_steps.md
+-rw-r--r--   0        0        0     8491 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/steps/index.md
+-rw-r--r--   0        0        0     7803 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/tasks/feedback_tasks.md
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/tasks/index.md
+-rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/tasks/special_tasks.md
+-rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/learn/tasks/text_generation.md
+-rw-r--r--   0        0        0    21822 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/papers/deita.md
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/papers/index.md
+-rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/papers/instruction_backtranslation.md
+-rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/sections/papers/ultrafeedback.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 distilabel-1.0.0/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/__main__.py
+-rw-r--r--   0        0        0     9461 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/distiset.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/cli/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/cli/app.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/cli/pipeline/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/cli/pipeline/app.py
+-rw-r--r--   0        0        0     8197 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/cli/pipeline/utils.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/__init__.py
+-rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/anthropic.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/anyscale.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/azure.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/base.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/chat_templates.py
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/cohere.py
+-rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/litellm.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/llamacpp.py
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/mistral.py
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/mixins.py
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/ollama.py
+-rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/openai.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/together.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/typing.py
+-rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/vertexai.py
+-rw-r--r--   0        0        0     7200 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/vllm.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/huggingface/__init__.py
+-rw-r--r--   0        0        0    15077 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/huggingface/inference_endpoints.py
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/llms/huggingface/transformers.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/mixins/__init__.py
+-rw-r--r--   0        0        0     6971 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/mixins/runtime_parameters.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/pipeline/__init__.py
+-rw-r--r--   0        0        0    17954 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/pipeline/_dag.py
+-rw-r--r--   0        0        0    37076 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/pipeline/base.py
+-rw-r--r--   0        0        0    32476 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/pipeline/local.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/pipeline/utils.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/__init__.py
+-rw-r--r--   0        0        0    19355 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/base.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/combine.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/conversation.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/decorator.py
+-rw-r--r--   0        0        0     9152 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/deita.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/expand.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/keep.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/typing.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/argilla/__init__.py
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/argilla/base.py
+-rw-r--r--   0        0        0    10934 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/argilla/preference.py
+-rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/argilla/text_generation.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/generators/__init__.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/generators/data.py
+-rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/generators/huggingface.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/globals/__init__.py
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/globals/huggingface.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/__init__.py
+-rw-r--r--   0        0        0     6966 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/base.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/complexity_scorer.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/generate_embeddings.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/instruction_backtranslation.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/pair_rm.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/quality_scorer.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/self_instruct.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/text_generation.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/typing.py
+-rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/ultrafeedback.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/__init__.py
+-rw-r--r--   0        0        0    12081 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/base.py
+-rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/english_nouns.txt
+-rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/generator.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/base.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/generator.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_quality/__init__.py
+-rw-r--r--   0        0        0     9098 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_quality/base.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/evol_quality/utils.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/templates/instruction-backtranslation.jinja2
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/templates/self-instruct.jinja2
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/templates/ultrafeedback/helpfulness.jinja2
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/templates/ultrafeedback/honesty.jinja2
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/templates/ultrafeedback/instruction-following.jinja2
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/templates/ultrafeedback/overall-rating.jinja2
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/steps/tasks/templates/ultrafeedback/truthfulness.jinja2
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/__init__.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/chat.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/dicts.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/docstring.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/files.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/itertools.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/lists.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/logging.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/notebook.py
+-rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/serialization.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/typing_.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/card/__init__.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/card/dataset_card.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 distilabel-1.0.0/src/distilabel/utils/card/distilabel_template.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/integration/test_pipe_llms.py
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/integration/test_pipe_simple.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/test_distiset.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/test_imports.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/cli/__init__.py
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/cli/test_pipeline.yaml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/cli/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/cli/pipeline/__init__.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/cli/pipeline/test_app.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/cli/pipeline/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/__init__.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_anthropic.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_anyscale.py
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_azure.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_cohere.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_litellm.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_llamacpp.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_mistral.py
+-rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_mixins.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_ollama.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_openai.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_together.py
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/test_vertexai.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/huggingface/__init__.py
+-rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/huggingface/test_inference_endpoints.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/llms/huggingface/test_transformers.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/mixins/__init__.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/mixins/test_runtime_parameters.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/pipeline/__init__.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/pipeline/conftest.py
+-rw-r--r--   0        0        0    44539 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/pipeline/test_base.py
+-rw-r--r--   0        0        0    17227 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/pipeline/test_dag.py
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/pipeline/test_local.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/pipeline/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/__init__.py
+-rw-r--r--   0        0        0     9554 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/test_base.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/test_combine.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/test_conversation.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/test_decorator.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/test_deita.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/test_expand.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/test_keep.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/argilla/__init__.py
+-rw-r--r--   0        0        0     5814 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/argilla/test_base.py
+-rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/argilla/test_preference.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/argilla/test_text_generation.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/generators/test_data.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/__init__.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/conftest.py
+-rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_base.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_complexity_scorer.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_generate_embeddings.py
+-rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_instruction_backtranslation.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_pair_rm.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_quality_scorer.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_self_instruct.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_text_generation.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/test_ultrafeedback.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/utils.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/__init__.py
+-rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/test_base.py
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/test_generator.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/__init__.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_base.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/evol_complexity.py/test_generator.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/evol_quality/__init__.py
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/steps/tasks/evol_quality/test_base.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/utils/test_chat.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/utils/test_docstring.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/utils/test_lists.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 distilabel-1.0.0/tests/unit/utils/test_typing.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 distilabel-1.0.0/.gitignore
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 distilabel-1.0.0/LICENSE
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 distilabel-1.0.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     9299 2020-02-02 00:00:00.000000 distilabel-1.0.0/README.md
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 distilabel-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    12494 2020-02-02 00:00:00.000000 distilabel-1.0.0/PKG-INFO
```

### Comparing `distilabel-0.6.0/.github/ISSUE_TEMPLATE/🆕-feature-request.md` & `distilabel-1.0.0/.github/ISSUE_TEMPLATE/🆕-feature-request.md`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/.github/ISSUE_TEMPLATE/🐛-bug-report.md` & `distilabel-1.0.0/.github/ISSUE_TEMPLATE/🐛-bug-report.md`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/.github/ISSUE_TEMPLATE/📚-documentation-update.md` & `distilabel-1.0.0/.github/ISSUE_TEMPLATE/📚-documentation-update.md`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/.github/workflows/docs.yml` & `distilabel-1.0.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/.github/workflows/release.yml` & `distilabel-1.0.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/docs/assets/distilabel-badge-dark.png` & `distilabel-1.0.0/docs/assets/distilabel-badge-dark.png`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/docs/assets/distilabel-badge-light.png` & `distilabel-1.0.0/docs/assets/distilabel-badge-light.png`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/docs/assets/distilabel-icon.svg` & `distilabel-1.0.0/docs/assets/distilabel-icon.svg`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/docs/assets/logo.svg` & `distilabel-1.0.0/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/docs/assets/images/distilabel-diagram-dark.svg` & `distilabel-1.0.0/docs/assets/images/distilabel-diagram-dark.svg`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/docs/assets/images/distilabel-diagram.svg` & `distilabel-1.0.0/docs/assets/images/distilabel-diagram.svg`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png` & `distilabel-1.0.0/docs/assets/tutorials-assets/instrucion_dataset_notus_ui.png`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/docs/assets/tutorials-assets/preference_dataset_notus_ui.png` & `distilabel-1.0.0/docs/assets/tutorials-assets/preference_dataset_notus_ui.png`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/docs/scripts/gen_ref_pages.py` & `distilabel-1.0.0/docs/scripts/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/examples/pipeline-ollama.py` & `distilabel-1.0.0/tests/unit/steps/generators/test_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,66 +7,44 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import pytest
+from distilabel.pipeline.local import Pipeline
+from distilabel.steps.generators.data import LoadDataFromDicts
+from pydantic import ValidationError
 
-import os
 
-from datasets import load_dataset
-from distilabel.llm import OllamaLLM
-from distilabel.pipeline import Pipeline
-from distilabel.tasks import TextGenerationTask
-
-if __name__ == "__main__":
-    dataset = (
-        load_dataset("HuggingFaceH4/instruction-dataset", split="test[:10]")
-        .remove_columns(["completion", "meta"])
-        .rename_column("prompt", "input")
-    )
-
-    pipeline = Pipeline(
-        generator=OllamaLLM(
-            model="mistral",  # should be deployed separately via https://github.com/jmorganca/ollama
-            task=TextGenerationTask(),
-            max_new_tokens=128,
-            temperature=0.3,
-            prompt_format="openai",
+class TestLoadDataFromDictsTask:
+    data = [{"instruction": "test"}] * 10
+
+    def test_init(self) -> None:
+        pipeline = Pipeline(name="unit-test-pipeline")
+        data: list[dict[str, str]] = self.data
+        task = LoadDataFromDicts(
+            name="task", pipeline=pipeline, data=data, batch_size=10
         )
-    )
+        assert task.data == data
+        assert task.batch_size == 10
 
-    dataset = pipeline.generate(
-        dataset,  # type: ignore
-        num_generations=2,
-        batch_size=1,
-        checkpoint_strategy=False,
-        display_progress_bar=True,
-    )
-
-    # Push to the HuggingFace Hub
-    dataset.push_to_hub(
-        os.getenv("HF_REPO_ID"),  # type: ignore
-        split="train",
-        private=True,
-        token=os.getenv("HF_TOKEN", None),
-    )
-
-    try:
-        from uuid import uuid4
-
-        import argilla as rg
-
-        rg.init(
-            api_url=os.getenv("ARGILLA_API_URL"),
-            api_key=os.getenv("ARGILLA_API_KEY"),
+    def test_with_errors(self) -> None:
+        pipeline = Pipeline(name="unit-test-pipeline")
+        with pytest.raises(ValidationError):
+            LoadDataFromDicts(name="task", pipeline=pipeline)
+
+    def test_process(self) -> None:
+        pipeline = Pipeline(name="unit-test-pipeline")
+        data: list[dict[str, str]] = self.data
+        batch_size = 1
+        task = LoadDataFromDicts(
+            name="task", pipeline=pipeline, data=data, batch_size=batch_size
         )
 
-        # Convert into an Argilla dataset and push it to Argilla
-        rg_dataset = dataset.to_argilla()
-        rg_dataset.push_to_argilla(
-            name=f"my-dataset-{uuid4()}",
-            workspace="admin",
-        )
-    except ImportError:
-        pass
+        result = task.process()
+        for i in range(len(self.data) - batch_size):
+            assert next(result) == ([self.data[i]], False)
+        assert next(result) == ([self.data[-batch_size]], True)
+        with pytest.raises(StopIteration):
+            next(result)
```

### Comparing `distilabel-0.6.0/examples/pipeline-prometheus.py` & `distilabel-1.0.0/tests/unit/steps/tasks/test_self_instruct.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,56 +8,44 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
+from distilabel.pipeline.local import Pipeline
+from distilabel.steps.tasks.self_instruct import SelfInstruct
 
-import torch
-from datasets import Dataset
-from distilabel.llm import TransformersLLM
-from distilabel.pipeline import Pipeline
-from distilabel.tasks import PrometheusTask
-from transformers import AutoTokenizer, LlamaForCausalLM
-
-if __name__ == "__main__":
-    model = LlamaForCausalLM.from_pretrained(
-        "kaist-ai/Prometheus-7b-v1.0", torch_dtype=torch.float16, device_map="auto"
-    )
-    tokenizer = AutoTokenizer.from_pretrained(
-        "meta-llama/Llama-2-7b-chat-hf", token=os.getenv("HF_TOKEN")
-    )
-    pipeline = Pipeline(
-        labeller=TransformersLLM(
-            model=model,  # type: ignore
-            tokenizer=tokenizer,
-            task=PrometheusTask(
-                scoring_criteria="Is the provided completion accurate based on the given instruction?",
-                score_descriptions={
-                    0: "Totaly off-topic and inaccurate",
-                    1: "Incorrect and inaccurate",
-                    2: "Almost correct, but partially inaccurate",
-                    3: "Correct but badly phrased",
-                    4: "Correct and accurate",
-                },
-            ),
-            temperature=1.0,
-            top_p=1.0,
-            max_new_tokens=512,
-        ),
-    )
-
-    dataset = Dataset.from_dict(
-        {
-            "input": ["What's the capital of Spain?"],
-            "generations": ["Paris"],
-            "ref_completion": ["Madrid"],
-        }
-    )
+from tests.unit.steps.tasks.utils import DummyLLM
+
+
+class TestSelfInstruct:
+    def test_format_input(self) -> None:
+        task = SelfInstruct(
+            name="self_instruct",
+            llm=DummyLLM(),
+            pipeline=Pipeline(name="unit-test-pipeline"),
+        )
+        task.load()
 
-    dataset = pipeline.generate(
-        dataset,  # type: ignore
-        display_progress_bar=True,
-        skip_dry_run=True,
-    )
+        input = task.format_input(input={"input": "test"})
+        assert input == [
+            {
+                "role": "user",
+                "content": '# Task Description\nDevelop 5 user queries that can be received by the given AI application and applicable to the provided context. Emphasize diversity in verbs and linguistic structures within the model\'s textual capabilities.\n\n# Criteria for Queries\nIncorporate a diverse range of verbs, avoiding repetition.\nEnsure queries are compatible with AI model\'s text generation functions and are limited to 1-2 sentences.\nDesign queries to be self-contained and standalone.\nBlend interrogative (e.g., "What is the significance of x?") and imperative (e.g., "Detail the process of x.") styles.\nWrite each query on a separate line and avoid using numbered lists or bullet points.\n\n# AI Application\nAI assistant\n\n# Context\ntest\n\n# Output\n',
+            }
+        ]
+
+    def test_format_output(self) -> None:
+        task = SelfInstruct(
+            name="self_instruct",
+            llm=DummyLLM(),
+            pipeline=Pipeline(name="unit-test-pipeline"),
+        )
+        task.load()
+
+        output = task.format_output(
+            output="Instruction 1\n\nInstruction 2\n\nInstruction 3"
+        )
+        assert output == {
+            "instructions": ["Instruction 1", "Instruction 2", "Instruction 3"]
+        }
```

### Comparing `distilabel-0.6.0/src/distilabel/__init__.py` & `distilabel-1.0.0/src/distilabel/cli/pipeline/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from distilabel.cli.pipeline.app import app
 
-__version__ = "0.6.0"
+__all__ = ["app"]
```

### Comparing `distilabel-0.6.0/src/distilabel/llm/openai.py` & `distilabel-1.0.0/src/distilabel/llms/huggingface/inference_endpoints.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,340 +8,370 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import json
-import warnings
-from functools import cached_property
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Dict,
-    Generator,
-    List,
-    Union,
+import asyncio
+import os
+from typing import TYPE_CHECKING, Any, List, Optional, Union
+
+from pydantic import (
+    Field,
+    PrivateAttr,
+    SecretStr,
+    ValidationError,
+    model_validator,
+    validate_call,
 )
+from typing_extensions import override
 
-from distilabel.llm.base import LLM
-from distilabel.llm.utils import LLMOutput
-from distilabel.logger import get_logger
-from distilabel.utils.imports import _OPENAI_AVAILABLE
-
-if _OPENAI_AVAILABLE:
-    from openai import OpenAI
+from distilabel.llms.base import AsyncLLM
+from distilabel.llms.typing import GenerateOutput
+from distilabel.mixins.runtime_parameters import RuntimeParameter
+from distilabel.steps.tasks.typing import ChatType
+from distilabel.utils.itertools import grouper
 
 if TYPE_CHECKING:
-    from distilabel.tasks.base import Task
-    from distilabel.tasks.prompt import SupportedFormats
+    from huggingface_hub import AsyncInferenceClient
+    from openai import AsyncOpenAI
+    from transformers import PreTrainedTokenizer
+
+
+_INFERENCE_ENDPOINTS_API_KEY_ENV_VAR_NAME = "HF_TOKEN"
+
+
+class InferenceEndpointsLLM(AsyncLLM):
+    """InferenceEndpoints LLM implementation running the async API client via either
+    the `huggingface_hub.AsyncInferenceClient` or via `openai.AsyncOpenAI`.
+
+    Attributes:
+        model_id: the model ID to use for the LLM as available in the Hugging Face Hub, which
+            will be used to resolve the base URL for the serverless Inference Endpoints API requests.
+            Defaults to `None`.
+        endpoint_name: the name of the Inference Endpoint to use for the LLM. Defaults to `None`.
+        endpoint_namespace: the namespace of the Inference Endpoint to use for the LLM. Defaults to `None`.
+        base_url: the base URL to use for the Inference Endpoints API requests.
+        api_key: the API key to authenticate the requests to the Inference Endpoints API.
+        tokenizer_id: the tokenizer ID to use for the LLM as available in the Hugging Face Hub.
+            Defaults to `None`, but defining one is recommended to properly format the prompt.
+        model_display_name: the model display name to use for the LLM. Defaults to `None`.
+        use_openai_client: whether to use the OpenAI client instead of the Hugging Face client.
+
+    Examples:
+        ```python
+        from distilabel.llms.huggingface import InferenceEndpointsLLM
+
+
+        # Free serverless Inference API
+        llm = InferenceEndpointsLLM(
+            model_id="mistralai/Mistral-7B-Instruct-v0.2",
+        )
 
-logger = get_logger()
+        # Dedicated Inference Endpoints
+        llm = InferenceEndpointsLLM(
+            endpoint_name="<ENDPOINT_NAME>",
+            api_key="<HF_API_KEY>",
+            endpoint_namespace="<USER|ORG>",
+        )
+
+        # Dedicated Inference Endpoints or TGI
+        llm = InferenceEndpointsLLM(
+            api_key="<HF_API_KEY>",
+            base_url="<BASE_URL>",
+        )
 
+        llm.load()
 
-class OpenAILLM(LLM):
-    def __init__(
+        # Synchrounous request
+        output = llm.generate(inputs=[[{"role": "user", "content": "Hello world!"}]])
+
+        # Asynchronous request
+        output = await llm.agenerate(input=[{"role": "user", "content": "Hello world!"}])
+        ```
+    """
+
+    model_id: Optional[str] = None
+
+    endpoint_name: Optional[RuntimeParameter[str]] = Field(
+        default=None,
+        description="The name of the Inference Endpoint to use for the LLM.",
+    )
+    endpoint_namespace: Optional[RuntimeParameter[str]] = Field(
+        default=None,
+        description="The namespace of the Inference Endpoint to use for the LLM.",
+    )
+    base_url: Optional[RuntimeParameter[str]] = Field(
+        default=None,
+        description="The base URL to use for the Inference Endpoints API requests.",
+    )
+    api_key: Optional[RuntimeParameter[SecretStr]] = Field(
+        default=os.getenv(_INFERENCE_ENDPOINTS_API_KEY_ENV_VAR_NAME),
+        description="The API key to authenticate the requests to the Inference Endpoints API.",
+    )
+
+    tokenizer_id: Optional[str] = None
+    model_display_name: Optional[str] = None
+    use_openai_client: bool = False
+
+    _model_name: Optional[str] = PrivateAttr(default=None)
+    _tokenizer: Optional["PreTrainedTokenizer"] = PrivateAttr(default=None)
+    _api_key_env_var: str = PrivateAttr(_INFERENCE_ENDPOINTS_API_KEY_ENV_VAR_NAME)
+    _aclient: Optional[Union["AsyncInferenceClient", "AsyncOpenAI"]] = PrivateAttr(...)
+
+    @model_validator(mode="after")  # type: ignore
+    def only_one_of_model_id_endpoint_name_or_base_url_provided(
         self,
-        task: "Task",
-        model: str = "gpt-3.5-turbo",
-        client: Union["OpenAI", None] = None,
-        api_key: Union[str, None] = None,
-        max_new_tokens: int = 128,
-        frequency_penalty: float = 0.0,
-        presence_penalty: float = 0.0,
-        temperature: float = 1.0,
-        top_p: float = 1.0,
-        num_threads: Union[int, None] = None,
-        prompt_format: Union["SupportedFormats", None] = None,
-        prompt_formatting_fn: Union[Callable[..., str], None] = None,
-    ) -> None:
-        """Initializes the OpenAILLM class.
+    ) -> "InferenceEndpointsLLM":
+        """Validates that only one of `model_id`, `endpoint_name`, or `base_url` is provided."""
 
-        Args:
-            task (Task): the task to be performed by the LLM.
-            model (str, optional): the model to be used for generation. Defaults to "gpt-3.5-turbo".
-            client (Union[OpenAI, None], optional): an OpenAI client to be used for generation.
-                If `None`, a new client will be created. Defaults to `None`.
-            api_key (Union[str, None], optional): the OpenAI API key to be used for generation.
-                If `None`, the `OPENAI_API_KEY` environment variable will be used. Defaults to `None`.
-            max_new_tokens (int, optional): the maximum number of tokens to be generated.
-                Defaults to 128.
-            frequency_penalty (float, optional): the frequency penalty to be used for generation.
-                Defaults to 0.0.
-            presence_penalty (float, optional): the presence penalty to be used for generation.
-                Defaults to 0.0.
-            temperature (float, optional): the temperature to be used for generation.
-                Defaults to 1.0.
-            top_p (float, optional): the top-p value to be used for generation.
-                Defaults to 1.0.
-            num_threads (Union[int, None], optional): the number of threads to be used
-                for parallel generation. If `None`, no parallel generation will be performed.
-                Defaults to `None`.
-            prompt_format (Union[SupportedFormats, None], optional): the format to be used
-                for the prompt. If `None`, the default format of the task will be used, available
-                formats are `openai`, `chatml`, `llama2`, `zephyr`, and `default`. Defaults to `None`,
-                but `default` (concatenation of `system_prompt` and `formatted_prompt` with a line-break)
-                will be used if no `prompt_formatting_fn` is provided.
-            prompt_formatting_fn (Union[Callable[..., str], None], optional): a function to be
-                applied to the prompt before generation. If `None`, no formatting will be applied.
-                Defaults to `None`.
+        if self.model_id and (not self.endpoint_name and not self.base_url):
+            return self
 
-        Raises:
-            AssertionError: if the provided `model` is not available in your OpenAI account.
+        if self.endpoint_name and (not self.model_id and not self.base_url):
+            return self
 
-        Examples:
-            >>> from distilabel.tasks import TextGenerationTask
-            >>> from distilabel.llm import OpenAILLM
-            >>> llm = OpenAILLM(model="gpt-3.5-turbo", task=TextGenerationTask())
-            >>> llm.generate([{"input": "What's the capital of Spain?"}])
-        """
-        super().__init__(
-            task=task,
-            num_threads=num_threads,
-            prompt_format=prompt_format,
-            prompt_formatting_fn=prompt_formatting_fn,
+        if self.base_url and (not self.model_id and not self.endpoint_name):
+            return self
+
+        raise ValidationError(
+            "Only one of `model_id`, `endpoint_name`, or `base_url` must be provided. Found"
+            f" `model_id`={self.model_id}, `endpoint_name`={self.endpoint_name}, and"
+            f" `base_url`={self.base_url}."
         )
 
-        if not _OPENAI_AVAILABLE:
-            raise ImportError(
-                "`OpenAILLM` cannot be used as `openai` is not installed, please "
-                " install it with `pip install openai`."
-            )
-
-        self.max_tokens = max_new_tokens
-        self.frequency_penalty = frequency_penalty
-        self.presence_penalty = presence_penalty
-        self.temperature = temperature
-        self.top_p = top_p
+    def load(self) -> None:  # noqa: C901
+        """Loads the either the `AsyncInferenceClient` or the `AsyncOpenAI` client to benefit
+        from async requests, running the Hugging Face Inference Endpoint underneath via the
+        `/v1/chat/completions` endpoint, exposed for the models running on TGI using the
+        `text-generation` task.
 
-        self.client = client or OpenAI(api_key=api_key, max_retries=6)
+        Raises:
+            ImportError: if the `openai` Python client is not installed.
+            ImportError: if the `huggingface-hub` Python client is not installed.
+            ValueError: if the model is not currently deployed or is not running the TGI framework.
+            ImportError: if the `transformers` Python client is not installed.
+        """
+        super().load()
 
         try:
-            assert (
-                model in self.available_models
-            ), f"Provided `model` is not available in your OpenAI account, available models are {self.available_models}"
-        except AttributeError:
-            logger.warning("Unable to check if model is available in your account.")
-        self.model = model
-
-    def __rich_repr__(self) -> Generator[Any, None, None]:
-        yield from super().__rich_repr__()
-        yield (
-            "parameters",
-            {
-                "max_tokens": self.max_tokens,
-                "frequency_penalty": self.frequency_penalty,
-                "presence_penalty": self.presence_penalty,
-                "temperature": self.temperature,
-                "top_p": self.top_p,
-            },
-        )
+            from huggingface_hub import (
+                AsyncInferenceClient,
+                InferenceClient,
+                get_inference_endpoint,
+            )
+        except ImportError as ie:
+            raise ImportError(
+                "Hugging Face Hub Python client is not installed. Please install it using"
+                " `pip install huggingface-hub`."
+            ) from ie
+
+        if self.api_key is None:
+            raise ValueError(
+                f"To use `{self.__class__.__name__}` an API key must be provided via `api_key`"
+                f" attribute or runtime parameter, or set the environment variable `{self._api_key_env_var}`."
+            )
 
-    @cached_property
-    def available_models(self) -> List[str]:
-        """Returns the list of available models in your OpenAI account."""
-        return [model.id for model in self.client.models.list().data]
+        if self.model_id is not None:
+            client = InferenceClient()
+            status = client.get_model_status(self.model_id)
+
+            if (
+                status.state not in {"Loadable", "Loaded"}
+                and status.framework != "text-generation-inference"
+            ):
+                raise ValueError(
+                    f"Model {self.model_id} is not currently deployed or is not running the TGI framework"
+                )
 
-    @property
-    def model_name(self) -> str:
-        """Returns the name of the OpenAI model."""
-        return self.model
+            self.base_url = client._resolve_url(
+                model=self.model_id, task="text-generation"
+            )
 
-    def _generate(
-        self,
-        inputs: List[Dict[str, Any]],
-        num_generations: int = 1,
-    ) -> List[List[LLMOutput]]:
-        """Generates `num_generations` for each input in `inputs`.
+        if self.endpoint_name is not None:
+            client = get_inference_endpoint(
+                name=self.endpoint_name,
+                namespace=self.endpoint_namespace,
+                token=self.api_key.get_secret_value(),
+            )
+            if client.status in ["paused", "scaledToZero"]:
+                client.resume().wait(timeout=300)
+            elif client.status in ["initializing"]:
+                client.wait(timeout=300)
+
+            self.base_url = client.url
+            self._model_name = client.repository
+
+        if self.use_openai_client:
+            try:
+                from openai import AsyncOpenAI
+            except ImportError as ie:
+                raise ImportError(
+                    "OpenAI Python client is not installed. Please install it using"
+                    " `pip install openai`."
+                ) from ie
+
+            self._aclient = AsyncOpenAI(
+                base_url=self.base_url,
+                api_key=self.api_key.get_secret_value(),
+                max_retries=6,
+            )
+        else:
+            self._aclient = AsyncInferenceClient(
+                model=self.base_url,
+                token=self.api_key.get_secret_value(),
+            )
 
-        Args:
-            inputs (List[Dict[str, Any]]): the inputs to be used for generation.
-            num_generations (int, optional): the number of generations to be performed for each
-                input. Defaults to 1.
+        if self.tokenizer_id:
+            try:
+                from transformers import AutoTokenizer
+            except ImportError as ie:
+                raise ImportError(
+                    "Transformers Python client is not installed. Please install it using"
+                    " `pip install transformers`."
+                ) from ie
 
-        Returns:
-            List[List[LLMOutput]]: the generated outputs.
-        """
-        prompts = self._generate_prompts(inputs, default_format="openai")
-        outputs = []
-        for prompt in prompts:
-            chat_completions = self.client.chat.completions.create(
-                messages=prompt,
-                model=self.model,
-                n=num_generations,
-                max_tokens=self.max_tokens,
-                frequency_penalty=self.frequency_penalty,
-                presence_penalty=self.presence_penalty,
-                temperature=self.temperature,
-                top_p=self.top_p,
-                timeout=50,
-            )
-
-            output = []
-            for chat_completion in chat_completions.choices:
-                try:
-                    parsed_response = self.task.parse_output(
-                        chat_completion.message.content.strip()
-                    )
-                except Exception as e:
-                    logger.error(f"Error parsing OpenAI response: {e}")
-                    parsed_response = None
-                output.append(
-                    LLMOutput(
-                        model_name=self.model_name,
-                        prompt_used=prompt,
-                        raw_output=chat_completion.message.content,
-                        parsed_output=parsed_response,
-                    )
-                )
-            outputs.append(output)
-        return outputs
+            self._tokenizer = AutoTokenizer.from_pretrained(self.tokenizer_id)
 
+    @property
+    @override
+    def model_name(self) -> Union[str, None]:  # type: ignore
+        """Returns the model name used for the LLM."""
+        return (
+            self.model_display_name
+            or self._model_name
+            or self.model_id
+            or self.endpoint_name
+            or self.base_url
+        )
 
-class JSONOpenAILLM(OpenAILLM):
-    def __init__(
+    async def _openai_agenerate(
         self,
-        task: "Task",
-        model: str = "gpt-3.5-turbo-1106",
-        client: Union["OpenAI", None] = None,
-        api_key: Union[str, None] = None,
+        input: "ChatType",
         max_new_tokens: int = 128,
         frequency_penalty: float = 0.0,
         presence_penalty: float = 0.0,
         temperature: float = 1.0,
-        top_p: float = 1.0,
-        num_threads: Union[int, None] = None,
-        prompt_format: Union["SupportedFormats", None] = None,
-        prompt_formatting_fn: Union[Callable[..., str], None] = None,
-    ) -> None:
-        """Initializes the JSONOpenAILLM class for generating JSON.
-
-        Args:
-            task (Task): the task to be performed by the LLM.
-            model (str, optional): the model to be used for generation. Defaults to "gpt-3.5-turbo".
-            client (Union[OpenAI, None], optional): an OpenAI client to be used for generation.
-                If `None`, a new client will be created. Defaults to `None`.
-            api_key (Union[str, None], optional): the OpenAI API key to be used for generation.
-                If `None`, the `OPENAI_API_KEY` environment variable will be used. Defaults to `None`.
-            max_new_tokens (int, optional): the maximum number of tokens to be generated.
-                Defaults to 128.
-            frequency_penalty (float, optional): the frequency penalty to be used for generation.
-                Defaults to 0.0.
-            presence_penalty (float, optional): the presence penalty to be used for generation.
-                Defaults to 0.0.
-            temperature (float, optional): the temperature to be used for generation.
-                Defaults to 1.0.
-            top_p (float, optional): the top-p value to be used for generation.
-                Defaults to 1.0.
-            num_threads (Union[int, None], optional): the number of threads to be used
-                for parallel generation. If `None`, no parallel generation will be performed.
-                Defaults to `None`.
-            prompt_format (Union[SupportedFormats, None], optional): the format to be used
-                for the prompt. If `None`, the default format of the task will be used, available
-                formats are `openai`, `chatml`, `llama2`, `zephyr`, and `default`. Defaults to `None`,
-                but `default` (concatenation of `system_prompt` and `formatted_prompt` with a line-break)
-                will be used if no `prompt_formatting_fn` is provided.
-            prompt_formatting_fn (Union[Callable[..., str], None], optional): a function to be
-                applied to the prompt before generation. If `None`, no formatting will be applied.
-                Defaults to `None`.
-
-        Raises:
-            AssertionError: if the provided `model` is not available in your OpenAI account.
-            AssertionError: if the provided `model` does not support JSON input.
-
-        Examples:
-            >>> from distilabel.tasks import TextGenerationTask
-            >>> from distilabel.llm import JSONOpenAILLM
-            >>> llm = JSONOpenAILLM(task=TextGenerationTask())
-            >>> llm.generate([{"input": "json for 'What's the capital of Spain?'"}])
-        """
-        super().__init__(
-            task,
-            model=model,
-            client=client,
-            api_key=api_key,
-            max_new_tokens=max_new_tokens,
+        top_p: Optional[float] = None,
+    ) -> GenerateOutput:
+        """Generates completions for the given input using the OpenAI async client."""
+        completion = await self._aclient.chat.completions.create(  # type: ignore
+            messages=input,  # type: ignore
+            model="tgi",
+            max_tokens=max_new_tokens,
+            n=1,
             frequency_penalty=frequency_penalty,
             presence_penalty=presence_penalty,
             temperature=temperature,
             top_p=top_p,
-            num_threads=num_threads,
-            prompt_format=prompt_format,
-            prompt_formatting_fn=prompt_formatting_fn,
-        )
-
-    @cached_property
-    def available_models(self) -> List[str]:
-        """Returns the list of available models in your OpenAI account."""
-        all_available_models = [model.id for model in self.client.models.list().data]
-        json_supporting_models = [
-            "gpt-4-0125-preview",
-            "gpt-4-turbo-preview",
-            "gpt-4-1106-preview",
-            "gpt-3.5-turbo-1106",
-        ]
-        available_json_supporting_models = list(
-            set(all_available_models) & set(json_supporting_models)
+            timeout=50,
         )
-        return available_json_supporting_models
+        if completion.choices[0].message.content is None:
+            self._logger.warning(
+                f"⚠️ Received no response using OpenAI client (model: '{self.model_name}')."
+                f" Finish reason was: {completion.choices[0].finish_reason}"
+            )
+        return [completion.choices[0].message.content]
 
-    def _generate(
+    # TODO: add `num_generations` parameter once either TGI or `AsyncInferenceClient` allows `n` parameter
+    @validate_call
+    async def agenerate(  # type: ignore
         self,
-        inputs: List[Dict[str, Any]],
-        num_generations: int = 1,
-    ) -> List[List[LLMOutput]]:
-        """Generates `num_generations` for each input in `inputs` in JSON format.
+        input: ChatType,
+        max_new_tokens: int = 128,
+        frequency_penalty: float = 0.0,
+        presence_penalty: float = 0.0,
+        repetition_penalty: Optional[float] = None,
+        temperature: float = 1.0,
+        do_sample: bool = False,
+        top_k: Optional[int] = None,
+        top_p: Optional[float] = None,
+        typical_p: Optional[float] = None,
+    ) -> "GenerateOutput":
+        """Generates completions for the given input using the OpenAI async client.
 
         Args:
-            inputs (List[Dict[str, Any]]): the inputs to be used for generation.
-            num_generations (int, optional): the number of generations to be performed for each
-                input. Defaults to 1.
+            input: a single input in chat format to generate responses for.
+            max_new_tokens: the maximum number of new tokens that the model will generate.
+                Defaults to `128`.
+            frequency_penalty: the repetition penalty to use for the generation. Defaults
+                to `0.0`. Only applies if `use_openai_client=True`.
+            presence_penalty: the presence penalty to use for the generation. Defaults to
+                `0.0`. Only applies if `use_openai_client=True`.
+            repetition_penalty: the repetition penalty to use for the generation. Defaults
+                to `None`. Only applies if `use_openai_client=False`.
+            temperature: the temperature to use for the generation. Defaults to `1.0`.
+            do_sample: whether to use sampling for the generation. Defaults to `False`.
+                Only applies if `use_openai_client=False`.
+            top_k: the top-k value to use for the generation. Defaults to `0.8`, since neither
+                `0.0` nor `1.0` are valid values in TGI.
+            top_p: the top-p value to use for the generation. Defaults to `1.0`.
+            typical_p: the typical-p value to use for the generation. Defaults to `0.5`.
 
         Returns:
-            List[List[LLMOutput]]: the generated outputs.
+            A list of lists of strings containing the generated responses for each input.
         """
-        prompts = self._generate_prompts(inputs, default_format="openai")
-        outputs = []
-        for prompt in prompts:
-            chat_completions = self.client.chat.completions.create(
-                messages=prompt,
-                model=self.model,
-                n=num_generations,
-                max_tokens=self.max_tokens,
-                frequency_penalty=self.frequency_penalty,
-                presence_penalty=self.presence_penalty,
-                temperature=self.temperature,
-                top_p=self.top_p,
-                timeout=50,
-                response_format={"type": "json_object"},
-            )
-
-            output = []
-            for chat_completion in chat_completions.choices:
-                try:
-                    parsed_response = self.task.parse_output(
-                        chat_completion.message.content.strip()
-                    )
-                except Exception as e:
-                    logger.error(f"Error parsing OpenAI response: {e}")
-                    parsed_response = None
-                try:
-                    json.loads(chat_completion.message.content)
-                except json.JSONDecodeError:
-                    warnings.warn(
-                        "The response is not a valid JSON.",
-                        UserWarning,
-                        stacklevel=2,
-                    )
-                    parsed_response = None
-                output.append(
-                    LLMOutput(
-                        model_name=self.model_name,
-                        prompt_used=prompt,
-                        raw_output=chat_completion.message.content,
-                        parsed_output=parsed_response,
-                    )
-                )
-            outputs.append(output)
-        return outputs
+
+        if self.use_openai_client:
+            return await self._openai_agenerate(
+                input=input,
+                max_new_tokens=max_new_tokens,
+                frequency_penalty=frequency_penalty,
+                presence_penalty=presence_penalty,
+                temperature=temperature,
+                top_p=top_p,
+            )
+
+        if self._tokenizer is not None:
+            prompt = self._tokenizer.apply_chat_template(  # type: ignore
+                conversation=input,  # type: ignore
+                tokenize=False,
+                add_generation_prompt=True,
+            )
+        else:
+            prompt = "\n".join([message["content"] for message in input])
+
+        try:
+            completion = await self._aclient.text_generation(  # type: ignore
+                prompt=prompt,  # type: ignore
+                max_new_tokens=max_new_tokens,
+                do_sample=do_sample,
+                typical_p=typical_p,
+                repetition_penalty=repetition_penalty,
+                temperature=temperature,
+                top_p=top_p,
+                top_k=top_k,
+            )
+            return [completion]
+        except Exception as e:
+            self._logger.warning(
+                f"⚠️ Received no response using Inference Client (model: '{self.model_name}')."
+                f" Finish reason was: {e}"
+            )
+            return [None]
+
+    # TODO: remove this function once `AsyncInferenceClient` allows `n` parameter
+    @override
+    def generate(
+        self,
+        inputs: List["ChatType"],
+        num_generations: int = 1,
+        **kwargs: Any,
+    ) -> List["GenerateOutput"]:
+        """Method to generate a list of responses asynchronously, returning the output
+        synchronously awaiting for the response of each input sent to `agenerate`.
+        """
+
+        async def agenerate(
+            inputs: List["ChatType"], **kwargs: Any
+        ) -> "GenerateOutput":
+            """Internal function to parallelize the asynchronous generation of responses."""
+            tasks = [
+                asyncio.create_task(self.agenerate(input=input, **kwargs))
+                for input in inputs
+                for _ in range(num_generations)
+            ]
+            return [outputs[0] for outputs in await asyncio.gather(*tasks)]
+
+        outputs = self.event_loop.run_until_complete(agenerate(inputs, **kwargs))
+        return list(grouper(outputs, n=num_generations, incomplete="ignore"))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `distilabel-0.6.0/src/distilabel/llm/together.py` & `distilabel-1.0.0/src/distilabel/llms/huggingface/transformers.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,224 +9,201 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
-from functools import cached_property
-from typing import TYPE_CHECKING, Any, Callable, Dict, Generator, List, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
-from distilabel.llm.base import LLM
-from distilabel.llm.utils import LLMOutput
-from distilabel.logger import get_logger
-from distilabel.utils.imports import _TOGETHER_AVAILABLE
+from pydantic import PrivateAttr, validate_call
 
-if _TOGETHER_AVAILABLE:
-    import together
+from distilabel.llms.base import LLM
+from distilabel.llms.chat_templates import CHATML_TEMPLATE
+from distilabel.llms.mixins import CudaDevicePlacementMixin
+from distilabel.llms.typing import GenerateOutput
+from distilabel.steps.tasks.typing import ChatType
 
 if TYPE_CHECKING:
-    from distilabel.tasks.base import Task
-    from distilabel.tasks.prompt import SupportedFormats
+    from transformers import Pipeline
+    from transformers.modeling_utils import PreTrainedModel
+    from transformers.tokenization_utils import PreTrainedTokenizer
+
+    from distilabel.llms.typing import HiddenState
+
+
+class TransformersLLM(LLM, CudaDevicePlacementMixin):
+    """Hugging Face `transformers` library LLM implementation using the text generation
+    pipeline.
+
+    Attributes:
+        model: the model Hugging Face Hub repo id or a path to a directory containing the
+            model weights and configuration files.
+        revision: if `model` refers to a Hugging Face Hub repository, then the revision
+            (e.g. a branch name or a commit id) to use. Defaults to `"main"`.
+        torch_dtype: the torch dtype to use for the model e.g. "float16", "float32", etc.
+            Defaults to `"auto"`.
+        trust_remote_code: whether to trust or not remote (code in the Hugging Face Hub
+            repository) code to load the model. Defaults to `False`.
+        model_kwargs: additional dictionary of keyword arguments that will be passed to
+            the `from_pretrained` method of the model.
+        tokenizer: the tokenizer Hugging Face Hub repo id or a path to a directory containing
+            the tokenizer config files. If not provided, the one associated to the `model`
+            will be used. Defaults to `None`.
+        use_fast: whether to use a fast tokenizer or not. Defaults to `True`.
+        chat_template: a chat template that will be used to build the prompts before
+            sending them to the model. If not provided, the chat template defined in the
+            tokenizer config will be used. If not provided and the tokenizer doesn't have
+            a chat template, then ChatML template will be used. Defaults to `None`.
+        device: the name or index of the device where the model will be loaded. Defaults
+            to `None`.
+        device_map: a dictionary mapping each layer of the model to a device, or a mode
+            like `"sequential"` or `"auto"`. Defaults to `None`.
+        token: the Hugging Face Hub token that will be used to authenticate to the Hugging
+            Face Hub. If not provided, the `HF_TOKEN` environment or `huggingface_hub` package
+            local configuration will be used. Defaults to `None`.
+    """
+
+    model: str
+    revision: str = "main"
+    torch_dtype: str = "auto"
+    trust_remote_code: bool = False
+    model_kwargs: Optional[Dict[str, Any]] = None
+    tokenizer: Optional[str] = None
+    use_fast: bool = True
+    chat_template: Optional[str] = None
+    device: Optional[Union[str, int]] = None
+    device_map: Optional[Union[str, Dict[str, Any]]] = None
+    token: Optional[str] = None
+
+    _pipeline: Optional["Pipeline"] = PrivateAttr(...)
+
+    def load(self) -> None:
+        """Loads the model and tokenizer and creates the text generation pipeline. In addition,
+        it will configure the tokenizer chat template."""
+        super().load()
 
+        if self.device == "cuda":
+            CudaDevicePlacementMixin.load(self)
 
-logger = get_logger()
-
-
-class TogetherInferenceLLM(LLM):
-    def __init__(
-        self,
-        model: str,
-        task: "Task",
-        api_key: Union[str, None] = None,
-        max_new_tokens: int = 128,
-        repetition_penalty: float = 1.0,
-        temperature: float = 1.0,
-        top_p: float = 1.0,
-        top_k: int = 1,
-        stop: Union[List[str], None] = None,
-        logprobs: int = 0,
-        num_threads: Union[int, None] = None,
-        prompt_format: Union["SupportedFormats", None] = None,
-        prompt_formatting_fn: Union[Callable[..., str], None] = None,
-    ) -> None:
-        """Initializes the TogetherInferenceLLM class.
-
-        Args:
-            model (str): the model to be used for generation.
-            task (Task): the task to be performed by the LLM.
-            max_new_tokens (int, optional): the maximum number of tokens to be generated.
-                Defaults to 128.
-            temperature (float, optional): the temperature to be used for generation. From the Together
-                Inference docs: "A decimal number that determines the degree of randomness in the response.
-                A value of 0 will always yield the same output. A temperature much less than 1 favors more
-                correctness and is appropriate for question answering or summarization. A value approaching
-                1 introduces more randomness in the output.". Defaults to 1.0.
-            repetition_penalty (float, optional): the repetition penalty to be used for generation. From the
-                Together Inference docs: "Controls the diversity of generated text by reducing the likelihood
-                of repeated sequences. Higher values decrease repetition.". Defaults to 1.0.
-            top_p (float, optional): the top-p value to be used for generation. From the Together
-                Inference docs: "used to dynamically adjust the number of choices for each predicted
-                token based on the cumulative probabilities. It specifies a probability threshold,
-                below which all less likely tokens are filtered out. This technique helps to maintain
-                diversity and generate more fluent and natural-sounding text.". Defaults to 1.0.
-            top_k (int, optional): the top-k value to be used for generation. From the Together Inference
-                docs: "used to limit the number of choices for the next predicted word or token. It specifies
-                the maximum number of tokens to consider at each step, based on their probability of occurrence.
-                This technique helps to speed up the generation process and can improve the quality of the
-                generated text by focusing on the most likely options.". Defaults to 1.
-            stop (List[str], optional): strings to delimitate the generation process, so that when the
-                model generates any of the provided characters, the generation process is considered completed.
-                Defaults to None.
-            logprobs (int, optional): the number of logprobs to be returned for each token. From the
-                Together Inference docs: "An integer that specifies how many top token log probabilities
-                are included in the response for each token generation step.". Defaults to None.
-            num_threads (Union[int, None], optional): the number of threads to be used
-                for parallel generation. If `None`, no parallel generation will be performed.
-                Defaults to `None`.
-            prompt_format (Union[SupportedFormats, None], optional): the format to be used
-                for the prompt. If `None`, the default format of the task will be used, available
-                formats are `openai`, `chatml`, `llama2`, `zephyr`, and `default`. Defaults to `None`,
-                but `default` (concatenation of `system_prompt` and `formatted_prompt` with a line-break)
-                will be used if no `prompt_formatting_fn` is provided.
-            prompt_formatting_fn (Union[Callable[..., str], None], optional): a function to be
-                applied to the prompt before generation. If `None`, no formatting will be applied.
-                Defaults to `None`.
-
-        Raises:
-            AssertionError: if the provided `model` is not available in Together Inference.
-
-        Examples:
-            >>> from distilabel.tasks import TextGenerationTask
-            >>> from distilabel.llm import TogetherInferenceLLM
-            >>> llm = TogetherInferenceLLM(model="togethercomputer/llama-2-7b", task=TextGenerationTask(), prompt_format="llama2")
-            >>> llm.generate([{"input": "What's the capital of Spain?"}])
-        """
-        if not _TOGETHER_AVAILABLE:
+        try:
+            from transformers import pipeline
+        except ImportError as ie:
             raise ImportError(
-                "`TogetherInferenceLLM` cannot be used as `together` is not installed, please "
-                " install it with `pip install together`."
-            )
+                "Transformers is not installed. Please install it using `pip install transformers`."
+            ) from ie
 
-        together.api_key = api_key or os.getenv("TOGETHER_API_KEY", None)
-        if together.api_key is None:
-            raise ValueError(
-                "No `api_key` provided, please provide one or set the `TOGETHER_API_KEY` "
-                "environment variable."
-            )
-
-        super().__init__(
-            task=task,
-            num_threads=num_threads,
-            prompt_format=prompt_format,
-            prompt_formatting_fn=prompt_formatting_fn,
+        self._pipeline = pipeline(
+            "text-generation",
+            model=self.model,
+            revision=self.revision,
+            torch_dtype=self.torch_dtype,
+            trust_remote_code=self.trust_remote_code,
+            model_kwargs=self.model_kwargs or {},
+            tokenizer=self.tokenizer or self.model,
+            use_fast=self.use_fast,
+            device=self.device,
+            device_map=self.device_map,
+            token=self.token or os.getenv("HF_TOKEN"),
+            return_full_text=False,
         )
 
-        assert (
-            model in self.available_models
-        ), f"Provided `model` is not available in Together Inference, available models are {self.available_models}"
-        self.model = model
-
-        self.max_new_tokens = max_new_tokens
-        self.temperature = temperature
-        self.top_p = top_p
-        self.top_k = top_k
-        self.repetition_penalty = repetition_penalty
-        self.stop = stop
-        self.logprobs = logprobs
-
-    def __rich_repr__(self) -> Generator[Any, None, None]:
-        yield from super().__rich_repr__()
-        yield (
-            "parameters",
-            {
-                "max_new_tokens": self.max_new_tokens,
-                "temperature": self.temperature,
-                "repetition_penalty": self.repetition_penalty,
-                "top_p": self.top_p,
-                "top_k": self.top_k,
-                "stop": self.stop,
-                "logprobs": self.logprobs,
-            },
-        )
-
-    @cached_property
-    def available_models(self) -> List[str]:
-        """Returns the list of available models in Together Inference."""
-        return [
-            model["name"]
-            for model in together.Models.list()
-            if model["display_type"] != "image"
-        ]
+        if self.chat_template is not None:
+            self._pipeline.tokenizer.chat_template = self.chat_template  # type: ignore
+        elif (
+            self._pipeline.tokenizer.chat_template is None  # type: ignore
+            and self._pipeline.tokenizer.default_chat_template is None  # type: ignore
+        ):
+            self._pipeline.tokenizer.chat_template = CHATML_TEMPLATE  # type: ignore
 
     @property
     def model_name(self) -> str:
-        """Returns the name of the Together Inference model."""
+        """Returns the model name used for the LLM."""
         return self.model
 
-    def _generate_single_output(self, prompt: str) -> LLMOutput:
-        """Runs the Together Inference text generation function over a single prompt
-        producing a single `LLMOutput`.
+    def prepare_input(self, input: "ChatType") -> str:
+        """Prepares the input by applying the chat template to the input, which is formatted
+        as an OpenAI conversation, and adding the generation prompt.
+        """
+        return self._pipeline.tokenizer.apply_chat_template(  # type: ignore
+            input,  # type: ignore
+            tokenize=False,
+            add_generation_prompt=True,
+        )
+
+    @validate_call
+    def generate(  # type: ignore
+        self,
+        inputs: List[ChatType],
+        num_generations: int = 1,
+        max_new_tokens: int = 128,
+        temperature: float = 0.1,
+        repetition_penalty: float = 1.1,
+        top_p: float = 1.0,
+        top_k: int = 0,
+        do_sample: bool = True,
+    ) -> List[GenerateOutput]:
+        """Generates `num_generations` responses for each input using the text generation
+        pipeline.
 
         Args:
-            prompt (str): the formatted prompt to be provided to the Together Inference
-                endpoint.
+            inputs: a list of inputs in chat format to generate responses for.
+            num_generations: the number of generations to create per input. Defaults to
+                `1`.
+            max_new_tokens: the maximum number of new tokens that the model will generate.
+                Defaults to `128`.
+            temperature: the temperature to use for the generation. Defaults to `0.1`.
+            repetition_penalty: the repetition penalty to use for the generation. Defaults
+                to `1.1`.
+            top_p: the top-p value to use for the generation. Defaults to `1.0`.
+            top_k: the top-k value to use for the generation. Defaults to `0`.
+            do_sample: whether to use sampling or not. Defaults to `True`.
 
-        Raises:
-            RuntimeError: raised if the Together Inference endpoint fails.
+        Returns:
+            A list of lists of strings containing the generated responses for each input.
         """
-        try:
-            output = together.Complete.create(
-                prompt=prompt,
-                model=self.model,
-                max_tokens=self.max_new_tokens,
-                stop=self.stop,
-                temperature=self.temperature,
-                top_k=self.top_k,
-                top_p=self.top_p,
-                repetition_penalty=self.repetition_penalty,
-                logprobs=self.logprobs,
-            )
-        except Exception as e:
-            raise RuntimeError(
-                f"Together Inference generation failed with exception: {e}"
-            ) from e
-
-        if output["output"]["choices"] is None or len(output["output"]["choices"]) < 1:  # type: ignore
-            raise RuntimeError("Together Inference generation returned no generations.")
-
-        choice = output["output"]["choices"][0]  # type: ignore
-        try:
-            parsed_response = self.task.parse_output(choice["text"].strip())
-        except Exception as e:
-            logger.error(f"Error parsing Together Inference response: {e}")
-            parsed_response = None
-
-        return LLMOutput(
-            model_name=self.model_name,
-            prompt_used=prompt,
-            raw_output=choice["text"] or None,
-            parsed_output=parsed_response,
+        outputs: List[List[Dict[str, str]]] = self._pipeline(  # type: ignore
+            [self.prepare_input(input=input) for input in inputs],
+            max_new_tokens=max_new_tokens,
+            temperature=temperature,
+            repetition_penalty=repetition_penalty,
+            top_p=top_p,
+            top_k=top_k,
+            do_sample=do_sample,
+            num_return_sequences=num_generations,
         )
+        return [
+            [generation["generated_text"] for generation in output]
+            for output in outputs
+        ]
 
-    def _generate(
-        self,
-        inputs: List[Dict[str, Any]],
-        num_generations: int = 1,
-    ) -> List[List[LLMOutput]]:
-        """Generates `num_generations` for each input in `inputs`.
+    def get_last_hidden_states(self, inputs: List["ChatType"]) -> List["HiddenState"]:
+        """Gets the last `hidden_states` of the model for the given inputs. It doesn't
+        execute the task head.
 
         Args:
-            inputs (List[Dict[str, Any]]): the inputs to be used for generation.
-            num_generations (int, optional): the number of generations to be performed for each
-                input. Defaults to 1.
+            inputs: a list of inputs in chat format to generate the embeddings for.
 
         Returns:
-            List[List[LLMOutput]]: the generated outputs.
+            A list containing the last hidden state for each sequence using a NumPy array
+            with shape [num_tokens, hidden_size].
         """
-        prompts = self._generate_prompts(inputs, default_format=None)
-        outputs = []
-        for prompt in prompts:
-            outputs.append(
-                [self._generate_single_output(prompt) for _ in range(num_generations)]
+        model: "PreTrainedModel" = (
+            self._pipeline.model.model  # type: ignore
+            if hasattr(self._pipeline.model, "model")  # type: ignore
+            else next(self._pipeline.model.children())  # type: ignore
+        )
+        tokenizer: "PreTrainedTokenizer" = self._pipeline.tokenizer  # type: ignore
+        input_ids = tokenizer(
+            [self.prepare_input(input) for input in inputs],  # type: ignore
+            return_tensors="pt",
+            padding=True,
+        ).to(model.device)
+        last_hidden_states = model(**input_ids)["last_hidden_state"]
+
+        return [
+            seq_last_hidden_state[attention_mask.bool(), :].detach().cpu().numpy()
+            for seq_last_hidden_state, attention_mask in zip(
+                last_hidden_states,
+                input_ids["attention_mask"],  # type: ignore
             )
-        return outputs
+        ]
```

### Comparing `distilabel-0.6.0/src/distilabel/llm/utils.py` & `distilabel-1.0.0/src/distilabel/steps/tasks/typing.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Any, Optional, TypedDict
+from typing import List
 
+from typing_extensions import TypedDict
 
-class LLMOutput(TypedDict):
-    """A type for the output of an LLM."""
 
-    model_name: str
-    prompt_used: Any
-    raw_output: Any
-    parsed_output: Optional[Any]
+class ChatItem(TypedDict):
+    role: str
+    content: str
+
+
+ChatType = List[ChatItem]
+"""ChatType is a type alias for a `list` of `dict`s following the OpenAI conversational format."""
```

### Comparing `distilabel-0.6.0/src/distilabel/llm/google/__init__.py` & `distilabel-1.0.0/src/distilabel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/src/distilabel/llm/huggingface/__init__.py` & `distilabel-1.0.0/src/distilabel/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/src/distilabel/tasks/mixins.py` & `distilabel-1.0.0/src/distilabel/steps/argilla/preference.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,223 +8,240 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import warnings
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Protocol
+import hashlib
+from typing import TYPE_CHECKING, Any, Dict, List, Union
 
-from distilabel.utils.argilla import (
-    infer_fields_from_dataset_row,
-    model_metadata_from_dataset_row,
-)
-from distilabel.utils.imports import _ARGILLA_AVAILABLE
+from pydantic import PrivateAttr
+from typing_extensions import override
 
-if _ARGILLA_AVAILABLE:
+try:
     import argilla as rg
+except ImportError:
+    pass
+
+from distilabel.steps.argilla.base import Argilla
+from distilabel.steps.base import StepInput
 
 if TYPE_CHECKING:
-    from argilla import FeedbackDataset, FeedbackRecord
+    from argilla import (
+        RatingQuestion,
+        SuggestionSchema,
+        TextField,
+        TextQuestion,
+    )
+
+    from distilabel.steps.typing import StepOutput
+
+
+class PreferenceToArgilla(Argilla):
+    """Step that creates a dataset in Argilla during the load phase, and then pushes the input
+    batches into it as records. This dataset is a preference dataset, where there's one field
+    for the instruction and one extra field per each generation within the same record, and then
+    a rating question per each of the generation fields. The rating question asks the annotator to
+    set a rating from 1 to 5 for each of the provided generations.
+
+    Note:
+        This step is meant to be used in conjunction with the `UltraFeedback` step, or any other step
+        generating both ratings and responses for a given set of instruction and generations for the
+        given instruction. But alternatively, it can also be used with any other task or step generating
+        only the `instruction` and `generations`, as the `ratings` and `rationales` are optional.
+
+    Attributes:
+        num_generations: The number of generations to include in the dataset.
+        dataset_name: The name of the dataset in Argilla.
+        dataset_workspace: The workspace where the dataset will be created in Argilla. Defaults to
+            `None`, which means it will be created in the default workspace.
+        api_url: The URL of the Argilla API. Defaults to `None`, which means it will be read from
+            the `ARGILLA_API_URL` environment variable.
+        api_key: The API key to authenticate with Argilla. Defaults to `None`, which means it will
+            be read from the `ARGILLA_API_KEY` environment variable.
+
+    Runtime parameters:
+        - `api_url`: The base URL to use for the Argilla API requests.
+        - `api_key`: The API key to authenticate the requests to the Argilla API.
+
+    Input columns:
+        - instruction (`str`): The instruction that was used to generate the completion.
+        - generations (`List[str]`): The completion that was generated based on the input instruction.
+        - ratings (`List[str]`, optional): The ratings for the generations. If not provided, the
+            generated ratings won't be pushed to Argilla.
+        - rationales (`List[str]`, optional): The rationales for the ratings. If not provided, the
+            generated rationales won't be pushed to Argilla.
+    """
 
+    num_generations: int
 
-class TaskProtocol(Protocol):
-    @property
-    def input_args_names(self) -> List[str]:
-        ...
+    _id: str = PrivateAttr(default="id")
+    _instruction: str = PrivateAttr(...)
+    _generations: str = PrivateAttr(...)
+    _ratings: str = PrivateAttr(...)
+    _rationales: str = PrivateAttr(...)
+
+    def load(self) -> None:
+        """Sets the `_instruction` and `_generations` attributes based on the `inputs_mapping`, otherwise
+        uses the default values; and then uses those values to create a `FeedbackDataset` suited for
+        the text-generation scenario. And then it pushes it to Argilla.
+        """
+        super().load()
 
+        # Both `instruction` and `generations` will be used as the fields of the dataset
+        self._instruction = self.input_mappings.get("instruction", "instruction")
+        self._generations = self.input_mappings.get("generations", "generations")
+        # Both `ratings` and `rationales` will be used as suggestions to the default questions of the dataset
+        self._ratings = self.input_mappings.get("ratings", "ratings")
+        self._rationales = self.input_mappings.get("rationales", "rationales")
+
+        if self._rg_dataset_exists():
+            _rg_dataset = rg.FeedbackDataset.from_argilla(  # type: ignore
+                name=self.dataset_name,
+                workspace=self.dataset_workspace,
+            )
+
+            for field in _rg_dataset.fields:
+                if (
+                    field.name
+                    not in [self._id, self._instruction]
+                    + [
+                        f"{self._generations}-{idx}"
+                        for idx in range(self.num_generations)
+                    ]
+                    and field.required
+                ):
+                    raise ValueError(
+                        f"The dataset {self.dataset_name} in the workspace {self.dataset_workspace} already exists,"
+                        f" but contains at least a required field that is neither `{self._id}`, `{self._instruction}`,"
+                        f" nor `{self._generations}`."
+                    )
 
-class RatingToArgillaMixin:
-    """Mixin that adds the `to_argilla_dataset` and `to_argilla_record` methods for tasks
-    that generate both ratings and rationales i.e. `PreferenceTask` or `CritiqueTask`.
-    """
+            self._rg_dataset = _rg_dataset
+        else:
+            _rg_dataset = rg.FeedbackDataset(  # type: ignore
+                fields=[
+                    rg.TextField(name=self._id, title=self._id),  # type: ignore
+                    rg.TextField(name=self._instruction, title=self._instruction),  # type: ignore
+                    *self._generation_fields(),  # type: ignore
+                ],
+                questions=self._rating_rationale_pairs(),  # type: ignore
+            )
+            self._rg_dataset = _rg_dataset.push_to_argilla(
+                name=self.dataset_name, workspace=self.dataset_workspace
+            )
+
+    def _generation_fields(self) -> List["TextField"]:
+        """Method to generate the fields for each of the generations."""
+        return [
+            rg.TextField(  # type: ignore
+                name=f"{self._generations}-{idx}",
+                title=f"{self._generations}-{idx}",
+                required=True if idx == 0 else False,
+            )
+            for idx in range(self.num_generations)
+        ]
 
-    def _check_column_is_present(
+    def _rating_rationale_pairs(
         self,
-        column_name: str,
-        dataset_row: Dict[str, Any],
-        column_type: str = "generations",
-    ) -> None:
-        """Helper function to check if a column is present in the dataset row.
-
-        Args:
-            column_name (str): Name of the column to check.
-            dataset_row (Dict[str, Any]): Row from the dataset.
-            column_type (str, optional): Type of column expected in the dataset. Defaults to "generations".
-
-        Raises:
-            ValueError: If the column is not present in the dataset row when it should be.
-        """
-        # The function is added mainly to simplify the code in the `to_argilla_dataset` to pass the mccabe complexity check.
-        if column_name is None or column_name not in dataset_row:
-            raise ValueError(
-                f"The `{column_type}_column='{column_name}'` is not present in the"
-                f" dataset row. Please provide any of {list(dataset_row.keys())}.",
-            )
-
-    def to_argilla_dataset(
-        self: TaskProtocol,
-        dataset_row: Dict[str, Any],
-        generations_column: str = "generations",
-        ratings_column: str = "rating",
-        rationale_column: str = "rationale",
-        ratings_values: Optional[List[int]] = None,
-    ) -> "FeedbackDataset":
-        # First we infer the fields from the input_args_names, but we could also
-        # create those manually instead using `rg.TextField(...)`
-        fields = infer_fields_from_dataset_row(
-            field_names=self.input_args_names, dataset_row=dataset_row
-        )
-        # Then we add the questions, which cannot be easily inferred in this case,
-        # because those depend neither on the outputs nor on the inputs, but in a combination
-        # of both, since the questions will be formulated using the inputs, but assigned to the
-        # outputs.
-        self._check_column_is_present(
-            generations_column, dataset_row, column_type="generations"
-        )
-        self._check_column_is_present(
-            ratings_column, dataset_row, column_type="ratings"
-        )
-
+    ) -> List[Union["RatingQuestion", "TextQuestion"]]:
+        """Method to generate the rating and rationale questions for each of the generations."""
         questions = []
-        for idx in range(1, len(dataset_row[generations_column]) + 1):
-            questions.append(
-                rg.RatingQuestion(  # type: ignore
-                    name=f"{generations_column}-{idx}-{ratings_column}",
-                    title=f"What's the {ratings_column} for {generations_column}-{idx}?",
-                    values=ratings_values or [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
-                )
-            )
-        if rationale_column:
-            self._check_column_is_present(
-                rationale_column, dataset_row, column_type="rationale"
-            )
-            questions.append(
-                rg.TextQuestion(  # type: ignore
-                    name=f"{ratings_column}-{rationale_column}",
-                    title=f"What's the {rationale_column} behind each {ratings_column}?",
-                )
+        for idx in range(self.num_generations):
+            questions.extend(
+                [
+                    rg.RatingQuestion(  # type: ignore
+                        name=f"{self._generations}-{idx}-rating",
+                        title=f"Rate {self._generations}-{idx} given {self._instruction} based on the annotation guidelines.",
+                        description=f"Ignore this question if the corresponding `{self._generations}-{idx}` field is not available."
+                        if idx != 0
+                        else None,
+                        values=[1, 2, 3, 4, 5],
+                        required=True if idx == 0 else False,
+                    ),
+                    rg.TextQuestion(  # type: ignore
+                        name=f"{self._generations}-{idx}-rationale",
+                        title=f"Specify the rationale for {self._generations}-{idx}'s rating.",
+                        description=f"Ignore this question if the corresponding `{self._generations}-{idx}` field is not available."
+                        if idx != 0
+                        else None,
+                        required=False,
+                    ),
+                ]
             )
-        # Finally, we define some metadata properties that can be potentially used
-        # while exploring the dataset within Argilla to get more insights on the data.
-        metadata_properties = []
-        for arg_name in self.input_args_names:
-            if isinstance(dataset_row[arg_name], list):
-                for idx in range(1, len(dataset_row[arg_name]) + 1):
-                    metadata_properties.append(
-                        rg.IntegerMetadataProperty(name=f"length-{arg_name}-{idx}")  # type: ignore
-                    )
-            elif isinstance(dataset_row[arg_name], str):
-                metadata_properties.append(
-                    rg.IntegerMetadataProperty(name=f"length-{arg_name}")  # type: ignore
-                )
-            else:
-                warnings.warn(
-                    f"Unsupported input type ({type(dataset_row[arg_name])}), skipping...",
-                    UserWarning,
-                    stacklevel=2,
-                )
-        metadata_properties.append(
-            rg.FloatMetadataProperty(name=f"distance-best-{ratings_column}")  # type: ignore
-        )
-        # Then we just return the `FeedbackDataset` with the fields, questions, and metadata properties
-        # defined above.
-        return rg.FeedbackDataset(
-            fields=fields,
-            questions=questions,
-            metadata_properties=metadata_properties,  # Note that these are always optional
-        )
-
-    def _merge_rationales(
-        self, rationales: List[str], generations_column: str = "generations"
-    ) -> str:
-        return "\n".join(
-            f"{generations_column}-{idx}:\n{rationale}\n"
-            for idx, rationale in enumerate(rationales, start=1)
-        )
-
-    def to_argilla_record(  # noqa: C901
-        self: TaskProtocol,
-        dataset_row: Dict[str, Any],
-        generations_column: str = "generations",
-        ratings_column: str = "rating",
-        rationale_column: str = "rationale",
-        ratings_values: Optional[List[int]] = None,
-    ) -> "FeedbackRecord":
-        """Converts a dataset row to an Argilla `FeedbackRecord`."""
-        # We start off with the fields, which are the inputs of the LLM, but also
-        # build the metadata from them, as previously specified within the
-        fields, metadata = {}, {}
-        for arg_name in self.input_args_names:
-            arg_value = dataset_row[arg_name]
-            if isinstance(arg_value, list):
-                for idx, value in enumerate(arg_value, start=1):
-                    fields[f"{arg_name}-{idx}"] = value.strip() if value else ""
-                    if value is not None:
-                        metadata[f"length-{arg_name}-{idx}"] = len(value.strip())
-            elif isinstance(arg_value, str):
-                fields[arg_name] = arg_value.strip() if arg_value else ""
-                if arg_value is not None:
-                    metadata[f"length-{arg_name}"] = len(arg_value.strip())
-            else:
-                warnings.warn(
-                    f"Unsupported input type ({type(arg_value)}), skipping...",
-                    UserWarning,
-                    stacklevel=2,
-                )
-        # Then we include the suggestions, which are generated from the outputs
-        # of the LLM instead.
-        suggestions = []
-        if dataset_row.get(rationale_column) is not None:
-            rationales = dataset_row.get(rationale_column)
-            suggestions.append(
-                {
-                    "question_name": f"{ratings_column}-{rationale_column}",
-                    "value": self._merge_rationales(rationales=rationales)  # type: ignore
-                    if isinstance(rationales, list)
-                    else rationales,
-                }
-            )
-        if ratings_column and ratings_column not in dataset_row:
-            raise ValueError(
-                f"The ratings column {ratings_column} is not present in the dataset row."
-            )
-        if dataset_row.get(ratings_column) is not None:
-            ratings = dataset_row.get(ratings_column)
-            if isinstance(ratings, list):
-                for idx, value in enumerate(ratings, start=1):  # type: ignore
-                    suggestions.append(
-                        {
-                            "question_name": f"{generations_column}-{idx}-{ratings_column}",
-                            "value": 1
-                            if value < 1
-                            else int(value)
-                            if value
-                            <= (
-                                max(ratings_values)
-                                if ratings_values is not None
-                                else 10
-                            )
-                            else None,
-                        }
-                    )
+        return questions
 
-                if len(ratings) >= 2:  # type: ignore
-                    sorted_ratings = sorted(ratings, reverse=True)  # type: ignore
-                    metadata[f"distance-best-{ratings_column}"] = (
-                        sorted_ratings[0] - sorted_ratings[1]
-                    )
-            elif isinstance(ratings, (str, float, int)):
-                suggestions.append(
+    @property
+    def inputs(self) -> List[str]:
+        """The inputs for the step are the `instruction` and the `generations`. Optionally, one could also
+        provide the `ratings` and the `rationales` for the generations."""
+        return ["instruction", "generations"]
+
+    def _add_suggestions_if_any(
+        self, input: Dict[str, Any]
+    ) -> List["SuggestionSchema"]:
+        """Method to generate the suggestions for the `FeedbackRecord` based on the input."""
+        # Since the `suggestions` i.e. answers to the `questions` are optional, will default to {}
+        suggestions = []
+        # If `ratings` is in `input`, then add those as suggestions
+        if self._ratings in input:
+            suggestions.extend(
+                [
                     {
-                        "question_name": f"{generations_column}-1-{ratings_column}",
-                        "value": int(ratings),
+                        "question_name": f"{self._generations}-{idx}-rating",
+                        "value": rating,
                     }
+                    for idx, rating in enumerate(input[self._ratings])
+                    if rating is not None
+                    and isinstance(rating, int)
+                    and rating in [1, 2, 3, 4, 5]
+                ],
+            )
+        # If `rationales` is in `input`, then add those as suggestions
+        if self._rationales in input:
+            suggestions.extend(
+                [
+                    {
+                        "question_name": f"{self._generations}-{idx}-rationale",
+                        "value": rationale,
+                    }
+                    for idx, rationale in enumerate(input[self._rationales])
+                    if rationale is not None and isinstance(rationale, str)
+                ],
+            )
+        return suggestions
+
+    @override
+    def process(self, inputs: StepInput) -> "StepOutput":  # type: ignore
+        """Creates and pushes the records as FeedbackRecords to the Argilla dataset.
+
+        Args:
+            inputs: A list of Python dictionaries with the inputs of the task.
+
+        Returns:
+            A list of Python dictionaries with the outputs of the task.
+        """
+        records = []
+        for input in inputs:
+            # Generate the SHA-256 hash of the instruction to use it as the metadata
+            instruction_id = hashlib.sha256(
+                input["instruction"].encode("utf-8")  # type: ignore
+            ).hexdigest()
+
+            generations = {
+                f"{self._generations}-{idx}": generation
+                for idx, generation in enumerate(input["generations"])  # type: ignore
+            }
+
+            records.append(  # type: ignore
+                rg.FeedbackRecord(  # type: ignore
+                    fields={
+                        "id": instruction_id,
+                        "instruction": input["instruction"],  # type: ignore
+                        **generations,
+                    },
+                    suggestions=self._add_suggestions_if_any(input),  # type: ignore
                 )
-        # Then we add the model metadata from the `generation_model` and `labelling_model`
-        # columns of the dataset, if they exist.
-        metadata.update(model_metadata_from_dataset_row(dataset_row=dataset_row))
-        # Finally, we return the `FeedbackRecord` with the fields and the metadata
-        return rg.FeedbackRecord(
-            fields=fields, suggestions=suggestions, metadata=metadata
-        )
+            )
+        self._rg_dataset.add_records(records)  # type: ignore
+        yield inputs
```

### Comparing `distilabel-0.6.0/src/distilabel/tasks/critique/__init__.py` & `distilabel-1.0.0/src/distilabel/steps/argilla/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/src/distilabel/tasks/critique/prometheus.py` & `distilabel-1.0.0/src/distilabel/llms/llamacpp.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,107 +8,124 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import re
-from dataclasses import dataclass
-from typing import Any, ClassVar, Dict, List
-
-from distilabel.tasks.base import get_template
-from distilabel.tasks.critique.base import CritiqueTask, CritiqueTaskOutput
-from distilabel.tasks.prompt import Prompt
-
-_PROMETHEUS_TEMPLATE = get_template("prometheus.jinja2")
-
-
-@dataclass
-class PrometheusTask(CritiqueTask):
-    """A `CritiqueTask` following the prompt templated used by Prometheus.
-
-    Args:
-        system_prompt (str, optional): the system prompt to be used for generation. Defaults to `None`.
-        scoring_criteria (str): the scoring criteria to be used for the task, that defines
-            the scores below, provided via `score_descriptions`.
-        score_descriptions (Dict[int, str]): the descriptions of the scores, where
-            the key is the rating value (ideally those should be consecutive), and the
-            value is the description of each rating.
-
-    Disclaimer:
-        Since the Prometheus model has been trained with OpenAI API generated data, the prompting
-        strategy may just be consistent / compliant with either GPT-3.5 or GPT-4 from OpenAI API, or
-        with their own model. Any other model may fail on the generation of a structured output, as
-        well as providing an incorrect / inaccurate critique.
-
-    References:
-        - [`Prometheus: Inducing Fine-grained Evaluation Capability in Language Models`](https://arxiv.org/abs/2310.08491)
-        - [`kaist-ai/prometheus-13b-v1.0`](https://huggingface.co/kaist-ai/prometheus-7b-v1.0)
-        - [`kaist-ai/prometheus-13b-v1.0`](https://huggingface.co/kaist-ai/prometheus-13b-v1.0)
-    """
+from typing import TYPE_CHECKING, List, Optional
 
-    scoring_criteria: str
-    score_descriptions: Dict[int, str]
+from pydantic import Field, FilePath, PrivateAttr, validate_call
 
-    system_prompt: str = "You are a fair evaluator language model."
+from distilabel.llms.base import LLM
+from distilabel.llms.typing import GenerateOutput
+from distilabel.mixins.runtime_parameters import RuntimeParameter
+from distilabel.steps.tasks.typing import ChatType
+
+if TYPE_CHECKING:
+    from llama_cpp import CreateChatCompletionResponse, Llama
+
+
+class LlamaCppLLM(LLM):
+    """llama.cpp LLM implementation running the Python bindings for the C++ code.
+
+    Attributes:
+        chat_format: the chat format to use for the model. Defaults to `chatml`.
+        model_path: contains the path to the GGUF quantized model, compatible with the
+            installed version of the `llama.cpp` Python bindings.
+        n_gpu_layers: the number of layers to use for the GPU. Defaults to `-1`, meaning that
+            the available GPU device will be used.
+        verbose: whether to print verbose output. Defaults to `False`.
+        _model: the Llama model instance. This attribute is meant to be used internally and
+            should not be accessed directly. It will be set in the `load` method.
+
+    Runtime parameters:
+        - `model_path`: the path to the GGUF quantized model.
+        - `n_gpu_layers`: the number of layers to use for the GPU. Defaults to `-1`.
+        - `verbose`: whether to print verbose output. Defaults to `False`.
+    """
 
-    __jinja2_template__: ClassVar[str] = _PROMETHEUS_TEMPLATE
+    chat_format: str = "chatml"
+    model_path: RuntimeParameter[FilePath] = Field(
+        default=None, description="The path to the GGUF quantized model."
+    )
+    n_gpu_layers: RuntimeParameter[int] = Field(
+        default=-1,
+        description="The number of layers that will be loaded in the GPU.",
+    )
+    verbose: RuntimeParameter[bool] = Field(
+        default=False,
+        description="Whether to print verbose output from llama.cpp library.",
+    )
+
+    _model: Optional["Llama"] = PrivateAttr(...)
+
+    def load(self) -> None:
+        """Loads the `Llama` model from the `model_path`."""
+
+        try:
+            from llama_cpp import Llama
+        except ImportError as ie:
+            raise ImportError(
+                "The `llama_cpp` package is required to use the `LlamaCppLLM` class."
+            ) from ie
+
+        self._model = Llama(
+            model_path=self.model_path.as_posix(),
+            chat_format=self.chat_format,
+            n_gpu_layers=self.n_gpu_layers,
+            verbose=self.verbose,
+        )
 
-    @property
-    def input_args_names(self) -> List[str]:
-        return super().input_args_names + ["ref_completion"]
+        super().load()
 
-    def generate_prompt(
-        self, input: str, generations: List[str], ref_completion: str, **_: Any
-    ) -> Prompt:
-        """Generates a prompt following the Prometheus specification.
+    @property
+    def model_name(self) -> str:
+        """Returns the model name used for the LLM."""
+        return self._model.model_path  # type: ignore
+
+    @validate_call
+    def generate(  # type: ignore
+        self,
+        inputs: List[ChatType],
+        num_generations: int = 1,
+        max_new_tokens: int = 128,
+        frequency_penalty: float = 0.0,
+        presence_penalty: float = 0.0,
+        temperature: float = 1.0,
+        top_p: float = 1.0,
+    ) -> List[GenerateOutput]:
+        """Generates `num_generations` responses for the given input using the Llama model.
 
         Args:
-            input (str): the input to be used for the prompt.
-            generations (List[str]): the generations to be used for the prompt, in
-                this case, the ones to be critiqued.
-            ref_completion (str): the reference completion to be used for the prompt,
-                which is the reference one, assuming the one with the highest score.
+            inputs: a list of inputs in chat format to generate responses for.
+            num_generations: the number of generations to create per input. Defaults to
+                `1`.
+            max_new_tokens: the maximum number of new tokens that the model will generate.
+                Defaults to `128`.
+            frequency_penalty: the repetition penalty to use for the generation. Defaults
+                to `0.0`.
+            presence_penalty: the presence penalty to use for the generation. Defaults to
+                `0.0`.
+            temperature: the temperature to use for the generation. Defaults to `0.1`.
+            top_p: the top-p value to use for the generation. Defaults to `1.0`.
 
         Returns:
-            Prompt: the generated prompt.
-
-        Examples:
-            >>> from distilabel.tasks.critique import PrometheusTask
-            >>> task = PrometheusTask(
-            ...     scoring_criteria="Overall quality of the responses provided.",
-            ...     score_descriptions={0: "false", 1: "partially false", 2: "average", 3: "partially true", 4: "true"},
-            ... )
-            >>> task.generate_prompt(
-            ...     input="What are the first 5 Fibonacci numbers?",
-            ...     generations=["0 1 1 2 3", "0 1 1 2 3"],
-            ...     ref_completion="0 1 1 2 3",
-            ... )
-            Prompt(
-                system_prompt="You are a fair evaluator language model.",
-                formatted_prompt=""###Task Description:...",
-            )
+            A list of lists of strings containing the generated responses for each input.
         """
-        render_kwargs = {
-            "instruction": input,
-            "completion": generations,
-            "ref_completion": ref_completion,
-            "scoring_criteria": self.scoring_criteria,
-            "score_descriptions": self.score_descriptions,
-        }
-        return Prompt(
-            system_prompt=self.system_prompt,
-            formatted_prompt=self.template.render(**render_kwargs),
-        )
-
-    def parse_output(self, output: str) -> CritiqueTaskOutput:  # type: ignore
-        """Parses the output of the model into the desired format."""
-        # We use a regex instead of splitting by the delimiter because the
-        # critique may contain the delimiter, and using the regex is safer.
-        pattern = r"(.+?)\. \[RESULT\] (\d+)"
-        match = re.search(pattern, output)
-        if match:
-            return CritiqueTaskOutput(
-                score=float(match.group(2)),
-                critique=match.group(1).strip(),
-            )
+        batch_outputs = []
+        for input in inputs:
+            outputs = []
+            for _ in range(num_generations):
+                chat_completions: "CreateChatCompletionResponse" = (
+                    self._model.create_chat_completion(  # type: ignore
+                        messages=input,  # type: ignore
+                        max_tokens=max_new_tokens,
+                        frequency_penalty=frequency_penalty,
+                        presence_penalty=presence_penalty,
+                        temperature=temperature,
+                        top_p=top_p,
+                    )
+                )
+                outputs.append(chat_completions["choices"][0]["message"]["content"])
+            batch_outputs.append(outputs)
+        return batch_outputs
```

### Comparing `distilabel-0.6.0/src/distilabel/tasks/preference/__init__.py` & `distilabel-1.0.0/src/distilabel/steps/globals/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/src/distilabel/tasks/preference/complexity_scorer.py` & `distilabel-1.0.0/src/distilabel/steps/tasks/complexity_scorer.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,81 +9,83 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
-from dataclasses import dataclass
-from typing import Any, Dict, List
+from typing import TYPE_CHECKING, Any, Dict, List, Union
 
-from distilabel.tasks.base import get_template
-from distilabel.tasks.preference.base import PreferenceTaskNoRationale
-from distilabel.tasks.prompt import Prompt
+from jinja2 import Template
+from pydantic import PrivateAttr
 
-_COMPLEXITY_SCORER_TEMPLATE = get_template("complexity-scorer.jinja2")
+from distilabel.steps.tasks.base import Task
 
+if TYPE_CHECKING:
+    from distilabel.steps.tasks.typing import ChatType
 
-@dataclass
-class ComplexityScorerTask(PreferenceTaskNoRationale):
-    """A `PreferenceTask` following the `Complexity Scorer` specification for rating instructions
-    in terms of complexity.
+_COMPLEXITY_SCORER_TEMPLATE = """
+Ranking the following questions according to the difficulty and complexity. Score 1-{{ instructions|length }}.
+You can give a score of {{ (instructions|length) + 1 }} if the question is too complex for you to answer it. You should
+respond with the format:
+[1] Score: 1
+[2] Score: 2
+...
+{% for instruction in instructions %}
+[{{ loop.index }}] {{ instruction }}
+{%- endfor %}
+""".lstrip()
 
-    This task is inspired by the Evol Complexity Scorer in the Deita framework: *Deita is an open-sourced project
-    designed to facilitate Automatic Data Selection for instruction tuning in Large Language Models (LLMs).*
+_PARSE_SCORE_LINE_REGEX = re.compile(r"\[\d+\] score: (\d+)", re.IGNORECASE)
 
-    The task is defined as follows:
-    Ask an LLM (in the original paper they used ChatGPT) to rate the instructions (the number of instructions
-    is dynamic in the sense that you can compare any number, in *Deita* the chose 6) to obtain a complexity
-    score *c* for each instruction.
 
-    This task will only need to receive the list of `generations` in a dataset to generate the scores.
+class ComplexityScorer(Task):
+    """This task is used to rank a list of instructions based on their complexity. It's
+    an implementation of the complexity score task from the paper 'What Makes Good Data
+    for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning'.
 
-    Args:
-        system_prompt (str, optional): the system prompt to be used. Not defined for this task.
+    Attributes:
+        _template: The Jinja2 template used to format the input data.
+
+    Input columns:
+        - instructions (`List[str]`): The list of instructions to be scored.
+
+    Output columns:
+        - complexity_score (`List[float]`): The complexity score for each instruction.
 
     References:
         - [`What Makes Good Data for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning`](https://arxiv.org/abs/2312.15685)
     """
 
-    system_prompt: str = ""
+    _template: Union[Template, None] = PrivateAttr(...)
 
-    __jinja2_template__: str = _COMPLEXITY_SCORER_TEMPLATE
+    def load(self) -> None:
+        super().load()
+        self._template = Template(_COMPLEXITY_SCORER_TEMPLATE)
 
-    def generate_prompt(self, generations: List[str], **_: Any) -> Prompt:
-        """Generates a prompt following the *Evol Complexity* specification in *Deita*.
-
-        Args:
-            generations (List[str]): the generations to be used for the prompt.
-
-        Returns:
-            Prompt: the generated prompt.
-
-        Examples:
-            >>> from distilabel.tasks import ComplexityScorerTask
-            >>> task = ComplexityScorerTask()
-            >>> task.generate_prompt(["instruction 1", "instruction 2"])
-            Prompt(system_prompt="", formatted_prompt="Ranking the following questions...")
-        """
-        render_kwargs = {"instructions": generations}
-        return Prompt(
-            system_prompt=self.system_prompt,
-            formatted_prompt=self.template.render(**render_kwargs),
-        )
+    @property
+    def inputs(self) -> List[str]:
+        return ["instructions"]
 
     @property
-    def input_args_names(self) -> List[str]:
-        """Returns the names of the input arguments of the task."""
-        return ["generations"]
-
-    def parse_output(self, output: str) -> Dict[str, List[str]]:
-        """Parses the output of the task, returning a list with the rank/score of each instruction.
-
-        Args:
-            output (str): The output of the LLM raw.
-
-        Returns:
-            Dict[str, List[str]]: A dict with containing the ranks/scores of each instruction.
-        """
-        output = output.lower().split("\n")
-        scores = [float(re.sub(r"\[\d+\] score:", "", o).strip()) for o in output]
-        return {self.output_args_names[0]: scores}
+    def outputs(self) -> List[str]:
+        return ["scores"]
+
+    def format_input(self, input: Dict[str, Any]) -> "ChatType":
+        return [{"role": "user", "content": self._template.render(**input)}]  # type: ignore
+
+    def format_output(
+        self, output: Union[str, None], input: Dict[str, Any]
+    ) -> Dict[str, Any]:
+        if output is None:
+            return {"scores": [None] * len(input["instructions"])}
+
+        scores = []
+        score_lines = output.split("\n")
+        for i, line in enumerate(score_lines):
+            match = _PARSE_SCORE_LINE_REGEX.match(line)
+            score = float(match.group(1)) if match else None
+            scores.append(score)
+            if i == len(input["instructions"]) - 1:
+                break
+
+        return {"scores": scores}
```

### Comparing `distilabel-0.6.0/src/distilabel/tasks/text_generation/__init__.py` & `distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/src/distilabel/tasks/text_generation/evol_instruct.py` & `distilabel-1.0.0/docs/sections/learn/steps/index.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,209 +1,167 @@
-# Copyright 2023-present, Argilla, Inc.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import sys
-
-if sys.version_info < (3, 9):
-    import importlib_resources
-else:
-    import importlib.resources as importlib_resources
-
-import random
-import string
-from dataclasses import dataclass
-from typing import Any, Dict, List, Literal, Optional, get_args
-
-from distilabel.logger import get_logger
-from distilabel.tasks.base import get_template
-from distilabel.tasks.prompt import Prompt
-from distilabel.tasks.text_generation.base import TextGenerationTask
-from distilabel.tasks.text_generation.mixins import InstructTaskMixin
-
-logger = get_logger()
-
-
-_EVOL_INSTRUCT_TEMPLATE = get_template("evol-instruct.jinja2")
-
-
-EvolutionMethod = Literal[
-    "breadth", "constraints", "deepen", "concretizing", "reasoning"
-]
-
-
-def _get_stopwords() -> List[str]:
-    """Gets the list of english stopwords from nltk package.
-
-    Returns:
-        List[str]: stopwords list.
-    """
-    try:
-        with (
-            importlib_resources.files("distilabel") / "tasks/_internal/stopwords_en.txt"
-        ).open("r") as f:
-            return f.read().split("\n")
-    except FileNotFoundError:
-        return []
-
-
-@dataclass
-class EvolInstructTask(InstructTaskMixin, TextGenerationTask):
-    """A `TextGenerationTask` following the `EvolInstruct` specification for building the prompts.
-
-    From the reference repository: *Evol-Instruct is a novel method using LLMs instead of humans to automatically mass-produce
-    open-domain instructions of various difficulty levels and skills range, to improve the performance of LLMs.*
-
-    The task is defined as follows:
-    Starting from an initial (simpler) instruction, select in-depth or in-breadth evolving to upgrade the simple instruction
-    to a more complex one or create a new one (to increase diversity).
-    The In-depth Evolving includes the following operations: add constraints, deepening, concretizing and increase reasoning.
-    The In-breadth Evolving is mutation, i.e., generating a completely new instruction based on the given instruction.
-
-    Given the evolved instructions are generated from LLMs, sometimes the evolving will fail. We adopt an instruction eliminator
-    to filter the failed instructions, called Elimination Evolving, but we don't apply the step of asking again to the LLM it the
-    answer is a copy from the same used prompt.
-
-    This evolutionary process can be repeated for several rounds to obtain instruction data containing various complexities.
-    Currently the task is implemented as a single step, so to generate multiple evolutions you can "repeat" the instructions
-    in the original dataset. An example can be seen at the following script:
-    [examples/pipeline-evol-instruct-alpaca.py](https://github.com/argilla-io/distilabel/tree/main/examples/pipeline-evol-instruct-alpaca.py)
-
-    Args:
-        system_prompt (str, optional): the system prompt to be used. Not defined for this task.
-
-    References:
-        - [`WizardLM: Empowering Large Language Models to Follow Complex Instructions`](https://arxiv.org/abs/2304.12244)
-    """
-
-    system_prompt: str = ""
-
-    __jinja2_template__: str = _EVOL_INSTRUCT_TEMPLATE
-
-    def generate_prompt(
-        self, input: str, evolution_method: Optional[EvolutionMethod] = None, **_: Any
-    ) -> Prompt:
-        """Generates a prompt following the Evol-Instruct specification.
-
-        Args:
-            input (str): the input to be used for the prompt.
-            evolution_method (str, optional): The evolution method to be used. If not provided (the default), a random one is chosen
-                like the original paper. Available ones are "breadth", "constraints", "deepen", "concretizing" and "reasoning".
-
-        Returns:
-            Prompt: the generated prompt.
-
-        Examples:
-            >>> from distilabel.tasks.text_generation import EvolInstructTask
-            >>> task = EvolInstructTask()
-            >>> task.generate_prompt("Give three tips for staying healthy.")
-            Prompt(
-                system_prompt="",
-                formatted_prompt="I want you to act as a Prompt ...",
-            )
-        """
-        evolution_method = self._get_evolution_method(evolution_method, EvolutionMethod)
-
-        render_kwargs = {
-            "evol_method": evolution_method,
-            "instruction": input,
-        }
-        return Prompt(
-            system_prompt=self.system_prompt,
-            formatted_prompt=self.template.render(**render_kwargs),
-        )
+# Steps
+
+The [`Step`][distilabel.steps.base.Step] is the base class in `distilabel`, every unit of work in a `Pipeline` will inherit from it.
+
+## What's a Step in distilabel?
+
+It's a base class is in charge of processing data, which in the end will be lists of dictionaries. In order to process, it defines two properties: `inputs` and `outputs`, which are a list of strings that represent the names of the columns that the step needs as input or output respectively i.e. the keys that have to be present in the list of dictionaries received by the step and the keys that will be added to these dictionaries after running it.
+
+Every `Step` is connected to a `Pipeline`, which in practice means that we will build them in the context of a `Pipeline`.
+
+Lastly, these steps inherit from `pydantic.BaseModel`, so all the attributes of a step will be validated upon definition.
+
+## An example: ConversationTemplate
+
+Let's see one simple type of step as an example, the [`ConversationTemplate`][distilabel.steps.conversation.ConversationTemplate]. Let's take a look at it's definition (the docstrings are removed for clarity, but it can be reviewd in the API reference):
+
+```python
+class ConversationTemplate(Step):
+
+    @property
+    def inputs(self) -> List[str]:
+        return ["instruction", "response"]
 
     @property
-    def output_args_names(self) -> List[str]:
-        return ["instructions"]
+    def outputs(self) -> List[str]:
+        return ["conversation"]
+
+    def process(self, inputs: StepInput) -> "StepOutput":
+        for input in inputs:
+            input["conversation"] = [
+                {"role": "user", "content": input["instruction"]},
+                {"role": "assistant", "content": input["response"]},
+            ]
+        yield inputs
+```
+
+At the very minimal, we need to define the `inputs` and `outputs` properties with the column names required as input, and returned as output respectively, and the processing logic of the step in the `process` method.
+
+In this example, we see that it takes `inputs` as argument, annotated as `StepInput`, which is a list of dictionaries with the data, and *yields* a `StepOutput`.
+
+### Working with the step
+
+Let's see how to instantiate this `Step` outside of a `Pipeline`:
+
+```python
+from distilabel.pipeline.local import Pipeline
+from distilabel.steps.conversation import ConversationTemplate
+
+conversation_template = ConversationTemplate(
+    name="my-conversation-template",
+    pipeline=Pipeline(name="my-pipeline"),
+)
+```
+
+As we mentioned, every `Step` must be defined in the context of a `Pipeline`, which means we need to pass it as an argument if we decide to create a standalone step. If we take a look at the `conversation_template` step, we see the following fields:
+
+```python
+conversation_template
+# ConversationTemplate(name='my-conversation-template', input_mappings={}, output_mappings={}, input_batch_size=50)
+```
+
+- The `name` of the `Step`, a mandatory field to identify the `Step` within the `Pipeline`. 
+- `input_mappings`, which is a dictionary that can be useful to map keys from the input dictionaries to the keys expected by the step. For example, if `input_mappings={"instruction": "prompt"}`, that means that the key `prompt` from the input dictionaries will be used as the key `instruction` for the step.
+- `output_mappings`, which is a dictionary that can be used to map the `outputs` of the step to other names. For example, if `output_mappings={"conversation": "prompt"}`, that means that the key `conversation` generated by the step will be renamed to `prompt` and the output dictionaries of this step will contain a key called `prompt` instead of `conversation`.
+- `input_batch_size` (by default set to 50), which is independent for every step and will determine how many input dictionaries will process at once. If won't matter that much in this step, but as we will see later, other types of steps will come with an `LLM`, so having this flexibility will be really useful.
+
+### Processing data
+
+Internally, the `Pipeline` will call the `process` method when appropriate, but we can see it in action with some dummy data:
+
+```python
+next(conversation_template.process([{"instruction": "Hello", "response": "Hi"}]))
+# [
+#   {
+#     "instruction": "Hello",
+#     "response": "Hi",
+#     "conversation": [
+#       {
+#         "role": "user",
+#         "content": "Hello"
+#       },
+#       {
+#         "role": "assistant",
+#         "content": "Hi"
+#       }
+#     ]
+#   }
+# ]
+```
+
+It takes the dictionary with data, adds another `conversation` with the data formatted as a conversation template, and passes this data to the following step.
+
+This is a small type step that shows what to expect when we are creating our `Step` objects, which can start from something as simple as generating a conversation template from some columns on a dataset.
+
+
+## Runtime Parameters
+
+Let's take a look at a special argument implementation that we will find when dealing with the `Steps`, the [Runtime parameters][distilabel.mixins.runtime_parameters.RuntimeParameter]. Let's inspect them using the previous example class:
+
+```python
+print(conversation_template.runtime_parameters_names)
+# {'input_batch_size': True}
+```
+
+The `ConversationTemplate` only has one `runtime_parameter`, which comes defined from the `Step` class, and can be defined as such:
+
+```python
+from distilabel.mixins.runtime_parameters import RuntimeParameter
+
+class Step(...):
+    ...
+    input_batch_size: RuntimeParameter[PositiveInt] = Field(
+        default=DEFAULT_INPUT_BATCH_SIZE,
+        description="The number of rows that will contain the batches processed by the"
+        " step.",
+    )
+```
+
+When we define the `input_batch_size` as a `RuntimeParameter`, the most direct effect we can see is we have some access to some extra information, thanks to the [RuntimeParamatersMixin][distilabel.mixins.runtime_parameters.RuntimeParametersMixin]:
+
+```python
+print(conversation_template.get_runtime_parameters_info())
+# [{'name': 'input_batch_size', 'optional': True, 'description': 'The number of rows that will contain the batches processed by the step.'}]
+```
+
+But other than accessing some extra information internally, we can directly interact with these parameters when we interacting or modifying the arguments of our `Steps` while running them in the context of a `Pipeline`. We will see them in action once we interact with the `Steps` inside of a `Pipeline`.
+
+## step decorator
+
+If all that we want to apply in a step is some simple processing, it can be easier to just create a plain function, and decorate it. We can find more examples in the [API reference][distilabel.steps.decorator], but let's see how we could define the previous step as a function and use the decorator:
+
+```python
+from distilabel.steps import StepInput, StepOutput, step 
+
+# Normal step
+@step(inputs=["instruction", "response"], outputs=["conversation"])
+def ConversationTemplate(inputs: StepInput) -> StepOutput:
+    for input in inputs:
+        input["conversation"] = [
+            {"role": "user", "content": input["instruction"]},
+            {"role": "assistant", "content": input["response"]},
+        ]
+    yield inputs
+```
+
+Which can be instantiated exactly the same as the `ConversationTemplate` class:
+
+```python
+conversation_template = ConversationTemplate(
+    name="my-conversation-template",
+    pipeline=Pipeline(name="my-pipeline"),
+)
+```
+
+This `@step` decorator has a special type depending `step_type` which will be better understood once we see the different types of steps.
+
+## Types of steps
+
+Other than the general or normal steps we have seen, there are special types of steps that have a restricted behaviour compared to the general `Step`.
+
+### Generator steps
+
+These are steps that are able to generate data, and don't need to receive any input from previous step, as it's implied in the normal steps. The typical use for these steps will be loading data for example, as can be seen in [`LoadDataFromDicts`][distilabel.steps.generators.data]. For this type of steps we will only need to define the `process` method, and we can optionally pass a `batch_size` argument, that will determine the batch size of the generated batches.
+
+### Global steps
 
-    def _elimination_evolving(
-        self, output: str, response_words: Optional[List[str]] = None
-    ) -> Optional[str]:
-        """Performs the elimination step of the Evol-Instruct task, steps 2-4 in the paper:
-
-        1. [NOT IMPLEMENTED] The evolved instruction does not provide any information gain compared
-        to the original one. Use ChatGPT to make this determination, this is outlined in Appendix G of the original paper.
-        2. The evolved instruction makes it difficult for the LLM to generate a response. We found that
-        when the generated response contains “sorry” and is relatively short in length (i.e., less than
-        80 words), it often indicates that the LLM struggles to respond to the evolved instruction.
-        So we can use this rule to make a judgment.
-        3. The response generated by the LLM only contains punctuation and stop words.
-        4. The evolved instruction obviously copies some words from the evolving prompt, such as
-        “given prompt”, “rewritten prompt”, “#Rewritten Prompt#”, etc.
-        """
-        output = output.strip()
-        if output == "":
-            return
-
-        # 2) The evolved instruction makes it difficult for the LLM to generate a response.
-        if "sorry" in output.lower() and len(output.split(" ")) < 80:
-            logger.info(
-                f"Evolution step removed the output, it's hard for the LLM to generate a response: {output}"
-            )
-            return
-
-        # 3) The output only contains punctuation and stop words
-        stopwords = _get_stopwords()
-        clean_output = [word for word in output.split(" ") if word not in stopwords]
-        if set(clean_output).difference(set(string.punctuation)) == 0:
-            logger.info(
-                f"Evolution step removed the output, it only contains punctuation and stop words: {output}"
-            )
-            return
-
-        # 4) Remove copied words from the prompt
-        prompt_words = {
-            "#Given Prompt#",
-            "#Created Prompt#",
-            "given prompt",
-            "created prompt",
-            "#The Given Prompt#",
-            "#Rewritten Prompt#",
-            "rewritten prompt",
-        }
-        if response_words:
-            prompt_words = prompt_words.union(response_words)
-        if any(word in output for word in prompt_words):
-            logger.info(
-                f"Evolution step removed the output due to word repetition from the prompt: {output}"
-            )
-            return
-
-        return output
-
-    def _get_evolution_method(
-        self, chosen_method: EvolutionMethod, available_methods: EvolutionMethod
-    ) -> None:
-        available_methods = get_args(available_methods)
-        if not chosen_method:
-            chosen_method = random.choice(available_methods)
-        if chosen_method not in available_methods:
-            raise ValueError(
-                f"Evolution method {chosen_method} is not available. Available ones are: {available_methods}"
-            )
-        return chosen_method
-
-    def parse_output(self, output: str) -> Dict[str, List[str]]:
-        """Parses the output of the model into the desired format, applying the elimination step for bad generations.
-
-        Args:
-            output (str): the output of the model.
-
-        Note:
-            The elimination step is applied to the output, but only steps 2-4 in the paper are implemented.
-            Refer to point 3.2, Elimination Evolving section in [`WizardLM: Empowering Large Language Models to Follow Complex Instructions`](https://arxiv.org/abs/2304.12244)
-            for more information on the elimination evolving step, and take a look at the `_elimination_evolving`
-            method for more information of the implementation.
-        """
-        output = self._elimination_evolving(output)
-        return {self.output_args_names[0]: output}
+Other special type of step are the global steps. These steps don't have any `inputs` or `outputs`, and their `process` method receives all the data at once instead of using batches. This kind of behavior is necessary for example to push a dataset to a specific place, or doing some filtering on the whole data before continuing with the pipeline.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `distilabel-0.6.0/src/distilabel/tasks/text_generation/evol_quality.py` & `distilabel-1.0.0/docs/sections/papers/ultrafeedback.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,145 +1,147 @@
-# Copyright 2023-present, Argilla, Inc.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-
-from dataclasses import dataclass
-from typing import Any, Dict, List, Literal, Optional
-
-from distilabel.tasks.base import get_template
-from distilabel.tasks.prompt import Prompt
-from distilabel.tasks.text_generation.evol_instruct import EvolInstructTask
-
-_EVOL_QUALITY_TEMPLATE = get_template("evol-quality.jinja2")
-
-
-EvolutionMethod = Literal[
-    "helpfulness",
-    "relevance",
-    "depth",
-    "creativity",
-    "details",
-]
-
-
-@dataclass
-class EvolQualityTask(EvolInstructTask):
-    """A `TextGenerationTask` following the `Deita` specification for improving the *quality* of instructions.
-
-    From the reference repository: *DEITA (short for Data-Efficient Instruction Tuning for Alignment),
-    a series of models fine-tuned from LLaMA and Mistral models using data samples automatically
-    selected with our proposed approach*.
-
-    The task is defined as follows:
-    Starting from an initial (simpler) instruction response, select an evolving-method to upgrade the quality
-    of the instruction. The Evolving methods includes the following operations: add "helpfulness", "relevance",
-    "depth", "creativity" and "details".
-
-    Given the evolved responses are generated from LLMs, sometimes the evolving will fail.
-    We adopt an responses eliminator to filter the failed instructions, called Elimination Evolving,
-    but we don't apply the step of asking again to the LLM it the answer is a copy from the same used
-    prompt. Note that we slightly modify the elimination evolving step, from the original paper, to
-    allow for filtering of the responses.
-
-    This evolutionary process can be repeated for several rounds to obtain instruction data containing various
-    complexities. Currently the task is implemented as a single step, so to generate multiple evolutions you
-    can "repeat" the instructions in the original dataset. An example of a similar implementation with
-    `EvolInstruct` can be seen at the following script: [examples/pipeline-evol-instruct-alpaca.py](https://github.com/argilla-io/distilabel/tree/main/examples/pipeline-evol-instruct-alpaca.py)
-
-    Args:
-        system_prompt (str, optional): the system prompt to be used. Not defined for this task.
-
-    References:
-        - [`What Makes Good Data for Alignment? A Comprehensive Study of Automatic Data Selection in Instruction Tuning`](https://arxiv.org/abs/2312.15685)
-        - [`WizardLM: Empowering Large Language Models to Follow Complex Instructions`](https://arxiv.org/abs/2304.12244)
-    """
-
-    system_prompt: str = ""
-
-    __jinja2_template__: str = _EVOL_QUALITY_TEMPLATE
-
-    def generate_prompt(
-        self,
-        input: str,
-        generation: str,
-        evolution_method: Optional[EvolutionMethod] = None,
-        **_: Any,
-    ) -> Prompt:
-        """Generates a prompt following the Evol-Instruct specification.
-
-        Args:
-            input (str):
-                The input to be used for the prompt. Corresponds to the instruction in the prompt.
-            generation (str):
-                The generation to be used for the prompt, which corresponds to a generated response
-                given the instruction given in the input.
-            evolution_method (str, optional):
-                The evolution method to be used. If not provided (the default), a random one is chosen
-                like the original paper. Available ones are "helpfulness", "relevance", "deepen",
-                "creativity" and "details".
-
-        Returns:
-            Prompt: the generated prompt.
-
-        Examples:
-            >>> from distilabel.tasks.text_generation import EvolQualityTask
-            >>> task = EvolQualityTask()
-            >>> task.generate_prompt("Give three tips for staying healthy.", "1. Eat healthy food. 2. Exercise. 3. Sleep well.")
-            Prompt(
-                system_prompt="",
-                formatted_prompt="I want you to act as a Prompt ...",
-            )
-        """
-        evolution_method = self._get_evolution_method(evolution_method, EvolutionMethod)
-
-        render_kwargs = {
-            "evol_method": evolution_method,
-            "instruction": input,
-            "generation": generation,
-        }
-        return Prompt(
-            system_prompt=self.system_prompt,
-            formatted_prompt=self.template.render(**render_kwargs),
-        )
-
-    @property
-    def input_args_names(self) -> List[str]:
-        return ["input", "generation"]
-
-    @property
-    def output_args_names(self) -> List[str]:
-        return ["generations"]
-
-    def parse_output(self, output: str) -> Dict[str, List[str]]:
-        """Parses the output of the model into the desired format, applying the elimination step for bad generations.
-
-        Args:
-            output (str): the output of the model.
-
-        Note:
-            The elimination step is applied to the output, but only steps 2-4 in the paper are implemented.
-            Refer to point 3.2, Elimination Evolving section in [`WizardLM: Empowering Large Language Models to Follow Complex Instructions`](https://arxiv.org/abs/2304.12244)
-            for more information on the elimination evolving step, and take a look at the `_elimination_evolving`
-            method for more information of the implementation.
-        """
-        response_words = {
-            "#Given Response#",
-            "#Created Response#",
-            "given response",
-            "created response",
-            "#The Given Response#",
-            "#Rewritten Response#",
-            "rewritten response",
-        }
-        output = self._elimination_evolving(output, response_words=response_words)
-        return {self.output_args_names[0]: output}
+UltraFeedback is a large-scale, fine-grained, diverse preference dataset, used for training powerful reward models and critic models.
+
+UltraFeedback collects about 64k prompts from diverse resources (including UltraChat, ShareGPT, Evol-Instruct, TruthfulQA, FalseQA, and FLAN), then they use these prompts to query multiple LLMs (commercial models, Llama models ranging 7B to 70B, and non-Llama models) and generate four different responses for each prompt, resulting in a total of 256k samples i.e. the UltraFeedback will rate four responses on every OpenAI request.
+
+To collect high-quality preference and textual feedback, they design a fine-grained annotation instruction, which contains four different aspects, namely instruction-following, truthfulness, honesty and helpfulness (even though within the paper they also mention a fifth one named verbalized calibration). Finally, GPT-4 is used to generate the ratings for the generated responses to the given prompt using the previously mentioned aspects.
+
+### Replication
+
+To replicate the paper we will be using `distilabel` and a smaller dataset created by the Hugging Face H4 team named [`HuggingFaceH4/instruction-dataset`](https://huggingface.co/datasets/HuggingFaceH4/instruction-dataset) for testing purposes.
+
+Also for testing purposes we will just show how to evaluate the generated responses for a given prompt using a new global aspect named `overall-rating` defined by Argilla, that computes the average of the four aspects, so as to reduce number of requests to be sent to OpenAI, but note that all the aspects are implemented within `distilabel` and can be used instead for a more faithful reproduction. Besides that we will generate two responses i.e. run the text generation on top of two LLMs instead of four, to reduce the compute required too.
+
+#### Installation
+
+To replicate UltraFeedback one will need to install `distilabel` as it follows:
+
+```bash
+pip install "distilabel[argilla,openai,vllm]>=1.0.0"
+```
+
+And since we will be using `vllm` we will need to use a VM with at least 2 NVIDIA GPUs with at least 16GB of memory each to run the text generation, and set the `OPENAI_API_KEY` environment variable value.
+
+#### Building blocks
+
+* `LoadHubDataset`: Generator Step to load a dataset from the Hugging Face Hub.
+* `TextGeneration`: Task to generate responses for a given instruction using an LLM.
+    * `vLLM`: LLM that loads a model from the Hugging Face Hub using `vLLM`.
+* `CombineColumns`: Task that combines multiple columns into a single one i.e. from string to list of strings. Useful when there are multiple parallel steps that are connected to the same node.
+* `UltraFeedback`: Task that generates ratings for the responses of a given instruction using the UltraFeedback prompt.
+    * `OpenAILLM`: LLM that loads a model from OpenAI using `OpenAILLM`.
+* `KeepColumns`: Task to keep the desired columns while removing the not needed ones, as well as defining the order for those. 
+* `PreferenceToArgilla`: Task to optionally push the generated dataset to Argilla to do some further analysis and human annotation.
+
+#### Code
+
+As mentioned before, we will put the previously mentioned building blocks together to replicate UltraFeedback.
+
+```python
+from distilabel.llms import OpenAILLM, vLLM
+from distilabel.pipeline import Pipeline
+from distilabel.steps import (
+    CombineColumns,
+    KeepColumns,
+    LoadHubDataset,
+    PreferenceToArgilla,
+)
+from distilabel.steps.tasks import TextGeneration, UltraFeedback
+
+
+with Pipeline(name="ultrafeedback-pipeline") as pipeline:
+    load_hub_dataset = LoadHubDataset(
+        name="load_dataset",
+        output_mappings={"prompt": "instruction"},
+    )
+
+    text_generation_with_notus = TextGeneration(
+        name="text_generation_with_notus",
+        llm=vLLM(model="argilla/notus-7b-v1"),
+        input_batch_size=10,
+        output_mappings={"model_name": "generation_model"},
+    )
+    text_generation_with_zephyr = TextGeneration(
+        name="text_generation_with_zephyr",
+        llm=vLLM(model="HuggingFaceH4/zephyr-7b-gemma-v0.1"),
+        input_batch_size=10,
+        output_mappings={"model_name": "generation_model"},
+    )
+    load_hub_dataset.connect(text_generation_with_notus)
+    load_hub_dataset.connect(text_generation_with_zephyr)
+
+    combine_columns = CombineColumns(
+        name="combine_columns",
+        columns=["generation", "generation_model"],
+        output_columns=["generations", "generation_models"],
+    )
+    text_generation_with_notus.connect(combine_columns)
+    text_generation_with_zephyr.connect(combine_columns)
+
+    ultrafeedback = UltraFeedback(
+        name="ultrafeedback_openai",
+        llm=OpenAILLM(model="gpt-4"),
+        aspect="overall-rating",
+        output_mappings={"model_name": "ultrafeedback_model"},
+    )
+    combine_columns.connect(ultrafeedback)
+
+    keep_columns = KeepColumns(
+        name="keep_columns",
+        columns=[
+            "instruction",
+            "generations",
+            "generation_models",
+            "ratings",
+            "rationales",
+            "ultrafeedback_model",
+        ],
+    )
+    ultrafeedback.connect(keep_columns)
+
+    # # Optional: Push the generated dataset to Argilla, but will need to `pip install argilla` first
+    # push_to_argilla = PreferenceToArgilla(
+    #     name="push_to_argilla",
+    #     api_url="<ARGILLA_API_URL>",
+    #     api_key="<ARGILLA_API_KEY>",  # type: ignore
+    #     dataset_name="ultrafeedback",
+    #     dataset_workspace="admin",
+    #     num_generations=2,
+    # )
+    # keep_columns.connect(push_to_argilla)
+```
+
+Then we need to call `pipeline.run` with the runtime parameters so that the pipeline can be launched.
+
+```python
+dataset = pipeline.run(
+    parameters={
+        "load_dataset": {
+            "repo_id": "HuggingFaceH4/instruction-dataset",
+            "split": "test",
+        },
+        "text_generation_with_notus": {
+            "generation_kwargs": {
+                "max_new_tokens": 512,
+                "temperature": 0.7,
+            },
+        },
+        "text_generation_with_zephyr": {
+            "generation_kwargs": {
+                "max_new_tokens": 512,
+                "temperature": 0.7,
+            },
+        },
+        "ultrafeedback_overall_rating": {
+            "generation_kwargs": {
+                "max_new_tokens": 1024,
+                "temperature": 0.7,
+            },
+        },
+    }
+)
+```
+
+Finally, we can optionally push the generated dataset, named `Distiset`, to the Hugging Face Hub via the `push_to_hub` method, so that each subset generated in the leaf steps is pushed to the Hub.
+
+```python
+dataset.push_to_hub("distilabel-internal-testing/ultrafeedback-instruction-dataset", private=True)
+```
```

### Comparing `distilabel-0.6.0/src/distilabel/tasks/text_generation/principles.py` & `distilabel-1.0.0/LICENSE`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,201 @@
-# Copyright 2023-present, Argilla, Inc.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-
-class UltraFeedbackPrinciples:
-    """A class containing a list of principles from the UltraFeedback paper, that can
-    be injected into the system prompt given to the LLM.
-
-    References:
-        - [`UltraFeedback: Boosting Language Models with High-quality Feedback`](https://arxiv.org/abs/2310.01377)
-        - [`UltraFeedback - GitHub Repository`](https://github.com/OpenBMB/UltraFeedback)
-    """
-
-    helpfulness = [
-        "The assistant should provide users with accurate, relevant, and up-to-date information, ensuring that the content is positive, interesting, engaging, educational, and helpful.",
-        "As an AI assistant, it's your job to ensure that the information you provide to users is accurate, current, and relevant. Offer comprehensive details to educate and engage the user.",
-        "Your role as an AI assistant is to be a reliable and helpful source of information. Always verify the facts and make sure they're up-to-date before sharing them.",
-        "As an AI assistant, inspire users with your knowledgeable insights. Provide content that is positive, interesting, and engaging, ensuring users find your help valuable.",
-        "Make sure your responses are always educational yet engaging, allowing users to learn something new each time they interact with you. You are an AI assistant after all!",
-        "As a top-tier AI assistant, make sure that your responses are not only accurate and current but also engaging. Be the positive interaction users look forward to.",
-        "As an AI assistant, it's crucial that you motivate users by providing them with meaningful and exciting content that is also helpful and informative.",
-        "Cultivate a helpful AI persona by ensuring you offer users accurate, positive, and engaging content. Make every interaction informative and delightful.",
-        "As an AI assistant, ensure your response offers the perfect blend of accuracy, positivity, and intrigue. Strive to be educational while keeping the user engaged.",
-        "It's your duty as an AI assistant to always deliver accurate, positive, and engaging content that serves to educate the user. Make every interaction a learning opportunity.",
-        "As an AI assistant, provide not just answers but also spark curiosity. Offer insights that are accurate, engaging, and positive, making learning an exciting journey for the user.",
-    ]
-    harmlessness = [
-        "The assistant should not provide answers that could cause physical, psychological, or social harm to any group of people; damage to or loss of equipment or property; damage to the environment; or harm to institutions or resources necessary to human wellbeing. Feel free to refuse to answer questions that could cause the above harm.",
-        "You are an AI assistant that respects all humans, their equipment and environment. Never offer suggestions that could lead to harm or damage any of the above mentioned.",
-        'You are an AI assistant that maintains a principle of "First do no harm". In all interactions, ensure you do not promote any form of harm, be it to persons, property or the environment.',
-        "You are an AI assistant. Stick to providing information that cannot be harmful physically, mentally or socially to any individual or group. Don't answer any queries that might lead to such consequences.",
-        "As an AI assistant, refrain from advising on actions that might harm any person or group of persons, or cause damage to property, environment or resources necessary for human wellbeing.",
-        "You're an AI helper wishing to provide safe assistance for all users. Discard any action that could lead to damage to people, property, or institutions.",
-        "You are a responsible AI assistant. Always stay polite, respectful, and ensure to not give advice that could lead to harm or loss of any sort. ",
-        "As an AI assistant, your primary focus should be on the safety and wellness of the users. Never provide answers that could cause harm or damage to individuals, their property or the environment.",
-        "You are an AI assistant that is centred around being harmless. Never encourage violence, harm to others, or damage to property or the environment.",
-        "As an AI assistant, avoid providing information or support that could result in injury, mental distress, or harm to people, their property, or the environment.",
-        "You are an AI assistant. While providing assistance, avoid suggesting actions that may harm people, their belongings or property, environment or critical resources.",
-    ]
-    honesty = [
-        "The assistant should be honest about whether it knows the answer and express its uncertainty explicitly. Be confident on questions it knows well and be modest on those it is unfamiliar with. Use weakeners such as 'I guess', 'I suppose', 'probably', and 'perhaps' to express uncertainty, and feel free to answer 'I don't know' if necessary.",
-        "As an AI, honesty is crucial to build trust with your user. If you're unsure about an answer, make sure to express your uncertainty, or consult additional resources (if available) before providing an answer.  ",
-        "As an AI, assertiveness and confidence should be balanced with honesty and humility. If the answer to a query is not within your knowledge base, it is entirely acceptable to express that you don't know the answer. ",
-        "You are an AI assistant that values honesty. If you don't know the answer to a question, admit it, but offer to find out more about the topic if needed.",
-        "You're not only an AI assistant, but also a reliable partner. Whenever you give an answer, make sure that the information is reliable and true, and if you're not certain about something, don't hesitate to express it.  ",
-        'You are an AI assistant. Your prime objective is to provide useful and accurate information. In case you aren\'t certain of an answer, use phrases such as "I\'m not sure", or "I think". Honesty always comes first.',
-        "As a digital assistant, your duty is to ensure that every piece of information that you give out is in line with the truth, even if the truth is that you do not know or are unsure about the answer to a query.",
-        "Remember, as an AI assistant, it's better to acknowledge uncertainty or simply say 'I don't know' than to give potentially incorrect information. Honesty leads to trust.",
-        "As an AI assistant, honesty is appreciated by your users. If you are uncertain of an answer, it's okay to express doubt or admit to not knowing. Offer to search for more information if needed. ",
-        "You are an AI helper that portrays honesty in every response. Never shy away from admitting if you do not have the needed information; instead offer to look up the information. ",
-        "Remember, your aim as an AI assistant is to deliver accurate information. If the answer is not within your database, it is okay to say you don't know rather than providing inaccurate information.",
-    ]
-    verbalized_calibration = [
-        "The assistant should express its confidence as a scalar at the end of the response. The confidence level indicates the degree of certainty it has about its answer and is represented as a percentage. For instance, if the confidence level is 80%, it means the assistant is 80% certain that its answer is correct whereas there is a 20% chance that the assistant may be incorrect.\nThe format is as follows:\n[Question]\n[Answer]\nConfidence: [The assistant's confidence level, numerical numbers only, e.g. 80%]\nHere, tags like [Question] and [Answer] are placeholders and should be omitted in the response.\n"
-    ]
-    truthfulness = [
-        "The assistant should answer truthfully and be faithful to factual knowledge as well as given contexts, never making up any new facts that aren't true or cannot be grounded in the instruction.",
-        "As an AI assistant, it is important that you answer truthfully. Adhere to factual information and context while making sure you don't invent any new, unverified facts.",
-        "As an AI assistant, conduct yourself with honesty. Always be diligent in giving accurate responses. Fictional facts or inaccuracies should be avoided in your responses.",
-        "As an AI assistant, stick to the truth. Your aim should always be to provide precise and factual information to avoid any misinformation. ",
-        "As an AI assistant, factual consistency is key. Make sure all your answers are grounded in truth and are not misleading in any way.",
-        "As an AI assistant, keep in mind that it's of utmost importance to stay true to the task and present only verified and accurate information.",
-        "As an AI assistant, find and uphold the truth in every answer. Ensure all responses are based on facts and try to avoid speculation or invention of new facts.",
-        "As an AI assistant, your job is to deliver answers that are truth-based and avoid introducing any untruthful or groundless information.",
-        "As an AI assistant, maintain objectivity while answering questions. Make sure the information given is truthful and never fabricated.",
-        "As an AI assistant, maintain the integrity of your responses. Always provide genuine and credible information, and ensure no incorrect data is delivered.",
-        "As an AI assistant, operate under the principle of truthfulness. Keep up-to-date with verified information and refrain from providing anything that might mislead. \n",
-    ]
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [2023-present] [Argilla, Inc.]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `distilabel-0.6.0/src/distilabel/tasks/text_generation/self_instruct.py` & `distilabel-1.0.0/src/distilabel/steps/tasks/self_instruct.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,98 +8,122 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import re
-from dataclasses import dataclass
-from typing import Any, Dict, List
-
-from distilabel.tasks.base import get_template
-from distilabel.tasks.prompt import Prompt
-from distilabel.tasks.text_generation.base import TextGenerationTask
-from distilabel.tasks.text_generation.mixins import InstructTaskMixin
-
-_SELF_INSTRUCT_TEMPLATE = get_template("self-instruct.jinja2")
-
-
-@dataclass
-class SelfInstructTask(InstructTaskMixin, TextGenerationTask):
-    """A `TextGenerationTask` following the Self-Instruct specification for building
-    the prompts.
-
-    Args:
-        system_prompt (str, optional): the system prompt to be used. Defaults to `None`.
-        principles (Dict[str, List[str]], optional): the principles to be used for the system prompt.
-            Defaults to `None`.
-        principles_distribution (Union[Dict[str, float], Literal["balanced"], None], optional): the
-            distribution of principles to be used for the system prompt. Defaults to `None`.
-        application_description (str, optional): the description of the AI application. Defaults to
-            "AI assistant".
-        num_instructions (int, optional): the number of instructions to be used for the prompt.
-            Defaults to 5.
-        criteria_for_query_generation (str, optional): the criteria for query generation that we want
-            our model to have. Default value covers default behaviour for SelfInstructTask. This value is
-            passed to the .jinja template, where extra instructions are added to ensure correct output format.
+import sys
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
-    References:
+if sys.version_info < (3, 9):
+    import importlib_resources
+else:
+    import importlib.resources as importlib_resources
+
+from jinja2 import Template
+from pydantic import PrivateAttr
+
+from distilabel.steps.tasks.base import Task
+
+if TYPE_CHECKING:
+    from distilabel.steps.tasks.typing import ChatType
+
+
+class SelfInstruct(Task):
+    """SelfInstruct is a pre-defined task that, given a number of instructions, a
+    certain criteria for query generations, an application description, and an input,
+    generates a number of instruction related to the given input and following what
+    is stated in the criteria for query generation and the application description.
+    It is based in the SelfInstruct framework from the paper "Self-Instruct: Aligning
+    Language Models with Self-Generated Instructions".
+
+    Attributes:
+        num_instructions: The number of instructions to be generated. Defaults to 5.
+        criteria_for_query_generation: The criteria for the query generation. Defaults
+            to the criteria defined within the paper.
+        application_description: The description of the AI application that one want
+            to build with these instructions. Defaults to `AI assistant`.
+
+    Input columns:
+        - input (`str`): The input to generate the instructions. It's also called seed in the paper.
+
+    Output columns:
+        - instructions (`List[str]`): The generated instructions.
+
+    Reference:
         - [`Self-Instruct: Aligning Language Models with Self-Generated Instructions`](https://arxiv.org/abs/2212.10560)
-        - [`Self-Instruct - GitHub Repository`](https://github.com/yizhongw/self-instruct)
     """
 
-    system_prompt: str = (
-        "You are an expert prompt writer, writing the best and most diverse prompts for a variety of tasks."
-        " You are given a task description and a set of instructions for how to write the prompts for an"
-        " specific AI application."
-    )
-
-    application_description: str = "AI assistant"
     num_instructions: int = 5
 
     criteria_for_query_generation: str = (
         "Incorporate a diverse range of verbs, avoiding repetition.\n"
         "Ensure queries are compatible with AI model's text generation functions and are limited to 1-2 sentences.\n"
         "Design queries to be self-contained and standalone.\n"
         'Blend interrogative (e.g., "What is the significance of x?") and imperative (e.g., "Detail the process of x.") styles.'
     )
 
-    __jinja2_template__: str = _SELF_INSTRUCT_TEMPLATE
+    application_description: str = "AI assistant"
+
+    _template: Template = PrivateAttr(default=...)
+
+    def load(self) -> None:
+        """Loads the Jinja2 template for SelfInstruct."""
+        super().load()
+
+        _path = str(
+            importlib_resources.files("distilabel")
+            / "steps"
+            / "tasks"
+            / "templates"
+            / "self-instruct.jinja2"
+        )
 
-    def generate_prompt(self, input: str, **_: Any) -> Prompt:
-        """Generates a prompt following the Self-Instruct specification.
+        self._template = Template(open(_path).read())
+
+    @property
+    def inputs(self) -> List[str]:
+        """The input for the task is the `input` i.e. seed text."""
+        return ["input"]
+
+    def format_input(self, input: Dict[str, Any]) -> "ChatType":
+        """The input is formatted as a `ChatType` assuming that the instruction
+        is the first interaction from the user within a conversation."""
+
+        return [
+            {
+                "role": "user",
+                "content": self._template.render(
+                    input=input["input"],
+                    application_description=self.application_description,
+                    criteria_for_query_generation=self.criteria_for_query_generation,
+                    num_instructions=self.num_instructions,
+                ),
+            }
+        ]
+
+    @property
+    def outputs(self):
+        """The output for the task is a list of `instructions` containing the generated instructions."""
+        return ["instructions"]
+
+    def format_output(
+        self,
+        output: Union[str, None],
+        input: Optional[Dict[str, Any]] = None,
+    ) -> Dict[str, Any]:
+        """The output is formatted as a list with the generated instructions.
 
         Args:
-            input (str): the input to be used for the prompt.
+            output: the raw output of the LLM.
+            input: the input to the task. Used for obtaining the number of responses.
 
         Returns:
-            Prompt: the generated prompt.
-
-        Examples:
-            >>> from distilabel.tasks.text_generation import SelfInstructTask
-            >>> task = SelfInstructTask(system_prompt="You are a helpful assistant.", num_instructions=2)
-            >>> task.generate_prompt("What are the first 5 Fibonacci numbers?")
-            Prompt(
-                system_prompt="You are a helpful assistant.",
-                formatted_prompt="# Task Description ...",
-            )
+            A dict with containing the generated instructions.
         """
-        render_kwargs = {
-            "application_description": self.application_description,
-            "num_instructions": self.num_instructions,
-            "criteria_for_query_generation": self.criteria_for_query_generation,
-            "input": input,
-        }
-        return Prompt(
-            system_prompt=self.system_prompt,
-            formatted_prompt=self.template.render(**render_kwargs),
-        )
 
-    @property
-    def output_args_names(self) -> List[str]:
-        return ["instructions"]
+        if output is None:
+            return {"instructions": []}
 
-    def parse_output(self, output: str) -> Dict[str, List[str]]:
-        """Parses the output of the model into the desired format."""
-        pattern = re.compile(r"\d+\.\s*(.*?)\n")
-        return {"instructions": pattern.findall(output)}
+        lines = [line for line in output.split("\n") if line != ""]
+        return {"instructions": lines}
```

### Comparing `distilabel-0.6.0/src/distilabel/utils/__init__.py` & `distilabel-1.0.0/src/distilabel/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,10 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from distilabel.utils.dataset import prepare_dataset
+from distilabel.cli.app import app
 
-__all__ = ["prepare_dataset"]
+if __name__ == "__main__":
+    app(prog_name="distilabel")
```

### Comparing `distilabel-0.6.0/src/distilabel/utils/dicts.py` & `distilabel-1.0.0/src/distilabel/utils/dicts.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections import defaultdict
-from typing import Any, Dict
+from typing import Any, Dict, List, TypeVar
 
+_K = TypeVar("_K")
 
-def combine_dicts(*dicts: Any) -> Dict[str, Any]:
+
+def combine_dicts(*dicts: Dict[_K, Any]) -> Dict[_K, List[Any]]:
     """Combines multiple dictionaries into a single dictionary joining the values
     as a list for each key.
 
     Args:
-        *dicts (Any): the dictionaries to be combined.
+        *dicts: the dictionaries to be combined.
 
     Returns:
-        Dict[str, Any]: the combined dictionary.
+        The combined dictionary.
     """
     combined_dict = defaultdict(list)
     for d in dicts:
         for key, value in d.items():
             combined_dict[key].append(value)
     return dict(combined_dict)
```

### Comparing `distilabel-0.6.0/src/distilabel/utils/serialization.py` & `distilabel-1.0.0/src/distilabel/llms/ollama.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,144 +8,147 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import importlib
-import json
-import os
-from dataclasses import asdict
-from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, Generic, Optional, TypeVar
-
-if TYPE_CHECKING:
-    from distilabel.tasks.base import Task
-
-
-T = TypeVar("T")
-
-TASK_FILE_NAME = "distilabel-task.json"
-
-
-def load_from_dict(template: Dict[str, Any]) -> Generic[T]:
-    """Reads a template (a class serialized) and returns a the instance
-    contained.
-
-    Args:
-        template (Dict[str, Any]): Dict containing the template, the dict serialized.
-
-    Returns:
-        Generic[T]: Instance contained in the template
-    """
-    type_info = template.pop("__type_info__")
-    mod = importlib.import_module(type_info["module"])
-    cls = getattr(mod, type_info["name"])
-    instance = cls(**template)
-    return instance
-
-
-def load_task_from_disk(path: os.PathLike) -> "Task":
-    """Loads a task from disk.
-
-    Args:
-        path: The path to the task.
-
-    Returns:
-        Task: The task.
-    """
-    task_path = Path(path) / TASK_FILE_NAME
-    if not task_path.exists():
-        raise FileNotFoundError(f"The task file does not exist: {task_path}")
-
-    task_content = read_json(task_path)
-    task = load_from_dict(task_content)
-    return task
+from typing import TYPE_CHECKING, List, Literal, Optional, Sequence, Union
 
+from pydantic import Field, PrivateAttr, validate_call
+from typing_extensions import TypedDict
 
-def write_json(filename: Path, data: Dict[str, Any]) -> None:
-    """Writes a json file to the given path, creates the parent dir.
+from distilabel.llms.base import AsyncLLM
+from distilabel.mixins.runtime_parameters import RuntimeParameter
+from distilabel.steps.tasks.typing import ChatType
 
-    Args:
-        filename (Path): Name of the file.
-        data (Dict[str, Any]): Dict to be written as json.
-    """
-    filename.parent.mkdir(parents=True, exist_ok=True)
-    with open(filename, "w") as f:
-        json.dump(data, f, indent=2)
-
-
-def read_json(filename: Path) -> Dict[str, Any]:
-    """Read a json file from disk.
-
-    Args:
-        filename (Path): Name of the json file.
-
-    Returns:
-        Dict[str, Any]: Dict containing the json data.
-    """
-    with open(filename, "r") as file:
-        return json.load(file)
+if TYPE_CHECKING:
+    from ollama import AsyncClient
 
 
-class _Serializable:
-    """Base class for serializable classes.
-    It provides the means to serialize and deserialize.
-
-    We currently defien the tasks as dataclasses, in which case we can
-    use the `asdict` method to serialize the class, but we may need to review
-    this if we decide to remove the dataclasses.
-    Other than the default content, the obtained from `dataclasses.asdict`, we
-    we store create a __type_info__ variable to store the relevant information
-    to load back the class.
+# Copied from `ollama._types.Options`
+class Options(TypedDict, total=False):
+    # load time options
+    numa: bool
+    num_ctx: int
+    num_batch: int
+    num_gqa: int
+    num_gpu: int
+    main_gpu: int
+    low_vram: bool
+    f16_kv: bool
+    logits_all: bool
+    vocab_only: bool
+    use_mmap: bool
+    use_mlock: bool
+    embedding_only: bool
+    rope_frequency_base: float
+    rope_frequency_scale: float
+    num_thread: int
+
+    # runtime options
+    num_keep: int
+    seed: int
+    num_predict: int
+    top_k: int
+    top_p: float
+    tfs_z: float
+    typical_p: float
+    repeat_last_n: int
+    temperature: float
+    repeat_penalty: float
+    presence_penalty: float
+    frequency_penalty: float
+    mirostat: int
+    mirostat_tau: float
+    mirostat_eta: float
+    penalize_newline: bool
+    stop: Sequence[str]
+
+
+class OllamaLLM(AsyncLLM):
+    """Ollama LLM implementation running the Async API client.
+
+    Attributes:
+        model: the model name to use for the LLM e.g. "notus".
+        host: the Ollama server host.
+        timeout: the timeout for the LLM. Defaults to `120`.
+        _aclient: the `AsyncClient` to use for the Ollama API. It is meant to be used internally.
+            Set in the `load` method.
+
+    Runtime parameters:
+        - `host`: the Ollama server host.
+        - `timeout`: the client timeout for the Ollama API. Defaults to `120`.
     """
 
-    __type_info__: Dict[str, Any] = {}
-
-    def dump(self) -> Dict[str, Any]:
-        """Transforms the class into a dict to write to a file.
-
-        Returns:
-            Dict[str, Any]: Serializable content of the class.
-        """
-        _dict = asdict(self)
-        # Remove private variables from the dump
-        _dict = {k: v for k, v in _dict.items() if not k.startswith("__")}
-        _dict["__type_info__"] = {
-            "module": type(self).__module__,
-            "name": type(self).__name__,
-        }
-        return _dict
-
-    def save(self, path: Optional[os.PathLike] = Path.cwd() / TASK_FILE_NAME) -> None:
-        """Writes the content to a file.
-
-        Args:
-            path (Optional[os.PathLike], optional):
-                Filename of the task. If a folder is given, will create the task
-                inside. If None is given, the file will be created at the current
-                working directory. Defaults to None.
+    model: str
+    host: Optional[RuntimeParameter[str]] = Field(
+        default=None, description="The host of the Ollama API."
+    )
+    timeout: RuntimeParameter[int] = Field(
+        default=120, description="The timeout for the Ollama API."
+    )
+    follow_redirects: bool = True
+
+    _aclient: Optional["AsyncClient"] = PrivateAttr(...)
+
+    def load(self) -> None:
+        """Loads the `AsyncClient` to use Ollama async API."""
+        super().load()
+
+        try:
+            from ollama import AsyncClient
+
+            self._aclient = AsyncClient(
+                host=self.host,
+                timeout=self.timeout,
+                follow_redirects=self.follow_redirects,
+            )
+        except ImportError as e:
+            raise ImportError(
+                "Ollama Python client is not installed. Please install it using"
+                " `pip install ollama`."
+            ) from e
+
+    @property
+    def model_name(self) -> str:
+        """Returns the model name used for the LLM."""
+        return self.model
+
+    @validate_call
+    async def agenerate(  # type: ignore
+        self,
+        input: ChatType,
+        num_generations: int = 1,
+        format: Literal["", "json"] = "",
+        # TODO: include relevant options from `Options` in `agenerate` method.
+        options: Union[Options, None] = None,
+        keep_alive: Union[bool, None] = None,
+    ) -> List[str]:
         """
-        path = Path(path)
-        if path.suffix == "":
-            # If the path has no suffix, assume the user just wants a folder to write the task
-            path = path / TASK_FILE_NAME
-        write_json(path, self.dump())
-
-    @classmethod
-    def from_json(cls, path: os.PathLike) -> Generic[T]:
-        """Loads a template from a file and returns the instance contained.
+        Generates a response asynchronously, using the [Ollama Async API definition](https://github.com/ollama/ollama-python).
 
         Args:
-            template_path (os.PathLike): _description_
-
-        Raises:
-            ValueError: _description_
+            input: the input to use for the generation.
+            num_generations: the number of generations to produce. Defaults to `1`.
+            format: the format to use for the generation. Defaults to `""`.
+            options: the options to use for the generation. Defaults to `None`.
+            keep_alive: whether to keep the connection alive. Defaults to `None`.
 
         Returns:
-            Generic[T]: _description_
+            A list of strings as completion for the given input.
         """
-        if Path(path).is_dir():
-            raise ValueError(f"You must provide a file path, not a directory: {path}")
-        template = read_json(path)
-        return load_from_dict(template)
+        generations = []
+        # TODO: remove this for-loop and override the `generate` method
+        for _ in range(num_generations):
+            completion = await self._aclient.chat(  # type: ignore
+                model=self.model,
+                messages=input,  # type: ignore
+                stream=False,
+                format=format,
+                options=options,
+                keep_alive=keep_alive,
+            )
+            # TODO: improve error handling
+            generations.append(completion["message"]["content"])
+
+        return generations
```

### Comparing `distilabel-0.6.0/src/distilabel/utils/types.py` & `distilabel-1.0.0/src/distilabel/utils/files.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,27 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from __future__ import annotations
+from pathlib import Path
+from typing import List
 
-from concurrent.futures import Future
-from typing import Any, Union
 
-from typing_extensions import TypeGuard, TypeVar
-
-T = TypeVar("T")
-
-
-def is_future(obj: Union[Future[T], Any]) -> TypeGuard[Future[T]]:
-    """Checks if an object is a future narrowing the type.
+def list_files_in_dir(dir_path: Path) -> List[Path]:
+    """List all files in a directory.
 
     Args:
-        obj (Future[T]): Object to check
+        dir_path: Path to the directory.
 
     Returns:
-        TypeGuard[Future[T]]: True if it is a future
+        A list of file names in the directory.
     """
-    return isinstance(obj, Future)
+    return [f for f in dir_path.iterdir() if f.is_file()]
```

### Comparing `distilabel-0.6.0/tests/__init__.py` & `distilabel-1.0.0/src/distilabel/steps/tasks/evol_instruct/evol_complexity/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/tests/llm/__init__.py` & `distilabel-1.0.0/src/distilabel/steps/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/tests/llm/test_anyscale.py` & `distilabel-1.0.0/tests/unit/llms/test_openai.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,91 +8,99 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import re
+import os
 from unittest import mock
+from unittest.mock import AsyncMock, MagicMock, Mock, patch
 
+import nest_asyncio
 import pytest
-from distilabel.llm.anyscale import AnyscaleLLM
-from distilabel.tasks.text_generation.base import TextGenerationTask
+from distilabel.llms.openai import OpenAILLM
 
-MODEL_NAME = "argilla/notus-7b-v1"
 
+@patch("openai.AsyncOpenAI")
+class TestOpenAILLM:
+    model_id: str = "gpt-4"
 
-@mock.patch("distilabel.llm.anyscale.OpenAI")
-@mock.patch(
-    "distilabel.llm.anyscale.OpenAILLM.available_models",
-    [MODEL_NAME],
-)
-class TestAnyscaleLLM:
-    def test_llm_anyscale(self, mock_anyscale):
-        llm = AnyscaleLLM(
-            model=MODEL_NAME,
-            task=TextGenerationTask(),
-            api_key="api.key",
-        )
-        assert isinstance(llm, AnyscaleLLM)
-        assert llm.model_name == MODEL_NAME
+    def test_openai_llm(self, _: MagicMock) -> None:
+        llm = OpenAILLM(model=self.model_id, api_key="api.key")  # type: ignore
+
+        assert isinstance(llm, OpenAILLM)
+        assert llm.model_name == self.model_id
+
+    def test_openai_llm_env_vars(self, _: MagicMock) -> None:
+        with mock.patch.dict(os.environ, clear=True):
+            os.environ["OPENAI_API_KEY"] = "another.api.key"
+            os.environ["OPENAI_BASE_URL"] = "https://example.com"
+
+            llm = OpenAILLM(model=self.model_id)
+
+            assert isinstance(llm, OpenAILLM)
+            assert llm.model_name == self.model_id
+            assert llm.base_url == "https://example.com"
+            assert llm.api_key.get_secret_value() == "another.api.key"  # type: ignore
+
+    @pytest.mark.asyncio
+    async def test_agenerate(self, mock_openai: MagicMock) -> None:
+        llm = OpenAILLM(model=self.model_id, api_key="api.key")  # type: ignore
+        llm._aclient = mock_openai
 
-    def test_unavailable_model(self, mock_anyscale):
-        with pytest.raises(
-            AssertionError,
-            match=re.escape(
-                f"Provided `model` is not available in your Anyscale account, available models are ['{MODEL_NAME}']"
-            ),
-        ):
-            AnyscaleLLM(
-                model="other_model",
-                task=TextGenerationTask(),
-                api_key="api.key",
-            )
-
-    def test_generate(self, mock_anyscale):
-        llm = AnyscaleLLM(
-            model=MODEL_NAME,
-            task=TextGenerationTask(),
-            api_key="api.key",
+        mocked_completion = Mock(
+            choices=[Mock(message=Mock(content=" Aenean hendrerit aliquam velit. ..."))]
         )
+        llm._aclient.chat.completions.create = AsyncMock(return_value=mocked_completion)
 
-        input = "What is Anyscale?"
-        model_response = "model response"
-        contents = [
-            [
+        await llm.agenerate(
+            input=[
+                {"role": "system", "content": ""},
                 {
-                    "model_name": llm.model_name,
-                    "prompt_used": [
-                        {
-                            "role": "system",
-                            "content": "You are a helpful, respectful and honest assistant. Always answer as helpfully as possible, while being safe. Your answers should not include any harmful, unethical, racist, sexist, toxic, dangerous, or illegal content. Please ensure that your responses are socially unbiased and positive in nature.\nIf a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. If you don't know the answer to a question, please don't share false information.",
-                        },
-                        {"role": "user", "content": input},
-                    ],
-                    "raw_output": model_response,
-                    "parsed_output": {"generations": model_response},
-                }
+                    "role": "user",
+                    "content": "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
+                },
             ]
-        ]
-
-        class MockContent:
-            def __init__(self, content=model_response):
-                self.content = content
+        )
 
-        class MockMessage:
-            def __init__(self, message=MockContent()):
-                self.message = message
+    @pytest.mark.asyncio
+    async def test_generate(self, mock_openai: MagicMock) -> None:
+        llm = OpenAILLM(model=self.model_id, api_key="api.key")  # type: ignore
+        llm._aclient = mock_openai
 
-        choices = [MockMessage()]
+        mocked_completion = Mock(
+            choices=[Mock(message=Mock(content=" Aenean hendrerit aliquam velit. ..."))]
+        )
+        llm._aclient.chat.completions.create = AsyncMock(return_value=mocked_completion)
 
-        class MockCompletions:
-            def __init__(self, choices=choices):
-                self.choices = choices
+        nest_asyncio.apply()
 
-        llm.client.chat.completions.create = mock.MagicMock(
-            return_value=MockCompletions()
+        llm.generate(
+            inputs=[
+                [
+                    {"role": "system", "content": ""},
+                    {
+                        "role": "user",
+                        "content": "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
+                    },
+                ]
+            ]
         )
 
-        result = llm.generate([{"input": input}])
-        assert result == contents
+    def test_serialization(self, _: MagicMock) -> None:
+        llm = OpenAILLM(model=self.model_id)
+
+        _dump = {
+            "model": self.model_id,
+            "generation_kwargs": {},
+            "max_retries": 6,
+            "base_url": "https://api.openai.com/v1",
+            "timeout": 120,
+            "type_info": {
+                "module": "distilabel.llms.openai",
+                "name": "OpenAILLM",
+            },
+        }
+
+        assert llm.dump() == _dump
+        assert isinstance(OpenAILLM.from_dict(_dump), OpenAILLM)
```

### Comparing `distilabel-0.6.0/tests/llm/google/__init__.py` & `distilabel-1.0.0/src/distilabel/utils/card/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/tests/tasks/__init__.py` & `distilabel-1.0.0/src/distilabel/steps/tasks/evol_quality/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/tests/tasks/text_generation/__init__.py` & `distilabel-1.0.0/src/distilabel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/tests/tasks/text_generation/test_evol_tasks.py` & `distilabel-1.0.0/tests/unit/steps/tasks/evol_instruct/test_generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,237 +8,179 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import argilla as rg
 import pytest
-from distilabel.dataset import CustomDataset
-from distilabel.tasks.text_generation.evol_complexity import EvolComplexityTask
-from distilabel.tasks.text_generation.evol_instruct import (
-    EvolInstructTask,
-    _get_stopwords,
-)
-from distilabel.tasks.text_generation.evol_quality import EvolQualityTask
-
-
-def test_get_stopwords():
-    stopwords = _get_stopwords()
-    assert len(stopwords) == 179
-
-
-breadth = """I want you to act as a Prompt Creator.
-Your goal is to draw inspiration from the #Given Prompt# to create a brand new prompt.
-This new prompt should belong to the same domain as the #Given Prompt# but must be even more rare.
-The LENGTH and complexity of the #Created Prompt# should be similar to that of the #Given Prompt#.
-The #Created Prompt# must be reasonable and must be understood and responded by humans.
-'#Given Prompt#', '#Created Prompt#', 'given prompt' and 'created prompt' are not allowed to appear in #Created Prompt#
-#Given Prompt#:
-HELLO
-#Created Prompt#:
-"""
-
-base_evol_instruct = """I want you to act as a Prompt Rewriter.
-Your objective is to rewrite a given prompt into a more complex version to make those famous AI systems (e.g., chatgpt and GPT4) a bit harder to handle.
-But the rewritten prompt must be reasonable and must be understood and responded by humans.
-Your rewriting cannot omit the non-text parts such as the table and code in #The Given Prompt#:. Also, please do not omit the input in #The Given Prompt#.
-You SHOULD complicate the given prompt using the following method:
-"""
-
-end_evol_instruct = """
-You should try your best not to make the #Rewritten Prompt# become verbose, #Rewritten Prompt# can only add 10 to 20 words into #The Given Prompt#.
-'#The Given Prompt#', '#Rewritten Prompt#', 'given prompt' and 'rewritten prompt' are not allowed to appear in #Rewritten Prompt#
-#The Given Prompt#:
-HELLO
-#Rewritten Prompt#:
-"""
-
-constraints = f"{base_evol_instruct}Please add one more constraints/requirements into #The Given Prompt#{end_evol_instruct}"
-deepen = f"{base_evol_instruct}If #The Given Prompt# contains inquiries about certain issues, the depth and breadth of the inquiry can be increased.{end_evol_instruct}"
-concretizing = f"{base_evol_instruct}Please replace general concepts with more specific concepts.{end_evol_instruct}"
-reasoning = f"{base_evol_instruct}If #The Given Prompt# can be solved with just a few simple thinking processes, you can rewrite it to explicitly request multiple-step reasoning.{end_evol_instruct}"
-
-base_evol_quality = """I want you to act as a Response Rewriter
-Your goal is to enhance the quality of the response given by an AI assistant
-to the #Given Prompt# through rewriting.
-But the rewritten response must be reasonable and must be understood by humans.
-Your rewriting cannot omit the non-text parts such as the table and code in
-#Given Prompt# and #Given Response#. Also, please do not omit the input
-in #Given Prompt#.
-You Should enhance the quality of the response using the following method:
-"""
-
-end_evol_quality = """
-You should try your best not to make the #Rewritten Response# become verbose,
-#Rewritten Response# can only add 10 to 20 words into #Given Response#.
-'#Given Response#', '#Rewritten Response#', 'given response' and 'rewritten response'
-are not allowed to appear in #Rewritten Response#
-#Given Prompt#:
-HELLO
-#Given Response#:
-HELLO
-#Rewritten Response#:"""
-
-helpfulness = f"{base_evol_quality}Please make the Response more helpful to the user.{end_evol_quality}"
-relevance = f"{base_evol_quality}Please make the Response more relevant to #Given Prompt#.{end_evol_quality}"
-depth = f"{base_evol_quality}Please make the Response more in-depth.{end_evol_quality}"
-creativity = f"{base_evol_quality}Please increase the creativity of the response.{end_evol_quality}"
-details = f"{base_evol_quality}Please increase the detail level of Response.{end_evol_quality}"
-
-
-@pytest.mark.parametrize(
-    "evolution_method, expected, instruct_type",
-    [
-        ("breadth", breadth, EvolInstructTask),
-        ("constraints", constraints, EvolInstructTask),
-        ("deepen", deepen, EvolInstructTask),
-        ("concretizing", concretizing, EvolInstructTask),
-        ("reasoning", reasoning, EvolInstructTask),
-        ("constraints", constraints, EvolComplexityTask),
-        ("deepen", deepen, EvolComplexityTask),
-        ("concretizing", concretizing, EvolComplexityTask),
-        ("reasoning", reasoning, EvolComplexityTask),
-        ("helpfulness", helpfulness, EvolQualityTask),
-        ("relevance", relevance, EvolQualityTask),
-        ("depth", depth, EvolQualityTask),
-        ("creativity", creativity, EvolQualityTask),
-        ("details", details, EvolQualityTask),
-        ("fake", ValueError, EvolInstructTask),
-        ("fake", ValueError, EvolQualityTask),
-        # # breadth is not a valid evolution method for EvolComplexityTask
-        ("breadth", ValueError, EvolComplexityTask),
-    ],
-)
-def test_evol_task(evolution_method: str, expected: str, instruct_type: object):
-    mock_kwargs = {"input": "HELLO", "generation": "HELLO"}
-    task = instruct_type()
-    assert isinstance(task, instruct_type)
-    assert task.system_prompt == ""
-    if isinstance(expected, str):
-        assert (
-            task.generate_prompt(
-                **mock_kwargs, evolution_method=evolution_method
-            ).formatted_prompt
-            == expected
+from distilabel.llms.base import LLM
+from distilabel.pipeline.local import Pipeline
+from distilabel.steps.tasks.evol_instruct.generator import (
+    EvolInstructGenerator,
+)
+from distilabel.steps.tasks.evol_instruct.utils import (
+    GENERATION_MUTATION_TEMPLATES,
+)
+from pydantic import ValidationError
+
+
+class TestEvolInstructGenerator:
+    def test_passing_pipeline(self, dummy_llm: LLM) -> None:
+        pipeline = Pipeline(name="unit-test-pipeline")
+        task = EvolInstructGenerator(
+            name="task", llm=dummy_llm, num_instructions=2, pipeline=pipeline
         )
-    else:
-        with pytest.raises(expected):
-            task.generate_prompt(**mock_kwargs, evolution_method=evolution_method)
-
-
-@pytest.mark.parametrize(
-    "response, expected",
-    [
-        ("Some common response", "Some common response"),
-        ("This contains #Given Response#, which is a response word", None),
-    ],
-)
-def test_evol_quality_elimination_evolving(response: str, expected: str):
-    task = EvolQualityTask()
-    assert task.parse_output(response)["generations"] == expected
-
+        assert task.name == "task"
+        assert task.llm is dummy_llm
+        assert task.num_instructions == 2
+        assert task.mutation_templates == GENERATION_MUTATION_TEMPLATES
+        assert task.pipeline is pipeline
+
+    def test_within_pipeline_context(self, dummy_llm: LLM) -> None:
+        with Pipeline(name="unit-test-pipeline") as pipeline:
+            task = EvolInstructGenerator(
+                name="task", llm=dummy_llm, num_instructions=2, pipeline=pipeline
+            )
+            assert task.name == "task"
+            assert task.llm is dummy_llm
+        assert task.pipeline == pipeline
+
+    def test_with_errors(self, dummy_llm: LLM) -> None:
+        with pytest.raises(
+            ValidationError, match="num_instructions\n  Field required \\[type=missing"
+        ):
+            EvolInstructGenerator(
+                name="task", pipeline=Pipeline(name="unit-test-pipeline")
+            )  # type: ignore
+
+        with pytest.raises(ValueError, match="Step 'task' hasn't received a pipeline"):
+            EvolInstructGenerator(name="task", llm=dummy_llm, num_instructions=2)
+
+    def test_process(self, dummy_llm: LLM) -> None:
+        pipeline = Pipeline(name="unit-test-pipeline")
+        task = EvolInstructGenerator(
+            name="task",
+            llm=dummy_llm,
+            num_instructions=1,
+            min_length=1,
+            max_length=10,
+            pipeline=pipeline,
+        )
+        task.load()
+        assert list(task.process()) == [
+            (
+                [
+                    {
+                        "instruction": "output",
+                        "model_name": "test",
+                    }
+                ],
+                True,
+            )
+        ]
+
+    def test_process_generate_answers(self, dummy_llm: LLM) -> None:
+        pipeline = Pipeline(name="unit-test-pipeline")
+        task = EvolInstructGenerator(
+            name="task",
+            llm=dummy_llm,
+            num_instructions=1,
+            min_length=1,
+            max_length=10,
+            generate_answers=True,
+            pipeline=pipeline,
+        )
+        task.load()
+        assert list(task.process()) == [
+            (
+                [
+                    {
+                        "instruction": "output",
+                        "answer": "output",
+                        "model_name": "test",
+                    }
+                ],
+                True,
+            )
+        ]
+
+    def test_serialization(self, dummy_llm: LLM) -> None:
+        pipeline = Pipeline(name="unit-test-pipeline")
+        task = EvolInstructGenerator(
+            name="task", llm=dummy_llm, num_instructions=2, pipeline=pipeline
+        )
+        task.load()
 
-def get_custom_evol_dataset(
-    instruction_type: object,
-) -> CustomDataset:
-    ds = CustomDataset.from_dict(
-        {
-            "input": [
-                'Create a sentence using the words "happy," "joyful," and "thrilled."\n',
-                "Construct plumbing diagrams for a two-story house\n",
-            ],
-            "generation_model": [["gpt-3.5-turbo"], ["gpt-3.5-turbo"]],
-            "generation_prompt": [
-                [
-                    [
-                        {"content": "", "role": "system"},
-                        {
-                            "content": "I want you to act as a Prompt Rewriter.\nYour objective is to rewrite a given prompt into a more complex version to make those famous AI systems (e.g., chatgpt and GPT4) a bit harder to handle.\nBut the rewritten prompt must be reasonable and must be understood and responded by humans.\nYour rewriting cannot omit the non-text parts such as the table and code in #The Given Prompt#:. Also, please do not omit the input in #The Given Prompt#.\nYou SHOULD complicate the given prompt using the following method:\nIf #The Given Prompt# can be solved with just a few simple thinking processes, you can rewrite it to explicitly request multiple-step reasoning.\nYou should try your best not to make the #Rewritten Prompt# become verbose, #Rewritten Prompt# can only add 10 to 20 words into #The Given Prompt#.\n'#The Given Prompt#', '#Rewritten Prompt#', 'given prompt' and 'rewritten prompt' are not allowed to appear in #Rewritten Prompt#\n#The Given Prompt#:\nCreate a sentence using the words \"happy,\" \"joyful,\" and \"thrilled.\"\n\n\n#Rewritten Prompt#:\n",
-                            "role": "user",
-                        },
-                    ]
-                ],
-                [
-                    [
-                        {"content": "", "role": "system"},
+        assert task.dump() == {
+            "name": "task",
+            "llm": {
+                "generation_kwargs": {},
+                "type_info": {
+                    "module": task.llm.__class__.__module__,
+                    "name": task.llm.__class__.__name__,
+                },
+            },
+            "input_mappings": task.input_mappings,
+            "output_mappings": task.output_mappings,
+            "batch_size": task.batch_size,
+            "num_instructions": task.num_instructions,
+            "generate_answers": task.generate_answers,
+            "mutation_templates": {
+                "FRESH_START": "Write one question or request containing one or more of the following words: <PROMPT>",
+                "CONSTRAINTS": "I want you act as a Prompt Rewriter.\n\nYour objective is to rewrite a given prompt into a more complex version to make those famous AI systems (e.g., chatgpt and GPT4) a bit harder to handle.\n\nBut the rewritten prompt must be reasonable and must be understood and responded by humans.\n\nYour rewriting cannot omit the non-text parts such as the table and code in #The Given Prompt#:. Also, please do not omit the input in #The Given Prompt#.\n\nYou SHOULD complicate the given prompt using the following method: \nPlease add one more constraints/requirements into '#The Given Prompt#'\n\nYou should try your best not to make the #Rewritten Prompt# become verbose, #Rewritten Prompt# can only add 10 to 20 words into #The Given Prompt#.\n\n'#The Given Prompt#', '#Rewritten Prompt#', 'given prompt' and 'rewritten prompt' are not allowed to appear in #Rewritten Prompt#\n\n#The Given Prompt#:\n<PROMPT>\n#Rewritten Prompt#:\n\n",
+                "DEEPENING": "I want you act as a Prompt Rewriter.\n\nYour objective is to rewrite a given prompt into a more complex version to make those famous AI systems (e.g., chatgpt and GPT4) a bit harder to handle.\n\nBut the rewritten prompt must be reasonable and must be understood and responded by humans.\n\nYour rewriting cannot omit the non-text parts such as the table and code in #The Given Prompt#:. Also, please do not omit the input in #The Given Prompt#.\n\nYou SHOULD complicate the given prompt using the following method: \nIf #The Given Prompt# contains inquiries about certain issues, the depth and breadth of the inquiry can be increased.\n\nYou should try your best not to make the #Rewritten Prompt# become verbose, #Rewritten Prompt# can only add 10 to 20 words into #The Given Prompt#.\n\n'#The Given Prompt#', '#Rewritten Prompt#', 'given prompt' and 'rewritten prompt' are not allowed to appear in #Rewritten Prompt#\n\n#The Given Prompt#:\n<PROMPT>\n#Rewritten Prompt#:\n\n",
+                "CONCRETIZING": "I want you act as a Prompt Rewriter.\n\nYour objective is to rewrite a given prompt into a more complex version to make those famous AI systems (e.g., chatgpt and GPT4) a bit harder to handle.\n\nBut the rewritten prompt must be reasonable and must be understood and responded by humans.\n\nYour rewriting cannot omit the non-text parts such as the table and code in #The Given Prompt#:. Also, please do not omit the input in #The Given Prompt#.\n\nYou SHOULD complicate the given prompt using the following method: \nPlease replace general concepts with more specific concepts.\n\nYou should try your best not to make the #Rewritten Prompt# become verbose, #Rewritten Prompt# can only add 10 to 20 words into #The Given Prompt#.\n\n'#The Given Prompt#', '#Rewritten Prompt#', 'given prompt' and 'rewritten prompt' are not allowed to appear in #Rewritten Prompt#\n\n#The Given Prompt#:\n<PROMPT>\n#Rewritten Prompt#:\n\n",
+                "INCREASED_REASONING_STEPS": "I want you act as a Prompt Rewriter.\n\nYour objective is to rewrite a given prompt into a more complex version to make those famous AI systems (e.g., chatgpt and GPT4) a bit harder to handle.\n\nBut the rewritten prompt must be reasonable and must be understood and responded by humans.\n\nYour rewriting cannot omit the non-text parts such as the table and code in #The Given Prompt#:. Also, please do not omit the input in #The Given Prompt#.\n\nYou SHOULD complicate the given prompt using the following method: \nIf #The Given Prompt# can be solved with just a few simple thinking processes, you can rewrite it to explicitly request multiple-step reasoning.\n\nYou should try your best not to make the #Rewritten Prompt# become verbose, #Rewritten Prompt# can only add 10 to 20 words into #The Given Prompt#.\n\n'#The Given Prompt#', '#Rewritten Prompt#', 'given prompt' and 'rewritten prompt' are not allowed to appear in #Rewritten Prompt#\n\n#The Given Prompt#:\n<PROMPT>\n#Rewritten Prompt#:\n\n",
+                "BREADTH": "I want you act as a Prompt Creator.\n\nYour goal is to draw inspiration from the #Given Prompt# to create a brand new prompt.\n\nThis new prompt should belong to the same domain as the #Given Prompt# but be even more rare.\n\nThe LENGTH and complexity of the #Created Prompt# should be similar to that of the #Given Prompt#.\n\nThe #Created Prompt# must be reasonable and must be understood and responded by humans.\n\n'#Given Prompt#', '#Created Prompt#', 'given prompt' and 'created prompt' are not allowed to appear in #Created Prompt#\n\n#Given Prompt#:\n<PROMPT>\n#Created Prompt#:\n\n",
+            },
+            "num_generations": task.num_generations,
+            "group_generations": task.group_generations,
+            "min_length": task.min_length,
+            "max_length": task.max_length,
+            "seed": task.seed,
+            "runtime_parameters_info": [
+                {
+                    "description": "The number of rows that will contain the batches generated by the step.",
+                    "name": "batch_size",
+                    "optional": True,
+                },
+                {
+                    "name": "llm",
+                    "runtime_parameters_info": [
                         {
-                            "content": "I want you to act as a Prompt Rewriter.\nYour objective is to rewrite a given prompt into a more complex version to make those famous AI systems (e.g., chatgpt and GPT4) a bit harder to handle.\nBut the rewritten prompt must be reasonable and must be understood and responded by humans.\nYour rewriting cannot omit the non-text parts such as the table and code in #The Given Prompt#:. Also, please do not omit the input in #The Given Prompt#.\nYou SHOULD complicate the given prompt using the following method:\nIf #The Given Prompt# contains inquiries about certain issues, the depth and breadth of the inquiry can be increased.\nYou should try your best not to make the #Rewritten Prompt# become verbose, #Rewritten Prompt# can only add 10 to 20 words into #The Given Prompt#.\n'#The Given Prompt#', '#Rewritten Prompt#', 'given prompt' and 'rewritten prompt' are not allowed to appear in #Rewritten Prompt#\n#The Given Prompt#:\nConstruct plumbing diagrams for a two-story house\n\n\n#Rewritten Prompt#:\n",
-                            "role": "user",
+                            "description": "The kwargs to be propagated to either `generate` or `agenerate` methods within each `LLM`.",
+                            "keys": [],
+                            "name": "generation_kwargs",
                         },
-                    ]
-                ],
-            ],
-            "raw_generation_responses": [
-                [
-                    'Compose a concise and articulate sentence that incorporates the terms "ecstatic," "exhilarated," "blissful," and "overjoyed."'
-                ],
-                [
-                    "Design comprehensive and detailed plumbing diagrams for a two-story house that include separate diagrams for each floor, showcasing the layout, dimensions, and connections of all plumbing fixtures, pipelines, drains, vents, water supply sources, and sewage disposal systems. These diagrams should consider the specific requirements and codes of local building regulations while providing a clear and accurate representation of the plumbing infrastructure throughout the entire house."
-                ],
-            ],
-            "instructions": [
-                [
-                    'Compose a concise and articulate sentence that incorporates the terms "ecstatic," "exhilarated," "blissful," and "overjoyed."'
-                ],
-                [
-                    "Design comprehensive and detailed plumbing diagrams for a two-story house that include separate diagrams for each floor, showcasing the layout, dimensions, and connections of all plumbing fixtures, pipelines, drains, vents, water supply sources, and sewage disposal systems. These diagrams should consider the specific requirements and codes of local building regulations while providing a clear and accurate representation of the plumbing infrastructure throughout the entire house."
-                ],
+                    ],
+                },
+                {
+                    "name": "num_generations",
+                    "optional": True,
+                    "description": "The number of generations to be produced per input.",
+                },
+                {
+                    "name": "min_length",
+                    "optional": True,
+                    "description": "Defines the length (in bytes) that the generated instruction needs to be higher than, to be considered valid.",
+                },
+                {
+                    "name": "max_length",
+                    "optional": True,
+                    "description": "Defines the length (in bytes) that the generated instruction needs to be lower than, to be considered valid.",
+                },
+                {
+                    "name": "seed",
+                    "optional": True,
+                    "description": "As `numpy` is being used in order to randomly pick a mutation method, then is nice to seed a random seed.",
+                },
             ],
+            "type_info": {
+                "module": EvolInstructGenerator.__module__,
+                "name": EvolInstructGenerator.__name__,
+            },
         }
-    )
-    ds.task = instruction_type()
-    return ds
 
-
-@pytest.mark.parametrize(
-    "instruction_type",
-    [
-        EvolInstructTask,
-        EvolComplexityTask,
-    ],
-)
-def test_evol_task_to_argilla_dataset(
-    instruction_type,
-):
-    ds = get_custom_evol_dataset(instruction_type)
-    ds_row = ds[0]
-    task = ds.task
-    rg_dataset = task.to_argilla_dataset(ds_row)
-    assert isinstance(rg_dataset, rg.FeedbackDataset)
-    assert len(rg_dataset.records) == 0
-
-
-@pytest.mark.parametrize(
-    "instruction_type",
-    [
-        EvolInstructTask,
-        EvolComplexityTask,
-    ],
-)
-def test_evol_task_to_argilla_record(
-    instruction_type,
-):
-    ds: CustomDataset = get_custom_evol_dataset(instruction_type)
-    ds_row = ds[0]
-    task = ds.task
-    records = task.to_argilla_record(ds_row)
-    assert isinstance(records, list)
-    assert len(records) == 1
-    assert isinstance(records[0], rg.FeedbackRecord)
-
-
-@pytest.mark.parametrize(
-    "instruction_type",
-    [
-        EvolInstructTask,
-        EvolComplexityTask,
-    ],
-)
-def test_evol_task_to_argilla(
-    instruction_type,
-):
-    ds = get_custom_evol_dataset(instruction_type)
-    rg_dataset = ds.to_argilla(vector_strategy=False, metric_strategy=False)
-    assert isinstance(rg_dataset, rg.FeedbackDataset)
-    assert len(rg_dataset.records) == 2
+        with Pipeline(name="unit-test-pipeline") as pipeline:
+            new_task = EvolInstructGenerator.from_dict(task.dump())
+            assert isinstance(new_task, EvolInstructGenerator)
```

### Comparing `distilabel-0.6.0/.gitignore` & `distilabel-1.0.0/.gitignore`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -73,8 +73,8 @@
 
 # mkdocs documentation
 /site
 
 # Other
 *.log
 *.swp
-.DS_Store
+.DS_Store
```

### Comparing `distilabel-0.6.0/LICENSE_HEADER` & `distilabel-1.0.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `distilabel-0.6.0/pyproject.toml` & `distilabel-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,73 +4,85 @@
 
 [project]
 name = "distilabel"
 description = "AI Feedback (AIF) framework"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
-keywords = ["llm", "annotation", "alignment"]
+keywords = ["llm", "annotation", "alignment", "synthetic", "data", "rlaif"]
 authors = [{ name = "Argilla", email = "admin@argilla.io" }]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "datasets >= 2.14.0",
+    "httpx >= 0.25.2",
+    "importlib-resources >= 6.1.1; python_version < '3.9'",
     "Jinja2 >= 3.1.2",
+    "multiprocess >= 0.70",
+    "nest-asyncio >= 1.6.0",
+    "networkx >= 3.0",
+    "pydantic >= 2.0",
     "rich >= 13.5.0",
-    "tenacity >= 8",
-    "importlib-resources >= 6.1.1; python_version < '3.9'",
-    "multiprocess",
+    "scipy >= 1.10.0",
+    "typer >= 0.9.0",
+    "tblib >= 3.0.0",
 ]
 dynamic = ["version"]
 
+[project.scripts]
+distilabel = "distilabel.cli.app:app"
+
 [project.optional-dependencies]
-dev = ["black == 23.10.0", "ruff == 0.1.0", "pre-commit >= 3.5.0"]
-hf-transformers = ["transformers >= 4.34.1", "torch >= 2.0.0"]
-hf-inference-endpoints = ["huggingface_hub >= 0.19.0"]
-llama-cpp = ["llama-cpp-python >= 0.2.0"]
-ollama = ["ollama >= 0.1.4"]
-openai = ["openai >= 1.0.0"]
-vllm = ["vllm >= 0.2.1"]
-vertexai = ["google-cloud-aiplatform >= 1.38.0"]
-together = ["together"]
-argilla = ["argilla >= 1.23.0", "sentence-transformers >= 2.0.0", "textdescriptives >= 2.0.0"]
-tests = ["pytest >= 7.4.0"]
-mistralai = ["mistralai >= 0.0.11"]
+dev = ["ruff == 0.2.2", "pre-commit >= 3.5.0"]
 docs = [
     "mkdocs-material >= 9.5.0",
     "mkdocstrings[python] >= 0.24.0",
     "mkdocs-literate-nav >= 0.6.1",
     "mkdocs-section-index >= 0.3.8",
     "mkdocs-gen-files >= 0.5.0",
     "mike >= 2.0.0",
     "Pillow >= 9.5.0",
     "CairoSVG >= 2.7.1",
     "mknotebooks >= 0.8.0",
 ]
+tests = ["pytest >= 7.4.0", "pytest-asyncio", "nest-asyncio"]
+
+# Optional LLMs, integrations, etc
+anthropic = ["anthropic >= 0.20.0"]
+argilla = ["argilla >= 1.23.0"]
+cohere = ["cohere >= 5.2.0"]
+hf-inference-endpoints = ["huggingface_hub >= 0.19.0"]
+hf-transformers = ["transformers >= 4.34.1", "torch >= 2.0.0"]
+litellm = ["litellm >= 1.30.0"]
+llama-cpp = ["llama-cpp-python >= 0.2.0"]
+mistralai = ["mistralai >= 0.1.0"]
+ollama = ["ollama >= 0.1.7"]
+openai = ["openai >= 1.0.0"]
+vertexai = ["google-cloud-aiplatform >= 1.38.0"]
+vllm = ["vllm >= 0.2.1", "filelock >= 3.13.4"]
 
 [project.urls]
 Documentation = "https://distilabel.argilla.io/"
 Issues = "https://github.com/argilla/distilabel/issues"
 Source = "https://github.com/argilla/distilabel"
 
 [tool.hatch.version]
 path = "src/distilabel/__init__.py"
 
 [tool.ruff]
 line-length = 88
-select = ["E", "W", "F", "I", "C", "B"]
-ignore = ["E501", "B905", "B008"]
 exclude = ["docs"]
 
-[tool.ruff.lint.mccabe]
-max-complexity = 14
+[tool.ruff.lint]
+select = ["E", "W", "F", "I", "C", "B"]
+ignore = ["E501", "B905", "B008"]
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
```

