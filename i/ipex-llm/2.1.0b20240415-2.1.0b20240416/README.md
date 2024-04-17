# Comparing `tmp/ipex_llm-2.1.0b20240415-py3-none-win_amd64.whl.zip` & `tmp/ipex_llm-2.1.0b20240416-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5233908 bytes, number of entries: 210
+Zip file size: 5238372 bytes, number of entries: 211
 -rw-------  2.0 unx     1898 b- defN 24-Mar-25 11:36 ipex_llm/__init__.py
 -rw-------  2.0 unx     6816 b- defN 24-Mar-25 11:36 ipex_llm/convert_model.py
 -rw-------  2.0 unx     2914 b- defN 24-Mar-25 11:36 ipex_llm/llm_patching.py
 -rw-------  2.0 unx     1177 b- defN 24-Mar-25 11:36 ipex_llm/models.py
 -rw-------  2.0 unx    12332 b- defN 24-Apr-15 15:07 ipex_llm/optimize.py
 -rw-------  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-chat.ps1
 -rwx------  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm/cli/llm-cli.ps1
@@ -38,69 +38,70 @@
 -rw-------  2.0 unx     1189 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/__init__.py
 -rw-------  2.0 unx    13589 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/bigdlllm.py
 -rw-------  2.0 unx     7225 b- defN 24-Mar-25 11:36 ipex_llm/langchain/embeddings/transformersembeddings.py
 -rw-------  2.0 unx     1636 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/__init__.py
 -rw-------  2.0 unx    24438 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/bigdlllm.py
 -rw-------  2.0 unx    10576 b- defN 24-Apr-03 15:07 ipex_llm/langchain/llms/transformersllm.py
 -rw-------  2.0 unx     7379 b- defN 24-Mar-25 11:36 ipex_llm/langchain/llms/transformerspipelinellm.py
--rw-------  2.0 unx        0 b- defN 24-Apr-15 15:08 ipex_llm/libs/__init__.py
--rw-------  2.0 unx    36352 b- defN 24-Apr-15 15:08 ipex_llm/libs/bloom-api.dll
--rw-------  2.0 unx   440320 b- defN 24-Apr-15 15:08 ipex_llm/libs/bloom.dll
--rw-------  2.0 unx   852992 b- defN 24-Apr-15 15:08 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
--rw-------  2.0 unx   856064 b- defN 24-Apr-15 15:08 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
--rw-------  2.0 unx   843776 b- defN 24-Apr-15 15:08 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
--rw-------  2.0 unx    24576 b- defN 24-Apr-15 15:08 ipex_llm/libs/gptneox-api.dll
--rw-------  2.0 unx   500224 b- defN 24-Apr-15 15:08 ipex_llm/libs/gptneox.dll
--rw-------  2.0 unx   464384 b- defN 24-Apr-15 15:08 ipex_llm/libs/libbloom_avx.dll
--rw-------  2.0 unx   441344 b- defN 24-Apr-15 15:08 ipex_llm/libs/libbloom_vnni.dll
--rw-------  2.0 unx   524800 b- defN 24-Apr-15 15:08 ipex_llm/libs/libgptneox_avx.dll
--rw-------  2.0 unx   501248 b- defN 24-Apr-15 15:08 ipex_llm/libs/libgptneox_vnni.dll
--rw-------  2.0 unx   519168 b- defN 24-Apr-15 15:08 ipex_llm/libs/libllama_avx.dll
--rw-------  2.0 unx   495104 b- defN 24-Apr-15 15:08 ipex_llm/libs/libllama_vnni.dll
--rw-------  2.0 unx   555520 b- defN 24-Apr-15 15:08 ipex_llm/libs/libstarcoder_avx.dll
--rw-------  2.0 unx   531968 b- defN 24-Apr-15 15:08 ipex_llm/libs/libstarcoder_vnni.dll
--rw-------  2.0 unx    25088 b- defN 24-Apr-15 15:08 ipex_llm/libs/llama-api.dll
--rw-------  2.0 unx   494080 b- defN 24-Apr-15 15:08 ipex_llm/libs/llama.dll
--rw-------  2.0 unx   103424 b- defN 24-Apr-15 15:08 ipex_llm/libs/main-bloom.exe
--rw-------  2.0 unx   726016 b- defN 24-Apr-15 15:08 ipex_llm/libs/main-chatglm_vnni.exe
--rw-------  2.0 unx    98816 b- defN 24-Apr-15 15:08 ipex_llm/libs/main-gptneox.exe
--rw-------  2.0 unx    99840 b- defN 24-Apr-15 15:08 ipex_llm/libs/main-llama.exe
--rw-------  2.0 unx   157696 b- defN 24-Apr-15 15:08 ipex_llm/libs/main-starcoder.exe
--rw-------  2.0 unx   125952 b- defN 24-Apr-15 15:08 ipex_llm/libs/quantize-bloom.exe
--rw-------  2.0 unx   126976 b- defN 24-Apr-15 15:08 ipex_llm/libs/quantize-bloom_vnni.exe
--rw-------  2.0 unx   103936 b- defN 24-Apr-15 15:08 ipex_llm/libs/quantize-gptneox.exe
--rw-------  2.0 unx   104448 b- defN 24-Apr-15 15:08 ipex_llm/libs/quantize-gptneox_vnni.exe
--rw-------  2.0 unx   108544 b- defN 24-Apr-15 15:08 ipex_llm/libs/quantize-llama.exe
--rw-------  2.0 unx   109568 b- defN 24-Apr-15 15:08 ipex_llm/libs/quantize-llama_vnni.exe
--rw-------  2.0 unx   126976 b- defN 24-Apr-15 15:08 ipex_llm/libs/quantize-starcoder.exe
--rw-------  2.0 unx   128000 b- defN 24-Apr-15 15:08 ipex_llm/libs/quantize-starcoder_vnni.exe
--rw-------  2.0 unx    21504 b- defN 24-Apr-15 15:08 ipex_llm/libs/starcoder-api.dll
--rw-------  2.0 unx   531456 b- defN 24-Apr-15 15:08 ipex_llm/libs/starcoder.dll
+-rw-------  2.0 unx        0 b- defN 24-Apr-16 15:09 ipex_llm/libs/__init__.py
+-rw-------  2.0 unx    36352 b- defN 24-Apr-16 15:09 ipex_llm/libs/bloom-api.dll
+-rw-------  2.0 unx   440320 b- defN 24-Apr-16 15:09 ipex_llm/libs/bloom.dll
+-rw-------  2.0 unx   852992 b- defN 24-Apr-16 15:09 ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd
+-rw-------  2.0 unx   856064 b- defN 24-Apr-16 15:09 ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd
+-rw-------  2.0 unx   843776 b- defN 24-Apr-16 15:09 ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd
+-rw-------  2.0 unx    24576 b- defN 24-Apr-16 15:09 ipex_llm/libs/gptneox-api.dll
+-rw-------  2.0 unx   500224 b- defN 24-Apr-16 15:09 ipex_llm/libs/gptneox.dll
+-rw-------  2.0 unx   464384 b- defN 24-Apr-16 15:09 ipex_llm/libs/libbloom_avx.dll
+-rw-------  2.0 unx   441344 b- defN 24-Apr-16 15:09 ipex_llm/libs/libbloom_vnni.dll
+-rw-------  2.0 unx   524800 b- defN 24-Apr-16 15:09 ipex_llm/libs/libgptneox_avx.dll
+-rw-------  2.0 unx   501248 b- defN 24-Apr-16 15:09 ipex_llm/libs/libgptneox_vnni.dll
+-rw-------  2.0 unx   519168 b- defN 24-Apr-16 15:09 ipex_llm/libs/libllama_avx.dll
+-rw-------  2.0 unx   495104 b- defN 24-Apr-16 15:09 ipex_llm/libs/libllama_vnni.dll
+-rw-------  2.0 unx   555520 b- defN 24-Apr-16 15:09 ipex_llm/libs/libstarcoder_avx.dll
+-rw-------  2.0 unx   531968 b- defN 24-Apr-16 15:09 ipex_llm/libs/libstarcoder_vnni.dll
+-rw-------  2.0 unx    25088 b- defN 24-Apr-16 15:09 ipex_llm/libs/llama-api.dll
+-rw-------  2.0 unx   494080 b- defN 24-Apr-16 15:09 ipex_llm/libs/llama.dll
+-rw-------  2.0 unx   103424 b- defN 24-Apr-16 15:09 ipex_llm/libs/main-bloom.exe
+-rw-------  2.0 unx   726016 b- defN 24-Apr-16 15:09 ipex_llm/libs/main-chatglm_vnni.exe
+-rw-------  2.0 unx    98816 b- defN 24-Apr-16 15:09 ipex_llm/libs/main-gptneox.exe
+-rw-------  2.0 unx    99840 b- defN 24-Apr-16 15:09 ipex_llm/libs/main-llama.exe
+-rw-------  2.0 unx   157696 b- defN 24-Apr-16 15:09 ipex_llm/libs/main-starcoder.exe
+-rw-------  2.0 unx   125952 b- defN 24-Apr-16 15:09 ipex_llm/libs/quantize-bloom.exe
+-rw-------  2.0 unx   126976 b- defN 24-Apr-16 15:09 ipex_llm/libs/quantize-bloom_vnni.exe
+-rw-------  2.0 unx   103936 b- defN 24-Apr-16 15:09 ipex_llm/libs/quantize-gptneox.exe
+-rw-------  2.0 unx   104448 b- defN 24-Apr-16 15:09 ipex_llm/libs/quantize-gptneox_vnni.exe
+-rw-------  2.0 unx   108544 b- defN 24-Apr-16 15:09 ipex_llm/libs/quantize-llama.exe
+-rw-------  2.0 unx   109568 b- defN 24-Apr-16 15:09 ipex_llm/libs/quantize-llama_vnni.exe
+-rw-------  2.0 unx   126976 b- defN 24-Apr-16 15:09 ipex_llm/libs/quantize-starcoder.exe
+-rw-------  2.0 unx   128000 b- defN 24-Apr-16 15:09 ipex_llm/libs/quantize-starcoder_vnni.exe
+-rw-------  2.0 unx    21504 b- defN 24-Apr-16 15:09 ipex_llm/libs/starcoder-api.dll
+-rw-------  2.0 unx   531456 b- defN 24-Apr-16 15:09 ipex_llm/libs/starcoder.dll
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/llamaindex/__init__.py
 -rw-------  2.0 unx     1139 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/__init__.py
 -rw-------  2.0 unx    26314 b- defN 24-Apr-07 15:05 ipex_llm/llamaindex/llms/bigdlllm.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/__init__.py
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/__init__.py
 -rw-------  2.0 unx    10084 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/bigdl_llm_model.py
 -rw-------  2.0 unx    11371 b- defN 24-Mar-27 11:49 ipex_llm/serving/fastchat/ipex_llm_worker.py
 -rw-------  2.0 unx    16649 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/model_worker.py
 -rw-------  2.0 unx     8692 b- defN 24-Mar-25 11:36 ipex_llm/serving/fastchat/vllm_worker.py
 -rw-------  2.0 unx     1005 b- defN 24-Mar-25 11:36 ipex_llm/transformers/__init__.py
 -rw-------  2.0 unx     1213 b- defN 24-Mar-25 11:36 ipex_llm/transformers/bmm.py
--rw-------  2.0 unx    67035 b- defN 24-Apr-11 02:22 ipex_llm/transformers/convert.py
+-rw-------  2.0 unx    67086 b- defN 24-Apr-16 15:08 ipex_llm/transformers/convert.py
 -rw-------  2.0 unx    14274 b- defN 24-Apr-07 15:05 ipex_llm/transformers/convert_ipex.py
 -rw-------  2.0 unx     4613 b- defN 24-Mar-25 11:36 ipex_llm/transformers/embedding.py
 -rw-------  2.0 unx     4533 b- defN 24-Apr-03 15:07 ipex_llm/transformers/kv.py
 -rw-------  2.0 unx     5429 b- defN 24-Mar-25 11:36 ipex_llm/transformers/loader.py
+-rw-------  2.0 unx    13535 b- defN 24-Apr-16 15:08 ipex_llm/transformers/lookup.py
 -rw-------  2.0 unx    38310 b- defN 24-Apr-11 15:08 ipex_llm/transformers/low_bit_linear.py
--rw-------  2.0 unx    35408 b- defN 24-Apr-09 15:06 ipex_llm/transformers/model.py
+-rw-------  2.0 unx    35750 b- defN 24-Apr-16 15:08 ipex_llm/transformers/model.py
 -rw-------  2.0 unx     6921 b- defN 24-Mar-25 11:36 ipex_llm/transformers/modelling_bigdl.py
 -rw-------  2.0 unx    14770 b- defN 24-Mar-25 11:36 ipex_llm/transformers/qlora.py
 -rw-------  2.0 unx    16567 b- defN 24-Mar-25 11:36 ipex_llm/transformers/relora.py
--rw-------  2.0 unx    53041 b- defN 24-Apr-07 15:05 ipex_llm/transformers/speculative.py
+-rw-------  2.0 unx    54368 b- defN 24-Apr-16 15:08 ipex_llm/transformers/speculative.py
 -rw-------  2.0 unx     8404 b- defN 24-Mar-25 11:36 ipex_llm/transformers/training_patch.py
 -rw-------  2.0 unx    13781 b- defN 24-Apr-01 11:38 ipex_llm/transformers/utils.py
 -rw-------  2.0 unx     7611 b- defN 24-Mar-25 11:36 ipex_llm/transformers/xpu_customize_fwd.py
 -rw-------  2.0 unx      875 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/__init__.py
 -rw-------  2.0 unx     2172 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/act.py
 -rw-------  2.0 unx     8861 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/awq.py
 -rw-------  2.0 unx     4422 b- defN 24-Mar-25 11:36 ipex_llm/transformers/awq/awq_config.py
@@ -125,43 +126,43 @@
 -rw-------  2.0 unx     4060 b- defN 24-Mar-25 11:36 ipex_llm/transformers/gguf/models/model_implement/falcon/tokenizer.json
 -rw-------  2.0 unx     7311 b- defN 24-Mar-25 11:36 ipex_llm/transformers/gguf/models/model_implement/mpt/tokenizer.json
 -rw-------  2.0 unx      586 b- defN 24-Mar-25 11:36 ipex_llm/transformers/gguf/models/model_implement/yuan2/__init__.py
 -rw-------  2.0 unx     2192 b- defN 24-Mar-25 11:36 ipex_llm/transformers/gguf/models/model_implement/yuan2/configuration_yuan.py
 -rw-------  2.0 unx    51084 b- defN 24-Mar-25 11:36 ipex_llm/transformers/gguf/models/model_implement/yuan2/yuan_hf_model.py
 -rw-------  2.0 unx     2658 b- defN 24-Mar-25 11:36 ipex_llm/transformers/layers/rope_embedding.py
 -rw-------  2.0 unx      584 b- defN 24-Mar-25 11:36 ipex_llm/transformers/models/__init__.py
--rw-------  2.0 unx     7410 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/aquila.py
--rw-------  2.0 unx    24483 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/baichuan.py
--rw-------  2.0 unx    27209 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/baichuan2.py
+-rw-------  2.0 unx     7415 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/aquila.py
+-rw-------  2.0 unx    24488 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/baichuan.py
+-rw-------  2.0 unx    27214 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/baichuan2.py
 -rw-------  2.0 unx     6085 b- defN 24-Mar-25 11:36 ipex_llm/transformers/models/bert.py
--rw-------  2.0 unx     8966 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/bloom.py
--rw-------  2.0 unx    13738 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/chatglm.py
--rw-------  2.0 unx    32035 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/chatglm2.py
--rw-------  2.0 unx     8692 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/chatglm2_32k.py
--rw-------  2.0 unx     8649 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/decilm.py
--rw-------  2.0 unx    33544 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/falcon.py
--rw-------  2.0 unx    12589 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/gemma.py
+-rw-------  2.0 unx     8971 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/bloom.py
+-rw-------  2.0 unx    13743 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/chatglm.py
+-rw-------  2.0 unx    32040 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/chatglm2.py
+-rw-------  2.0 unx     8697 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/chatglm2_32k.py
+-rw-------  2.0 unx     8654 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/decilm.py
+-rw-------  2.0 unx    33549 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/falcon.py
+-rw-------  2.0 unx    12594 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/gemma.py
 -rw-------  2.0 unx     4342 b- defN 24-Mar-25 11:36 ipex_llm/transformers/models/gptbigcode.py
--rw-------  2.0 unx    17968 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/gptj.py
--rw-------  2.0 unx     6214 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/gptneox.py
--rw-------  2.0 unx    11642 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/internlm.py
--rw-------  2.0 unx    96035 b- defN 24-Apr-12 15:07 ipex_llm/transformers/models/llama.py
--rw-------  2.0 unx    45326 b- defN 24-Apr-12 15:07 ipex_llm/transformers/models/mistral.py
--rw-------  2.0 unx    27293 b- defN 24-Apr-12 15:07 ipex_llm/transformers/models/mixtral.py
--rw-------  2.0 unx     9535 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/mpt.py
--rw-------  2.0 unx     6287 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/phixtral.py
--rw-------  2.0 unx    32330 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/qwen.py
--rw-------  2.0 unx    32600 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/qwen2.py
--rw-------  2.0 unx    11813 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/qwen_vl.py
+-rw-------  2.0 unx    17973 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/gptj.py
+-rw-------  2.0 unx     6219 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/gptneox.py
+-rw-------  2.0 unx    11647 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/internlm.py
+-rw-------  2.0 unx    96040 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/llama.py
+-rw-------  2.0 unx    45331 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/mistral.py
+-rw-------  2.0 unx    27298 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/mixtral.py
+-rw-------  2.0 unx     9540 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/mpt.py
+-rw-------  2.0 unx     6292 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/phixtral.py
+-rw-------  2.0 unx    32335 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/qwen.py
+-rw-------  2.0 unx    32605 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/qwen2.py
+-rw-------  2.0 unx    11818 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/qwen_vl.py
 -rw-------  2.0 unx     6135 b- defN 24-Mar-29 11:38 ipex_llm/transformers/models/rwkv4.py
 -rw-------  2.0 unx    10722 b- defN 24-Apr-09 15:06 ipex_llm/transformers/models/rwkv5.py
--rw-------  2.0 unx    21120 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/stablelm.py
+-rw-------  2.0 unx    21125 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/stablelm.py
 -rw-------  2.0 unx     8822 b- defN 24-Apr-03 15:07 ipex_llm/transformers/models/starcoder2.py
 -rw-------  2.0 unx    17660 b- defN 24-Apr-09 15:06 ipex_llm/transformers/models/utils.py
--rw-------  2.0 unx    20630 b- defN 24-Apr-11 02:22 ipex_llm/transformers/models/yuan.py
+-rw-------  2.0 unx    20635 b- defN 24-Apr-16 15:08 ipex_llm/transformers/models/yuan.py
 -rw-------  2.0 unx      874 b- defN 24-Mar-25 11:36 ipex_llm/utils/__init__.py
 -rw-------  2.0 unx    18074 b- defN 24-Mar-25 11:36 ipex_llm/utils/convert_chatglm.py
 -rw-------  2.0 unx    72612 b- defN 24-Mar-25 11:36 ipex_llm/utils/convert_util.py
 -rw-------  2.0 unx     2093 b- defN 24-Mar-25 11:36 ipex_llm/utils/glibc_checker.py
 -rw-------  2.0 unx     2477 b- defN 24-Mar-25 11:36 ipex_llm/utils/ipex_importer.py
 -rw-------  2.0 unx     2259 b- defN 24-Mar-25 11:36 ipex_llm/utils/isa_checker.py
 -rw-------  2.0 unx     7129 b- defN 24-Mar-25 11:36 ipex_llm/utils/lazy_load_torch.py
@@ -198,15 +199,15 @@
 -rw-------  2.0 unx    11428 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/models/bigdl_llama.py
 -rw-------  2.0 unx     8770 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/models/bigdl_mistral.py
 -rw-------  2.0 unx     8675 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/models/bigdl_mixtral.py
 -rw-------  2.0 unx     7699 b- defN 24-Mar-25 11:36 ipex_llm/vllm/model_executor/models/bigdl_model.py
 -rw-------  2.0 unx      584 b- defN 24-Mar-25 11:36 ipex_llm/vllm/transformers_utils/__init__.py
 -rw-------  2.0 unx     8707 b- defN 24-Mar-25 11:36 ipex_llm/vllm/transformers_utils/tokenizer.py
 -rw-------  2.0 unx    13950 b- defN 24-Mar-25 11:36 ipex_llm/vllm/worker/worker.py
--rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240415.data/scripts/llm-chat.ps1
--rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240415.data/scripts/llm-cli.ps1
--rw-------  2.0 unx     4400 b- defN 24-Apr-15 15:08 ipex_llm-2.1.0b20240415.dist-info/METADATA
--rw-------  2.0 unx       98 b- defN 24-Apr-15 15:08 ipex_llm-2.1.0b20240415.dist-info/WHEEL
--rw-------  2.0 unx       61 b- defN 24-Apr-15 15:08 ipex_llm-2.1.0b20240415.dist-info/entry_points.txt
--rw-------  2.0 unx        9 b- defN 24-Apr-15 15:08 ipex_llm-2.1.0b20240415.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    19997 b- defN 24-Apr-15 15:08 ipex_llm-2.1.0b20240415.dist-info/RECORD
-210 files, 12759793 bytes uncompressed, 5201928 bytes compressed:  59.2%
+-rwxr-xr-x  2.0 unx     2769 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240416.data/scripts/llm-chat.ps1
+-rwxr-xr-x  2.0 unx     3009 b- defN 24-Mar-25 11:36 ipex_llm-2.1.0b20240416.data/scripts/llm-cli.ps1
+-rw-------  2.0 unx     4400 b- defN 24-Apr-16 15:09 ipex_llm-2.1.0b20240416.dist-info/METADATA
+-rw-------  2.0 unx       98 b- defN 24-Apr-16 15:09 ipex_llm-2.1.0b20240416.dist-info/WHEEL
+-rw-------  2.0 unx       61 b- defN 24-Apr-16 15:09 ipex_llm-2.1.0b20240416.dist-info/entry_points.txt
+-rw-------  2.0 unx        9 b- defN 24-Apr-16 15:09 ipex_llm-2.1.0b20240416.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    20086 b- defN 24-Apr-16 15:09 ipex_llm-2.1.0b20240416.dist-info/RECORD
+211 files, 12775252 bytes uncompressed, 5206254 bytes compressed:  59.2%
```

## zipnote {}

```diff
@@ -270,14 +270,17 @@
 
 Filename: ipex_llm/transformers/kv.py
 Comment: 
 
 Filename: ipex_llm/transformers/loader.py
 Comment: 
 
+Filename: ipex_llm/transformers/lookup.py
+Comment: 
+
 Filename: ipex_llm/transformers/low_bit_linear.py
 Comment: 
 
 Filename: ipex_llm/transformers/model.py
 Comment: 
 
 Filename: ipex_llm/transformers/modelling_bigdl.py
@@ -603,29 +606,29 @@
 
 Filename: ipex_llm/vllm/transformers_utils/tokenizer.py
 Comment: 
 
 Filename: ipex_llm/vllm/worker/worker.py
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240415.data/scripts/llm-chat.ps1
+Filename: ipex_llm-2.1.0b20240416.data/scripts/llm-chat.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240415.data/scripts/llm-cli.ps1
+Filename: ipex_llm-2.1.0b20240416.data/scripts/llm-cli.ps1
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240415.dist-info/METADATA
+Filename: ipex_llm-2.1.0b20240416.dist-info/METADATA
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240415.dist-info/WHEEL
+Filename: ipex_llm-2.1.0b20240416.dist-info/WHEEL
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240415.dist-info/entry_points.txt
+Filename: ipex_llm-2.1.0b20240416.dist-info/entry_points.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240415.dist-info/top_level.txt
+Filename: ipex_llm-2.1.0b20240416.dist-info/top_level.txt
 Comment: 
 
-Filename: ipex_llm-2.1.0b20240415.dist-info/RECORD
+Filename: ipex_llm-2.1.0b20240416.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipex_llm/libs/bloom-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800036cc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 15 15:02:51 2024
+Time/Date		Tue Apr 16 15:07:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000003200
 SizeOfInitializedData	0000000000005e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000036cc
@@ -6375,17 +6375,19 @@
    180005621:	push   %rdx
    180005622:	add    %al,0x1(%rax)
    180005628:	pop    %rax
    180005629:	push   %rdx
    18000562a:	add    %al,0x1(%rax)
    180005630:	add    %al,(%rax)
    180005632:	add    %al,(%rax)
-   180005634:	fwait
-   180005635:	rex.B sbb $0x66,%eax
-   18000563b:	add    %cl,-0x20000000(%rip)        # 0x160005641
+   180005634:	rex.R xchg %eax,%esp
+   180005636:	(bad)
+   180005637:	data16 add %al,(%rax)
+   18000563a:	add    %al,(%rax)
+   18000563c:	or     $0xe0000000,%eax
    180005641:	add    (%rax),%al
    180005643:	add    %cl,(%rcx,%rbx,2)
    180005646:	add    %al,(%rax)
    180005648:	or     $0x3f,%al
 	...
    18000567e:	add    %al,(%rax)
    180005680:	add    %eax,(%rax)
```

## ipex_llm/libs/bloom.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018004e578
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 15 15:02:52 2024
+Time/Date		Tue Apr 16 15:07:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000004ea00
 SizeOfInitializedData	00000000000bea00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000004e578
@@ -104626,15 +104626,16 @@
    18005771a:	add    $0x180,%eax
    18005771f:	add    %dh,0x6(%rax)
    180057722:	add    $0x180,%eax
    180057727:	add    %bh,0x6(%rax)
    18005772a:	add    $0x180,%eax
    18005772f:	add    %al,(%rax)
    180057731:	add    %al,(%rax)
-   180057733:	add    %bl,0x661d(%rcx,%rax,2)
+   180057733:	add    %al,0x1e(%rsp,%rdx,4)
+   180057737:	data16 add %al,(%rax)
    18005773a:	add    %al,(%rax)
    18005773c:	or     $0x50000000,%eax
    180057741:	add    (%rax),%eax
    180057743:	add    %ah,(%rax)
    180057745:	addl   $0x0,0x56f2000(%rip)        # 0x18574974f
 	...
    18005777f:	add    %dl,0x1800584(%rax)
```

## ipex_llm/libs/gptneox-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002cbc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 15 15:02:51 2024
+Time/Date		Tue Apr 16 15:07:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002600
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002cbc
@@ -5058,17 +5058,19 @@
    1800049c0:	cmp    %al,0x0(%rdx)
    1800049c3:	addb   $0x0,(%rcx)
    1800049c6:	add    %al,(%rax)
    1800049c8:	rex
    1800049c9:	rex.X add %al,0x1(%rax)
    1800049d0:	add    %al,(%rax)
    1800049d2:	add    %al,(%rax)
-   1800049d4:	fwait
-   1800049d5:	rex.B sbb $0x66,%eax
-   1800049db:	add    %cl,-0x20000000(%rip)        # 0x1600049e1
+   1800049d4:	rex.R xchg %eax,%esp
+   1800049d6:	(bad)
+   1800049d7:	data16 add %al,(%rax)
+   1800049da:	add    %al,(%rax)
+   1800049dc:	or     $0xe0000000,%eax
    1800049e1:	add    (%rax),%al
    1800049e3:	add    %ah,0x0(%rsp,%rcx,2)
    1800049e7:	add    %ah,0x0(%rsi,%rsi,1)
 	...
    1800049ff:	add    %al,(%rcx)
 	...
    180004a09:	add    %al,(%rax)
```

## ipex_llm/libs/gptneox.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180055cd8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 15 15:02:52 2024
+Time/Date		Tue Apr 16 15:07:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000056600
 SizeOfInitializedData	00000000000c5a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000055cd8
@@ -116002,15 +116002,16 @@
    18005efdd:	add    %al,(%rax)
    18005efdf:	add    %bh,0x1800586(%rax)
    18005efe5:	add    %al,(%rax)
    18005efe7:	add    %al,%al
    18005efe9:	xchg   %al,0x180(%rip)        # 0x18005f16f
    18005efef:	add    %al,(%rax)
    18005eff1:	add    %al,(%rax)
-   18005eff3:	add    %bl,0x661d(%rcx,%rax,2)
+   18005eff3:	add    %al,0x1e(%rsp,%rdx,4)
+   18005eff7:	data16 add %al,(%rax)
    18005effa:	add    %al,(%rax)
    18005effc:	or     $0x50000000,%eax
    18005f001:	add    (%rax),%eax
    18005f003:	add    %al,-0x197bfffb(%rsp,%rdi,8)
    18005f00a:	add    $0x0,%eax
 	...
    18005f07f:	add    %bh,%al
```

## ipex_llm/libs/libbloom_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180053f68
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 15 15:07:24 2024
+Time/Date		Tue Apr 16 15:06:08 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000054400
 SizeOfInitializedData	00000000000bee00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000053f68
@@ -109707,15 +109707,18 @@
    18005d66a:	add    $0x180,%eax
    18005d66f:	add    %dh,0x66(%rax)
    18005d672:	add    $0x180,%eax
    18005d677:	add    %bh,0x66(%rax)
    18005d67a:	add    $0x180,%eax
    18005d67f:	add    %al,(%rax)
    18005d681:	add    %al,(%rax)
-   18005d683:	add    %ch,0x661d(%rdx,%rax,2)
+   18005d683:	add    %ah,%al
+   18005d685:	xchg   %eax,%ebx
+   18005d686:	(bad)
+   18005d687:	data16 add %al,(%rax)
    18005d68a:	add    %al,(%rax)
    18005d68c:	or     $0x50000000,%eax
    18005d691:	add    (%rax),%eax
    18005d693:	add    %ah,-0x5ffffa20(%rax)
    18005d699:	enter  $0x5,$0x0
 	...
    18005d6fd:	add    %al,(%rax)
```

## ipex_llm/libs/libbloom_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018004e788
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 15 15:04:02 2024
+Time/Date		Tue Apr 16 15:02:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000004ee00
 SizeOfInitializedData	00000000000bea00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000004e788
@@ -104729,17 +104729,20 @@
    1800576fa:	add    $0x180,%eax
    1800576ff:	add    %dh,0x6(%rax)
    180057702:	add    $0x180,%eax
    180057707:	add    %bh,0x6(%rax)
    18005770a:	add    $0x180,%eax
    18005770f:	add    %al,(%rax)
    180057711:	add    %al,(%rax)
-   180057713:	add    %ah,%dl
-   180057715:	rex.B sbb $0x66,%eax
-   18005771b:	add    %cl,0x50000000(%rip)        # 0x1d0057721
+   180057713:	add    %cl,(%rsi)
+   180057715:	xchg   %eax,%ebx
+   180057716:	(bad)
+   180057717:	data16 add %al,(%rax)
+   18005771a:	add    %al,(%rax)
+   18005771c:	or     $0x50000000,%eax
    180057721:	add    (%rax),%eax
    180057723:	add    %ah,(%rax)
    180057725:	addl   $0x0,0x5732000(%rip)        # 0x18578972f
 	...
    18005777f:	add    %dl,0x1800584(%rax)
    180057785:	add    %al,(%rax)
    180057787:	add    %bl,0x1800584(%rax)
```

## ipex_llm/libs/libgptneox_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005b758
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 15 15:07:25 2024
+Time/Date		Tue Apr 16 15:06:08 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c000
 SizeOfInitializedData	00000000000c6000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005b758
@@ -121130,17 +121130,20 @@
    180063f2f:	add    %bh,0x18005d6(%rax)
    180063f35:	add    %al,(%rax)
    180063f37:	add    %al,%al
    180063f39:	(bad)
    180063f3a:	add    $0x180,%eax
    180063f3f:	add    %al,(%rax)
    180063f41:	add    %al,(%rax)
-   180063f43:	add    %ch,0x661d42(%rbp)
-   180063f49:	add    %al,(%rax)
-   180063f4b:	add    %cl,0x50000000(%rip)        # 0x1d0063f51
+   180063f43:	add    %ah,%al
+   180063f45:	xchg   %eax,%ebx
+   180063f46:	(bad)
+   180063f47:	data16 add %al,(%rax)
+   180063f4a:	add    %al,(%rax)
+   180063f4c:	or     $0x50000000,%eax
    180063f51:	add    (%rax),%eax
    180063f53:	add    %al,0x3f840006(%rbx,%rcx,2)
    180063f5a:	(bad)
 	...
    180063f7f:	add    %bh,%al
    180063f81:	rex.WRX (bad)
    180063f83:	addb   $0x0,(%rcx)
```

## ipex_llm/libs/libgptneox_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180055ee8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 15 15:04:02 2024
+Time/Date		Tue Apr 16 15:02:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000056800
 SizeOfInitializedData	00000000000c5c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000055ee8
@@ -116158,17 +116158,20 @@
    18005efbd:	add    %al,(%rax)
    18005efbf:	add    %bh,0x1800586(%rax)
    18005efc5:	add    %al,(%rax)
    18005efc7:	add    %al,%al
    18005efc9:	xchg   %al,0x180(%rip)        # 0x18005f14f
    18005efcf:	add    %al,(%rax)
    18005efd1:	add    %al,(%rax)
-   18005efd3:	add    %ah,%dl
-   18005efd5:	rex.B sbb $0x66,%eax
-   18005efdb:	add    %cl,0x50000000(%rip)        # 0x1d005efe1
+   18005efd3:	add    %cl,(%rsi)
+   18005efd5:	xchg   %eax,%ebx
+   18005efd6:	(bad)
+   18005efd7:	data16 add %al,(%rax)
+   18005efda:	add    %al,(%rax)
+   18005efdc:	or     $0x50000000,%eax
    18005efe1:	add    (%rax),%eax
    18005efe3:	add    %al,(%rsp,%rdi,8)
    18005efe6:	add    $0x5e80400,%eax
 	...
    18005efff:	add    %bh,-0x1(%rax)
    18005f002:	add    $0x180,%eax
    18005f007:	add    %al,0x18005ff(%rax)
```

## ipex_llm/libs/libllama_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005a468
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 15 15:07:25 2024
+Time/Date		Tue Apr 16 15:06:08 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005ac00
 SizeOfInitializedData	00000000000c5e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005a468
@@ -119884,17 +119884,20 @@
    180063010:	enter  $0x5c6,$0x80
    180063014:	add    %eax,(%rax)
    180063016:	add    %al,(%rax)
    180063018:	rol    $1,%dh
    18006301a:	add    $0x180,%eax
    18006301f:	add    %al,(%rax)
    180063021:	add    %al,(%rax)
-   180063023:	add    %ch,0x661d42(%rbp)
-   180063029:	add    %al,(%rax)
-   18006302b:	add    %cl,0x50000000(%rip)        # 0x1d0063031
+   180063023:	add    %ah,%al
+   180063025:	xchg   %eax,%ebx
+   180063026:	(bad)
+   180063027:	data16 add %al,(%rax)
+   18006302a:	add    %al,(%rax)
+   18006302c:	or     $0x50000000,%eax
    180063031:	add    (%rax),%eax
    180063033:	add    %al,-0x7ffff9c4(%rax)
    180063039:	sub    $0x6,%al
 	...
    18006307f:	add    %dh,%al
    180063081:	(bad)
    180063082:	(bad)
```

## ipex_llm/libs/libllama_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180054bf8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 15 15:04:02 2024
+Time/Date		Tue Apr 16 15:02:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000055400
 SizeOfInitializedData	00000000000c5800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000054bf8
@@ -114891,17 +114891,20 @@
    18005e0a4:	add    %eax,(%rax)
    18005e0a6:	add    %al,(%rax)
    18005e0a8:	shlb   $1,0x5(%rsi)
    18005e0ab:	addb   $0x0,(%rcx)
    18005e0ae:	add    %al,(%rax)
    18005e0b0:	add    %al,(%rax)
    18005e0b2:	add    %al,(%rax)
-   18005e0b4:	loop   0x18005e0f7
-   18005e0b6:	sbb    $0x66,%eax
-   18005e0bb:	add    %cl,0x50000000(%rip)        # 0x1d005e0c1
+   18005e0b4:	(bad)
+   18005e0b5:	xchg   %eax,%ebx
+   18005e0b6:	(bad)
+   18005e0b7:	data16 add %al,(%rax)
+   18005e0ba:	add    %al,(%rax)
+   18005e0bc:	or     $0x50000000,%eax
    18005e0c1:	add    (%rax),%eax
    18005e0c3:	add    %al,(%rax)
    18005e0c5:	in     (%dx),%eax
    18005e0c6:	add    $0x5d50000,%eax
 	...
    18005e0ff:	add    %dh,-0x10(%rax)
    18005e102:	add    $0x180,%eax
```

## ipex_llm/libs/libstarcoder_avx.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800618c8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 15 15:07:24 2024
+Time/Date		Tue Apr 16 15:06:08 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000061e00
 SizeOfInitializedData	00000000000c7800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000618c8
@@ -130445,17 +130445,19 @@
    18006ab65:	add    %al,(%rax)
    18006ab67:	add    %al,%al
    18006ab69:	ss (bad)
    18006ab6b:	addb   $0x0,(%rcx)
    18006ab6e:	add    %al,(%rax)
    18006ab70:	add    %al,(%rax)
    18006ab72:	add    %al,(%rax)
-   18006ab74:	lods   %ds:(%rsi),%al
-   18006ab75:	rex.X sbb $0x66,%eax
-   18006ab7b:	add    %cl,0x50000000(%rip)        # 0x1d006ab81
+   18006ab74:	loopne 0x18006ab09
+   18006ab76:	(bad)
+   18006ab77:	data16 add %al,(%rax)
+   18006ab7a:	add    %al,(%rax)
+   18006ab7c:	or     $0x50000000,%eax
    18006ab81:	add    (%rax),%eax
    18006ab83:	add    %dl,-0x43(%rax)
    18006ab86:	(bad)
    18006ab87:	add    %dl,-0x51(%rax)
    18006ab8a:	(bad)
 	...
    18006abff:	add    %al,%al
```

## ipex_llm/libs/libstarcoder_vnni.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005c0e8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 15 15:04:02 2024
+Time/Date		Tue Apr 16 15:02:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c800
 SizeOfInitializedData	00000000000c7200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005c0e8
@@ -125332,17 +125332,20 @@
    180065c35:	add    %al,(%rax)
    180065c37:	add    %al,%al
    180065c39:	out    %al,$0x5
    180065c3b:	addb   $0x0,(%rcx)
    180065c3e:	add    %al,(%rax)
    180065c40:	add    %al,(%rax)
    180065c42:	add    %al,(%rax)
-   180065c44:	loop   0x180065c87
-   180065c46:	sbb    $0x66,%eax
-   180065c4b:	add    %cl,0x50000000(%rip)        # 0x1d0065c51
+   180065c44:	(bad)
+   180065c45:	xchg   %eax,%ebx
+   180065c46:	(bad)
+   180065c47:	data16 add %al,(%rax)
+   180065c4a:	add    %al,(%rax)
+   180065c4c:	or     $0x50000000,%eax
    180065c51:	add    (%rax),%eax
    180065c53:	add    %dl,%al
    180065c55:	insl   (%dx),%es:(%rdi)
    180065c56:	(bad)
    180065c57:	add    %dl,%al
    180065c59:	pop    %rcx
    180065c5a:	(bad)
```

## ipex_llm/libs/llama-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002dac
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 15 15:02:51 2024
+Time/Date		Tue Apr 16 15:07:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002800
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002dac
@@ -5355,17 +5355,19 @@
    180004a20:	cmp    %al,0x0(%rdx)
    180004a23:	addb   $0x0,(%rcx)
    180004a26:	add    %al,(%rax)
    180004a28:	rex
    180004a29:	rex.X add %al,0x1(%rax)
    180004a30:	add    %al,(%rax)
    180004a32:	add    %al,(%rax)
-   180004a34:	fwait
-   180004a35:	rex.B sbb $0x66,%eax
-   180004a3b:	add    %cl,-0x20000000(%rip)        # 0x160004a41
+   180004a34:	rex.R xchg %eax,%esp
+   180004a36:	(bad)
+   180004a37:	data16 add %al,(%rax)
+   180004a3a:	add    %al,(%rax)
+   180004a3c:	or     $0xe0000000,%eax
    180004a41:	add    (%rax),%al
    180004a43:	add    %ah,%ah
    180004a45:	rex.WR add %r8b,(%rax)
    180004a48:	in     $0x38,%al
 	...
    180004a7e:	add    %al,(%rax)
    180004a80:	add    %eax,(%rax)
```

## ipex_llm/libs/llama.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800549e8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 15 15:02:52 2024
+Time/Date		Tue Apr 16 15:07:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000055000
 SizeOfInitializedData	00000000000c5800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000549e8
@@ -114691,15 +114691,16 @@
    18005d0c1:	add    $0x180,%ax
    18005d0c5:	add    %al,(%rax)
    18005d0c7:	add    %dl,%al
    18005d0c9:	add    $0x180,%ax
    18005d0cd:	add    %al,(%rax)
    18005d0cf:	add    %al,(%rax)
    18005d0d1:	add    %al,(%rax)
-   18005d0d3:	add    %bl,0x661d(%rcx,%rax,2)
+   18005d0d3:	add    %al,0x1e(%rsp,%rdx,4)
+   18005d0d7:	data16 add %al,(%rax)
    18005d0da:	add    %al,(%rax)
    18005d0dc:	or     $0x50000000,%eax
    18005d0e1:	add    (%rax),%eax
    18005d0e3:	add    %al,(%rax)
    18005d0e5:	fldl   0x5d10000(%rip)        # 0x185d6d0eb
 	...
    18005d0ff:	add    %dh,-0x20(%rax)
```

## ipex_llm/libs/main-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001045c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon Apr 15 15:02:51 2024
+Time/Date		Tue Apr 16 15:07:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010800
 SizeOfInitializedData	0000000000008e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001045c
@@ -25509,17 +25509,19 @@
    140014ab0:	enter  $0x125,$0x40
    140014ab4:	add    %eax,(%rax)
    140014ab6:	add    %al,(%rax)
    140014ab8:	shlb   $1,0x14001(%rip)        # 0x140028abf
    140014abe:	add    %al,(%rax)
    140014ac0:	add    %al,(%rax)
    140014ac2:	add    %al,(%rax)
-   140014ac4:	fwait
-   140014ac5:	rex.B sbb $0x66,%eax
-   140014acb:	add    %cl,0x20000000(%rip)        # 0x160014ad1
+   140014ac4:	rex.R xchg %eax,%esp
+   140014ac6:	(bad)
+   140014ac7:	data16 add %al,(%rax)
+   140014aca:	add    %al,(%rax)
+   140014acc:	or     $0x20000000,%eax
    140014ad1:	add    (%rax),%eax
    140014ad3:	add    %cl,%ah
    140014ad5:	push   %rsp
    140014ad6:	add    %eax,(%rax)
    140014ad8:	int3
    140014ad9:	rex add %eax,(%rax)
 	...
```

## ipex_llm/libs/main-chatglm_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400836bc
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon Apr 15 15:04:30 2024
+Time/Date		Tue Apr 16 15:03:06 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000087c00
 SizeOfInitializedData	00000000000cbe00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000836bc
@@ -188955,17 +188955,20 @@
    140093e25:	add    %al,(%rax)
    140093e27:	add    %al,(%rax)
    140093e29:	cltd
    140093e2a:	or     %al,0x1(%rax)
    140093e2d:	add    %al,(%rax)
    140093e2f:	add    %al,(%rax)
    140093e31:	add    %al,(%rax)
-   140093e33:	add    %bh,%dh
-   140093e35:	rex.B sbb $0x66,%eax
-   140093e3b:	add    %cl,-0x34000000(%rip)        # 0x10c093e41
+   140093e33:	add    %ch,(%rdx)
+   140093e35:	xchg   %eax,%ebx
+   140093e36:	(bad)
+   140093e37:	data16 add %al,(%rax)
+   140093e3a:	add    %al,(%rax)
+   140093e3c:	or     $0xcc000000,%eax
    140093e41:	add    (%rax),%eax
    140093e43:	add    %dl,-0x6ffff68e(%rax)
    140093e49:	(bad)
 	...
    140093e7e:	add    %al,(%rax)
    140093e80:	xorb   $0x40,0x9(%rsi)
    140093e84:	add    %eax,(%rax)
```

## ipex_llm/libs/main-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000ef6c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon Apr 15 15:02:51 2024
+Time/Date		Tue Apr 16 15:07:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f200
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000ef6c
@@ -24136,17 +24136,19 @@
    140013edf:	add    %ch,%al
    140013ee1:	adc    $0x14001,%eax
    140013ee6:	add    %al,(%rax)
    140013ee8:	lock adc $0x14001,%eax
    140013eee:	add    %al,(%rax)
    140013ef0:	add    %al,(%rax)
    140013ef2:	add    %al,(%rax)
-   140013ef4:	fwait
-   140013ef5:	rex.B sbb $0x66,%eax
-   140013efb:	add    %cl,-0x70000000(%rip)        # 0xd0013f01
+   140013ef4:	rex.R xchg %eax,%esp
+   140013ef6:	(bad)
+   140013ef7:	data16 add %al,(%rax)
+   140013efa:	add    %al,(%rax)
+   140013efc:	or     $0x90000000,%eax
    140013f01:	add    (%rax),%eax
    140013f03:	add    %ch,0x1(%rcx,%rcx,2)
    140013f07:	add    %ch,0x1(%rdi,%rbp,1)
 	...
    140013f7f:	add    %ah,(%rax)
    140013f81:	add    %r8,0x1(%r8)
    140013f85:	add    %al,(%rax)
```

## ipex_llm/libs/main-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014000f32c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon Apr 15 15:02:52 2024
+Time/Date		Tue Apr 16 15:07:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000000f600
 SizeOfInitializedData	0000000000009400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000f32c
@@ -24679,17 +24679,19 @@
    140013faf:	add    %ch,%al
    140013fb1:	adc    $0x14001,%eax
    140013fb6:	add    %al,(%rax)
    140013fb8:	lock adc $0x14001,%eax
    140013fbe:	add    %al,(%rax)
    140013fc0:	add    %al,(%rax)
    140013fc2:	add    %al,(%rax)
-   140013fc4:	pushf
-   140013fc5:	rex.B sbb $0x66,%eax
-   140013fcb:	add    %cl,-0x70000000(%rip)        # 0xd0013fd1
+   140013fc4:	rex.R xchg %eax,%esp
+   140013fc6:	(bad)
+   140013fc7:	data16 add %al,(%rax)
+   140013fca:	add    %al,(%rax)
+   140013fcc:	or     $0x90000000,%eax
    140013fd1:	add    (%rax),%eax
    140013fd3:	add    %ch,%ah
    140013fd5:	add    %rax,(%r8)
    140013fd8:	in     (%dx),%al
    140013fd9:	xor    (%rcx),%eax
 	...
    140013fff:	add    %ah,0x140014d(%rax)
```

## ipex_llm/libs/main-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014001a85c
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon Apr 15 15:02:52 2024
+Time/Date		Tue Apr 16 15:07:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000001b000
 SizeOfInitializedData	000000000000bc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001a85c
@@ -40341,15 +40341,16 @@
    14001f111:	movb   $0x40,(%rcx)
    14001f114:	add    %eax,(%rax)
    14001f116:	add    %al,(%rax)
    14001f118:	push   $0x14001c6
    14001f11d:	add    %al,(%rax)
    14001f11f:	add    %al,(%rax)
    14001f121:	add    %al,(%rax)
-   14001f123:	add    %bl,0x661d(%rcx,%rax,2)
+   14001f123:	add    %al,0x1e(%rsp,%rdx,4)
+   14001f127:	data16 add %al,(%rax)
    14001f12a:	add    %al,(%rax)
    14001f12c:	or     $0x20000000,%eax
    14001f131:	add    (%rax),%eax
    14001f133:	add    %dl,(%rbx,%rax,1)
    14001f136:	add    (%rax),%al
    14001f138:	adc    $0xf7,%al
    14001f13a:	add    %eax,(%rax)
```

## ipex_llm/libs/quantize-bloom.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013918
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon Apr 15 15:02:52 2024
+Time/Date		Tue Apr 16 15:07:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013a00
 SizeOfInitializedData	00000000000acc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013918
@@ -32184,15 +32184,16 @@
    140019125:	add    %al,(%rax)
    140019127:	add    %al,(%rax)
    140019129:	push   %rbp
    14001912a:	add    %eax,0x1(%rax)
    14001912d:	add    %al,(%rax)
    14001912f:	add    %al,(%rax)
    140019131:	add    %al,(%rax)
-   140019133:	add    %bl,0x661d(%rcx,%rax,2)
+   140019133:	add    %al,0x1e(%rsp,%rdx,4)
+   140019137:	data16 add %al,(%rax)
    14001913a:	add    %al,(%rax)
    14001913c:	or     $0x20000000,%eax
    140019141:	add    (%rax),%eax
    140019143:	add    %dh,%al
    140019145:	movabs 0x18ef00001,%al
 	...
    14001917e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-bloom_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013b28
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon Apr 15 15:04:02 2024
+Time/Date		Tue Apr 16 15:02:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013b28
@@ -32326,17 +32326,20 @@
    140019105:	add    %al,(%rax)
    140019107:	add    %al,(%rax)
    140019109:	push   %rbp
    14001910a:	add    %eax,0x1(%rax)
    14001910d:	add    %al,(%rax)
    14001910f:	add    %al,(%rax)
    140019111:	add    %al,(%rax)
-   140019113:	add    %ah,%dl
-   140019115:	rex.B sbb $0x66,%eax
-   14001911b:	add    %cl,0x20000000(%rip)        # 0x160019121
+   140019113:	add    %cl,(%rsi)
+   140019115:	xchg   %eax,%ebx
+   140019116:	(bad)
+   140019117:	data16 add %al,(%rax)
+   14001911a:	add    %al,(%rax)
+   14001911c:	or     $0x20000000,%eax
    140019121:	add    (%rax),%eax
    140019123:	add    %dh,%al
    140019125:	movabs 0x190f00001,%al
 	...
    14001917e:	add    %al,(%rax)
    140019180:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/quantize-gptneox.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010988
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon Apr 15 15:02:51 2024
+Time/Date		Tue Apr 16 15:07:47 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010a00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010988
@@ -27145,17 +27145,19 @@
    140015f02:	add    %eax,0x1(%rax)
    140015f05:	add    %al,(%rax)
    140015f07:	add    %dh,0x23(%rax)
    140015f0a:	add    %eax,0x1(%rax)
    140015f0d:	add    %al,(%rax)
    140015f0f:	add    %al,(%rax)
    140015f11:	add    %al,(%rax)
-   140015f13:	add    %bl,0x661d41(%rbx)
-   140015f19:	add    %al,(%rax)
-   140015f1b:	add    %cl,-0x70000000(%rip)        # 0xd0015f21
+   140015f13:	add    %al,-0x6c(%rbx)
+   140015f16:	(bad)
+   140015f17:	data16 add %al,(%rax)
+   140015f1a:	add    %al,(%rax)
+   140015f1c:	or     $0x90000000,%eax
    140015f21:	add    (%rax),%eax
    140015f23:	add    %ch,%al
    140015f25:	add    %eax,%fs:(%rax)
    140015f28:	call   0x14001607f
 	...
    140015f7d:	add    %al,(%rax)
    140015f7f:	add    %bl,0x1400168(%rax)
```

## ipex_llm/libs/quantize-gptneox_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140010b98
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon Apr 15 15:04:01 2024
+Time/Date		Tue Apr 16 15:02:37 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000010c00
 SizeOfInitializedData	00000000000aa600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000010b98
@@ -27284,16 +27284,16 @@
    140015ee2:	add    %eax,0x1(%rax)
    140015ee5:	add    %al,(%rax)
    140015ee7:	add    %dh,0x23(%rax)
    140015eea:	add    %eax,0x1(%rax)
    140015eed:	add    %al,(%rax)
    140015eef:	add    %al,(%rax)
    140015ef1:	add    %al,(%rax)
-   140015ef3:	add    %ah,%cl
-   140015ef5:	rex.B sbb $0x66,%eax
+   140015ef3:	add    %cl,0x661e93(%rip)        # 0x140677d8c
+   140015ef9:	add    %al,(%rax)
    140015efb:	add    %cl,-0x70000000(%rip)        # 0xd0015f01
    140015f01:	add    (%rax),%eax
    140015f03:	add    %ch,%al
    140015f05:	add    %eax,%fs:(%rax)
    140015f08:	call   0x140016061
 	...
    140015f7d:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-llama.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x00000001400118e8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon Apr 15 15:02:51 2024
+Time/Date		Tue Apr 16 15:07:47 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011800
 SizeOfInitializedData	00000000000aaa00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000118e8
@@ -28436,17 +28436,19 @@
    140016fed:	add    %al,(%rax)
    140016fef:	add    %cl,0x1400133(%rax)
    140016ff5:	add    %al,(%rax)
    140016ff7:	add    %dl,0x1400133(%rax)
    140016ffd:	add    %al,(%rax)
    140016fff:	add    %al,(%rax)
    140017001:	add    %al,(%rax)
-   140017003:	add    %bl,0x661d41(%rbx)
-   140017009:	add    %al,(%rax)
-   14001700b:	add    %cl,-0x70000000(%rip)        # 0xd0017011
+   140017003:	add    %al,-0x6c(%rbx)
+   140017006:	(bad)
+   140017007:	data16 add %al,(%rax)
+   14001700a:	add    %al,(%rax)
+   14001700c:	or     $0x90000000,%eax
    140017011:	add    (%rax),%eax
    140017013:	add    %ch,%ah
    140017015:	jne    0x140017018
    140017017:	add    %ch,%ah
    140017019:	(bad)
    14001701a:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/quantize-llama_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140011af8
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon Apr 15 15:04:01 2024
+Time/Date		Tue Apr 16 15:02:37 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000011c00
 SizeOfInitializedData	00000000000aaa00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000011af8
@@ -28571,16 +28571,16 @@
    140016fcd:	add    %al,(%rax)
    140016fcf:	add    %cl,0x1400133(%rax)
    140016fd5:	add    %al,(%rax)
    140016fd7:	add    %dl,0x1400133(%rax)
    140016fdd:	add    %al,(%rax)
    140016fdf:	add    %al,(%rax)
    140016fe1:	add    %al,(%rax)
-   140016fe3:	add    %ah,%cl
-   140016fe5:	rex.B sbb $0x66,%eax
+   140016fe3:	add    %cl,0x661e93(%rip)        # 0x140678e7c
+   140016fe9:	add    %al,(%rax)
    140016feb:	add    %cl,-0x70000000(%rip)        # 0xd0016ff1
    140016ff1:	add    (%rax),%eax
    140016ff3:	add    %ch,0x1(%rbp,%rsi,2)
    140016ff7:	add    %ch,0x1(%rbp,%riz,2)
    140016ffb:	add    %al,(%rax)
    140016ffd:	add    %al,(%rax)
    140016fff:	add    %ah,(%rax)
```

## ipex_llm/libs/quantize-starcoder.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013c60
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon Apr 15 15:02:52 2024
+Time/Date		Tue Apr 16 15:07:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013c00
 SizeOfInitializedData	00000000000ace00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013c60
@@ -32539,15 +32539,16 @@
    140019225:	add    %al,(%rax)
    140019227:	add    %al,(%rax)
    140019229:	push   %rbp
    14001922a:	add    %eax,0x1(%rax)
    14001922d:	add    %al,(%rax)
    14001922f:	add    %al,(%rax)
    140019231:	add    %al,(%rax)
-   140019233:	add    %bl,0x661d(%rcx,%rax,2)
+   140019233:	add    %al,0x1e(%rsp,%rdx,4)
+   140019237:	data16 add %al,(%rax)
    14001923a:	add    %al,(%rax)
    14001923c:	or     $0x20000000,%eax
    140019241:	add    (%rax),%eax
    140019243:	add    %bh,%ah
    140019245:	movabs 0x191fc0001,%eax
 	...
    14001927e:	add    %al,(%rax)
```

## ipex_llm/libs/quantize-starcoder_vnni.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140013e70
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Mon Apr 15 15:04:02 2024
+Time/Date		Tue Apr 16 15:02:38 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000013e00
 SizeOfInitializedData	00000000000ad000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000013e70
@@ -32656,17 +32656,20 @@
    140019205:	add    %al,(%rax)
    140019207:	add    %al,(%rax)
    140019209:	push   %rbp
    14001920a:	add    %eax,0x1(%rax)
    14001920d:	add    %al,(%rax)
    14001920f:	add    %al,(%rax)
    140019211:	add    %al,(%rax)
-   140019213:	add    %ah,%dl
-   140019215:	rex.B sbb $0x66,%eax
-   14001921b:	add    %cl,0x20000000(%rip)        # 0x160019221
+   140019213:	add    %cl,(%rsi)
+   140019215:	xchg   %eax,%ebx
+   140019216:	(bad)
+   140019217:	data16 add %al,(%rax)
+   14001921a:	add    %al,(%rax)
+   14001921c:	or     $0x20000000,%eax
    140019221:	add    (%rax),%eax
    140019223:	add    %bh,%ah
    140019225:	movabs 0x193fc0001,%eax
 	...
    14001927e:	add    %al,(%rax)
    140019280:	add    %eax,(%rax)
 	...
```

## ipex_llm/libs/starcoder-api.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018000277c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 15 15:02:51 2024
+Time/Date		Tue Apr 16 15:07:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		0000000000002200
 SizeOfInitializedData	0000000000003400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000000277c
@@ -4028,17 +4028,19 @@
    1800045f0:	cmp    %al,0x0(%rdx)
    1800045f3:	addb   $0x0,(%rcx)
    1800045f6:	add    %al,(%rax)
    1800045f8:	rex
    1800045f9:	rex.X add %al,0x1(%rax)
    180004600:	add    %al,(%rax)
    180004602:	add    %al,(%rax)
-   180004604:	fwait
-   180004605:	rex.B sbb $0x66,%eax
-   18000460b:	add    %cl,-0x20000000(%rip)        # 0x160004611
+   180004604:	rex.R xchg %eax,%esp
+   180004606:	(bad)
+   180004607:	data16 add %al,(%rax)
+   18000460a:	add    %al,(%rax)
+   18000460c:	or     $0xe0000000,%eax
    180004611:	add    (%rax),%al
    180004613:	add    %ah,%ah
    180004615:	rex.W add %al,(%rax)
    180004618:	in     $0x2e,%al
 	...
    18000467e:	add    %al,(%rax)
    180004680:	add    %eax,(%rax)
```

## ipex_llm/libs/starcoder.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005bed8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Mon Apr 15 15:02:52 2024
+Time/Date		Tue Apr 16 15:07:48 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	37
 SizeOfCode		000000000005c600
 SizeOfInitializedData	00000000000c7200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005bed8
@@ -125227,17 +125227,19 @@
    180065c55:	add    %al,(%rax)
    180065c57:	add    %al,%al
    180065c59:	out    %al,$0x5
    180065c5b:	addb   $0x0,(%rcx)
    180065c5e:	add    %al,(%rax)
    180065c60:	add    %al,(%rax)
    180065c62:	add    %al,(%rax)
-   180065c64:	pushf
-   180065c65:	rex.B sbb $0x66,%eax
-   180065c6b:	add    %cl,0x50000000(%rip)        # 0x1d0065c71
+   180065c64:	rex.R xchg %eax,%esp
+   180065c66:	(bad)
+   180065c67:	data16 add %al,(%rax)
+   180065c6a:	add    %al,(%rax)
+   180065c6c:	or     $0x50000000,%eax
    180065c71:	add    (%rax),%eax
    180065c73:	add    %dl,%al
    180065c75:	insl   (%dx),%es:(%rdi)
    180065c76:	(bad)
    180065c77:	add    %dl,%al
    180065c79:	push   %rdi
    180065c7a:	(bad)
```

## ipex_llm/transformers/convert.py

```diff
@@ -613,15 +613,16 @@
         rope_base = model.config.rotary_emb_base
         from accelerate.big_modeling import init_empty_weights
 
         def split_qkv_proj_func(module):
             if "QWenAttention" in module.__class__.__name__:
                 c_attn_weight = module.c_attn.weight.data
                 c_attn_bias = module.c_attn.bias.data
-                projection_size = module.projection_size
+                # Compatible with AutoTP case
+                projection_size = c_attn_weight.shape[0] // 3
                 hid_size = module.hidden_size
                 with init_empty_weights():
                     q_proj = torch.nn.Linear(hid_size, projection_size)
                     k_proj = torch.nn.Linear(hid_size, projection_size)
                     v_proj = torch.nn.Linear(hid_size, projection_size)
                 if not model.config.to_dict().get("bigdl_transformers_low_bit", False):
                     q_proj.weight = torch.nn.Parameter(
```

## ipex_llm/transformers/model.py

```diff
@@ -326,22 +326,29 @@
             if imatrix_file is not None:
                 imatrix_data = load_imatrix_data(imatrix_file)
                 kwargs["imatrix_data"] = imatrix_data
             kwargs["embedding_qtype"] = embedding_qtype
             model = cls.load_convert(q_k, optimize_model, *args, **kwargs)
 
             if speculative:
-                from .speculative import speculative_generate, clear_benchmarks
+                from .speculative import speculative_generate, clear_benchmarks,\
+                    _crop_past_key_values
                 # load a sym_int4 model as draft model
                 draft_model = cls.load_convert('sym_int4', optimize_model, *args, **kwargs)
                 model.draft_model = draft_model
                 import types
                 # add speculative_generate to pretrained model dynamically
                 model.clear_benchmarks = types.MethodType(clear_benchmarks, model)
                 model.speculative_generate = types.MethodType(speculative_generate, model)
+                model._crop_past_key_values = types.MethodType(_crop_past_key_values, model)
+
+            # add lookup_generate to pretrained model
+            from .lookup import lookup_generate
+            import types
+            model.lookup_generate = types.MethodType(lookup_generate, model)
         else:
             # load default
             model = cls.HF_Model.from_pretrained(*args, **kwargs)
 
         return model
 
     @staticmethod
```

## ipex_llm/transformers/speculative.py

```diff
@@ -435,34 +435,57 @@
             elif model_type == "qwen":
                 past_key_values[i] = (new_cache_k.transpose(1, 2), new_cache_v.transpose(1, 2))
             else:
                 past_key_values[i] = (new_cache_k, new_cache_v)
     return past_key_values, not enough_kv_room
 
 
-@torch.no_grad()
-def speculative_generate(self,
-                         inputs: Optional[torch.Tensor] = None,
-                         draft_model=None,
-                         max_new_tokens=10,
-                         max_step_draft=8,
-                         th_stop_draft=0.8,
-                         auto_th_stop_draft=True,
-                         auto_parameters=[1, 0.5, 0.9, 1e-2, 0.9],
-                         hf_adjust=False,
-                         min_step_draft=3,
-                         generation_config: Optional[GenerationConfig] = None,
-                         attention_mask=None,
-                         **sampling_kwargs):
-    invalidInputError(draft_model is not None,
-                      "Draft model should be provided.")
-    # min_step_draft >= 1. Since the max_step_draft may adjust,
-    # min_step_draft can > max_step_draft
-    min_step_draft = min_step_draft if min_step_draft >= 1 else 1
+def _crop_past_key_values(self, past_key_values, new_cache_size, _enable_ipex=False):
+    if _enable_ipex:
+        cur_len = past_key_values[0][0].size(1)
+        delta = new_cache_size
+        tmp = torch.empty(1, (cur_len - delta), (cur_len - delta), 1,
+                          dtype=torch.long).contiguous()
+        past_key_values = [[tmp, key_cache, value_cache, beam_idx]
+                           for _, key_cache, value_cache, beam_idx in past_key_values]
+    else:
+        if self.config.model_type in ["qwen"]:
+            past_key_values = [
+                (k[:, :-(new_cache_size), :],
+                    v[:, :-(new_cache_size), :])
+                for k, v in past_key_values
+            ]
+        elif self.config.model_type == "chatglm":
+            # for chatglm, cache shape is [sl, bs, nh, hn]
+            past_key_values = [
+                (k[:-(new_cache_size), :, :, :],
+                    v[:-(new_cache_size), :, :, :])
+                for k, v in past_key_values
+            ]
+        elif self.config.model_type in ["baichuan", "gptj"]:
+            past_key_values = [
+                (k[:, :, :-(new_cache_size), :],
+                    v[:, :, :-(new_cache_size), :])
+                for k, v in past_key_values
+            ]
+        elif self.config.model_type == "gpt_bigcode":
+            past_key_values = [
+                kv[:, :-(new_cache_size)]
+                for kv in past_key_values
+            ]
+        else:
+            past_key_values = [
+                (k[:, :, :-(new_cache_size)],
+                    v[:, :, :-(new_cache_size)])
+                for k, v in past_key_values
+            ]
+    return past_key_values
 
+
+def _prepare_generate_args(self, inputs, generation_config, **sampling_kwargs):
     if generation_config is None:
         generation_config = self.generation_config
 
     generation_config = copy.deepcopy(generation_config)
     # All unused kwargs must be model kwargs
     model_kwargs = generation_config.update(**sampling_kwargs)
     generation_config.validate()
@@ -490,18 +513,35 @@
     # inputs_tensor has to be defined
     # model_input_name is defined if model-specific keyword input is passed
     # otherwise model_input_name is None
     # all model-specific keyword inputs are removed from `model_kwargs`
     inputs_tensor, model_input_name, model_kwargs = self._prepare_model_inputs(
         inputs, generation_config.bos_token_id, model_kwargs
     )
-    batch_size = inputs_tensor.shape[0]
 
     # 4. Define other model kwargs
-    # Removed not used
+    # model_kwargs["output_attentions"] = generation_config.output_attentions
+    # model_kwargs["output_hidden_states"] = generation_config.output_hidden_states
+    # # decoder-only models with inputs_embeds forwarding must use caching
+    # # (otherwise we can't detect whether we are generating the first new token or not,
+    # # and we only want to use the embeddings for the first new token)
+    # if not self.config.is_encoder_decoder and model_input_name == "inputs_embeds":
+    #     model_kwargs["use_cache"] = True
+    # else:
+    #     model_kwargs["use_cache"] = generation_config.use_cache
+
+    # accepts_attention_mask = "attention_mask" in set(
+    #     inspect.signature(self.forward).parameters.keys())
+    # requires_attention_mask = "encoder_outputs" not in model_kwargs
+
+    # if model_kwargs.get("attention_mask", None) is None and \
+    #         requires_attention_mask and accepts_attention_mask:
+    #     model_kwargs["attention_mask"] = self._prepare_attention_mask_for_generation(
+    #         inputs_tensor, generation_config.pad_token_id, generation_config.eos_token_id
+    #     )
 
     # decoder-only models should use left-padding for generation
     if not self.config.is_encoder_decoder:
         # If `input_ids` was given, check if the last id in any sequence is `pad_token_id`
         # Note: If using, `inputs_embeds` this check does not work,
         # because we want to be more hands-off.
         if (
@@ -539,14 +579,69 @@
     input_ids, model_kwargs = self._expand_inputs_for_generation(
         input_ids=input_ids,
         expand_size=generation_config.num_return_sequences,
         is_encoder_decoder=self.config.is_encoder_decoder,
         **model_kwargs,
     )
 
+    return input_ids, generation_config, logits_processor, stopping_criteria, model_kwargs
+
+
+def _non_cpu_ipex_verify(self, verify_input_ids, past_key_values, cur_attention_mask=None,
+                         return_dict=True, use_cache=True):
+    forward_args = {
+        "input_ids": verify_input_ids,
+        "past_key_values": past_key_values,
+        "return_dict": return_dict,
+        "use_cache": use_cache,
+    }
+    if cur_attention_mask:
+        forward_args["attention_mask"] = cur_attention_mask
+
+    if self.config.model_type == "chatglm":
+        past_key_value_len = past_key_values[0][0].shape[0]
+        position_ids = torch.arange(verify_input_ids.shape[1], dtype=torch.long,
+                                    device=verify_input_ids.device)
+        position_ids = position_ids.unsqueeze(0).repeat(1, 1) + past_key_value_len
+        forward_args["position_ids"] = position_ids
+    elif self.config.model_type == "gptj":
+        past_length = past_key_values[0][0].size(2)
+        input_len = verify_input_ids.shape[1]
+        position_ids = torch.arange(past_length, input_len + past_length,
+                                    dtype=torch.long, device=verify_input_ids.device)
+        position_ids = position_ids.unsqueeze(0).view(-1, input_len)
+        forward_args["position_ids"] = position_ids
+
+    return self(**forward_args)
+
+
+@torch.no_grad()
+def speculative_generate(self,
+                         inputs: Optional[torch.Tensor] = None,
+                         draft_model=None,
+                         max_new_tokens=10,
+                         max_step_draft=8,
+                         th_stop_draft=0.8,
+                         auto_th_stop_draft=True,
+                         auto_parameters=[1, 0.5, 0.9, 1e-2, 0.9],
+                         hf_adjust=False,
+                         min_step_draft=3,
+                         generation_config: Optional[GenerationConfig] = None,
+                         attention_mask=None,
+                         **sampling_kwargs):
+    invalidInputError(draft_model is not None,
+                      "Draft model should be provided.")
+    # min_step_draft >= 1. Since the max_step_draft may adjust,
+    # min_step_draft can > max_step_draft
+    min_step_draft = min_step_draft if min_step_draft >= 1 else 1
+
+    input_ids, generation_config, logits_processor, stopping_criteria, \
+        model_kwargs = _prepare_generate_args(self, inputs, generation_config,
+                                              **sampling_kwargs)
+
     step = 0
     step_draft = 0
     step_verify = 0
 
     draft_gen_length = max_step_draft + 6 if hf_adjust else max_step_draft + 1
     current_input_ids = input_ids
     generate_ids = torch.empty([input_ids.size(0), max_new_tokens+max_step_draft],
@@ -847,35 +942,16 @@
                                               attention_mask=cur_attention_mask,
                                               past_key_values=past_key_values,
                                               position_ids=position_ids,
                                               )
                 logits = output[0]
                 past_key_values = output[1]
             else:
-                forward_args = {
-                    "input_ids": drafted_input_ids,
-                    "past_key_values": past_key_values,
-                    "attention_mask": cur_attention_mask,
-                    "return_dict": True,
-                    "use_cache": True,
-                }
-                if self.config.model_type == "chatglm":
-                    past_key_value_len = past_key_values[0][0].shape[0]
-                    position_ids = torch.arange(drafted_input_ids.shape[1], dtype=torch.long,
-                                                device=drafted_input_ids.device)
-                    position_ids = position_ids.unsqueeze(0).repeat(1, 1) + past_key_value_len
-                    forward_args["position_ids"] = position_ids
-                elif self.config.model_type == "gptj":
-                    past_length = past_key_values[0][0].size(2)
-                    input_len = drafted_input_ids.shape[1]
-                    position_ids = torch.arange(past_length, input_len + past_length,
-                                                dtype=torch.long, device=drafted_input_ids.device)
-                    position_ids = position_ids.unsqueeze(0).view(-1, input_len)
-                    forward_args["position_ids"] = position_ids
-                output = self(**forward_args)
+                output = _non_cpu_ipex_verify(self, drafted_input_ids, past_key_values,
+                                              cur_attention_mask, return_dict=True, use_cache=True)
             if isinstance(output, dict):
                 logits = output['logits']
                 past_key_values = output['past_key_values']
             temp_input_ids = torch.cat((input_ids, generate_ids[:, :step],
                                         draft_generate_ids[:, 1:step_draft + 2]), dim=-1)
             for i in range(logits.size(1)):
                 logits[:, i, :] = logits_processor(temp_input_ids[:, :input_ids.size(1)+step+i],
@@ -935,53 +1011,18 @@
 
             max_of_max_matched = output_ids.size(1)
             # Accept number is max_matched, min is 1
             self.accept_num.append(max_matched)
             # Clean up target model KV cache
             if max_of_max_matched != max_matched:
                 output_ids = output_ids[:, :max_matched]
-                if _enable_ipex:
-                    cur_len = past_key_values[0][0].size(1)
-                    delta = max_of_max_matched - max_matched
-                    tmp = torch.empty(1, (cur_len - delta), (cur_len - delta), 1,
-                                      dtype=torch.long,
-                                      ).contiguous()
-                    past_key_values = [[tmp, key_cache, value_cache, beam_idx]
-                                       for _, key_cache, value_cache, beam_idx in past_key_values]
-                else:
-                    if self.config.model_type in ["qwen"]:
-                        past_key_values = [
-                            (k[:, :-(max_of_max_matched - max_matched), :],
-                             v[:, :-(max_of_max_matched - max_matched), :])
-                            for k, v in past_key_values
-                        ]
-                    elif self.config.model_type == "chatglm":
-                        # for chatglm, cache shape is [sl, bs, nh, hn]
-                        past_key_values = [
-                            (k[:-(max_of_max_matched - max_matched), :, :, :],
-                             v[:-(max_of_max_matched - max_matched), :, :, :])
-                            for k, v in past_key_values
-                        ]
-                    elif self.config.model_type in ["baichuan", "gptj"]:
-                        past_key_values = [
-                            (k[:, :, :-(max_of_max_matched - max_matched), :],
-                             v[:, :, :-(max_of_max_matched - max_matched), :])
-                            for k, v in past_key_values
-                        ]
-                    elif self.config.model_type == "gpt_bigcode":
-                        past_key_values = [
-                            kv[:, :-(max_of_max_matched - max_matched)]
-                            for kv in past_key_values
-                        ]
-                    else:
-                        past_key_values = [
-                            (k[:, :, :-(max_of_max_matched - max_matched)],
-                             v[:, :, :-(max_of_max_matched - max_matched)])
-                            for k, v in past_key_values
-                        ]
+                new_cache_size = max_of_max_matched - max_matched
+                past_key_values = self._crop_past_key_values(past_key_values,
+                                                             new_cache_size,
+                                                             _enable_ipex)
 
             # Each iter assign new_matched kv_cache to past_key_values1
             if self.device.type == 'cpu' and (not _enable_ipex):
                 _update_past_key_values_storage_cpu(self, past_key_values, past_key_values_storage,
                                                     original_draft_past_key_values,
                                                     _enable_ipex)
```

## ipex_llm/transformers/models/aquila.py

```diff
@@ -46,15 +46,15 @@
     append_kv_cache, is_enough_kv_cache_room_4_31
 from ipex_llm.transformers.models.utils import apply_rotary_pos_emb
 from ipex_llm.transformers.models.utils import apply_rotary_pos_emb_no_cache_xpu
 from ipex_llm.utils.common import log4Error
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def aquila_attention_forward(
     self,
     hidden_states: torch.Tensor,
     attention_mask: Optional[torch.Tensor] = None,
     position_ids: Optional[torch.LongTensor] = None,
```

## ipex_llm/transformers/models/baichuan.py

```diff
@@ -33,15 +33,15 @@
 from ipex_llm.transformers.models.utils import init_fp8_kv_cache, append_fp8_kv_cache, \
     restore_fp8_kv_cache, use_quantize_kv_cache
 from ipex_llm.transformers.models.utils import rotate_half, apply_rotary_pos_emb
 from ipex_llm.transformers.models.utils import apply_rotary_pos_emb_no_cache_xpu
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def baichuan_attention_forward_7b(
     self,
     hidden_states: torch.Tensor,
     attention_mask: Optional[torch.Tensor] = None,
     position_ids: Optional[torch.LongTensor] = None,
```

## ipex_llm/transformers/models/baichuan2.py

```diff
@@ -42,15 +42,15 @@
     logger.warning(
         "Xformers is not installed correctly. If you want to use memory_efficient_attention to "
         "accelerate training use the following command to install Xformers\npip install xformers."
     )
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def baichuan_13b_rms_norm_forward(self, hidden_states):
     if hidden_states.device.type == "xpu" and not (self.training and hidden_states.requires_grad):
         import linear_q4_0
         x_2d = hidden_states.reshape(-1, hidden_states.size(-1)).contiguous()
         output = linear_q4_0.rms_norm(self.weight, x_2d, self.epsilon)
```

## ipex_llm/transformers/models/bloom.py

```diff
@@ -38,15 +38,15 @@
 import torch.utils.checkpoint
 from torch.nn import functional as F
 from ipex_llm.transformers.models.utils import use_fused_layer_norm
 from ipex_llm.transformers.models.utils import init_kv_cache, extend_kv_cache, append_kv_cache
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def dropout_add(x: torch.Tensor, residual: torch.Tensor, prob: float, training: bool):
     """
     Dropout add function
 
     Args:
```

## ipex_llm/transformers/models/chatglm.py

```diff
@@ -36,15 +36,15 @@
     cos, sin = F.embedding(position_id, cos.squeeze(1)).unsqueeze(2), \
         F.embedding(position_id, sin.squeeze(1)).unsqueeze(2)
     q, k = (q * cos) + (rotate_half(q) * sin), (k * cos) + (rotate_half(k) * sin)
     return q, k
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 KV_CACHE_ALLOC_MIN_LENGTH = 512
 
 
 def attention_fn(
         self,
         query_layer,
         key_layer,
```

## ipex_llm/transformers/models/chatglm2.py

```diff
@@ -26,15 +26,15 @@
 from ipex_llm.transformers.models.utils import init_fp8_kv_cache, append_fp8_kv_cache, \
     restore_fp8_kv_cache, use_quantize_kv_cache
 from ipex_llm.transformers.models.utils import use_esimd_sdp
 
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 KV_CACHE_ALLOC_MIN_LENGTH = 512
 
 
 def split_tensor_along_last_dim(
         tensor: torch.Tensor,
         num_partitions: int,
         contiguous_split_chunks: bool = False,
```

## ipex_llm/transformers/models/chatglm2_32k.py

```diff
@@ -21,15 +21,15 @@
 from typing import Optional, Tuple, Union, List, Callable, Dict, Any
 import torch.nn.functional as F
 from ipex_llm.transformers.models.utils import init_kv_cache, extend_kv_cache, append_kv_cache
 
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 KV_CACHE_ALLOC_MIN_LENGTH = 512
 
 
 def split_tensor_along_last_dim(
         tensor: torch.Tensor,
         num_partitions: int,
         contiguous_split_chunks: bool = False,
```

## ipex_llm/transformers/models/decilm.py

```diff
@@ -39,15 +39,15 @@
     apply_rotary_pos_emb
 from ipex_llm.transformers.models.utils import apply_rotary_pos_emb_no_cache_xpu
 from ipex_llm.transformers.models.llama import should_use_fuse_rope, repeat_kv
 from ipex_llm.utils.common import invalidInputError
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def decilm_attention_forward_4_35_2(
     self,
     hidden_states: torch.Tensor,
     attention_mask: Optional[torch.Tensor] = None,
     position_ids: Optional[torch.LongTensor] = None,
```

## ipex_llm/transformers/models/falcon.py

```diff
@@ -39,15 +39,15 @@
 from torch.nn import functional as F
 from ipex_llm.utils.common import invalidInputError
 from ipex_llm.transformers.models.utils import init_kv_cache, extend_kv_cache, append_kv_cache
 import warnings
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 # Copied from transformers.models.llama.modeling_llama.rotate_half
 def rotate_half(x):
     """Rotates half the hidden dims of the input."""
     x1 = x[..., : x.shape[-1] // 2]
     x2 = x[..., x.shape[-1] // 2:]
```

## ipex_llm/transformers/models/gemma.py

```diff
@@ -41,15 +41,15 @@
 from ipex_llm.transformers.models.utils import mlp_fusion_check, GELU
 from ipex_llm.transformers.models.utils import is_enough_kv_cache_room_4_36, rotate_half
 from ipex_llm.transformers.low_bit_linear import SYM_INT4, FP8E5
 from ipex_llm.transformers.models.utils import decoding_fast_path_qtype_check
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def apply_rotary_pos_emb(q, k, cos, sin, position_ids=None, unsqueeze_dim=1):
     cos = cos.unsqueeze(unsqueeze_dim)
     sin = sin.unsqueeze(unsqueeze_dim)
     q_embed = (q * cos) + (rotate_half(q) * sin)
     k_embed = (k * cos) + (rotate_half(k) * sin)
```

## ipex_llm/transformers/models/gptj.py

```diff
@@ -24,15 +24,15 @@
 from transformers.utils.import_utils import is_torch_fx_proxy
 from transformers.modeling_outputs import BaseModelOutputWithPast
 from transformers.models.gptj.modeling_gptj import GPTJModel
 from ipex_llm.utils.common import invalidInputError
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def _get_embed_positions(self, position_ids):
     embed_positions = self.embed_positions
     if embed_positions.device != position_ids.device:
         embed_positions = embed_positions.to(position_ids.device)
         self.embed_positions = embed_positions
```

## ipex_llm/transformers/models/gptneox.py

```diff
@@ -36,15 +36,15 @@
 from ipex_llm.transformers.models.utils import apply_rotary_pos_emb
 from ipex_llm.transformers.models.utils import init_kv_cache, extend_kv_cache, \
     append_kv_cache, is_enough_kv_cache_room_4_31
 from ipex_llm.transformers.models.utils import apply_rotary_pos_emb_no_cache_xpu
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def gptneox_attention_forward(
         self,
         hidden_states: torch.FloatTensor,
         attention_mask: torch.FloatTensor,
         position_ids: torch.LongTensor,
```

## ipex_llm/transformers/models/internlm.py

```diff
@@ -46,15 +46,15 @@
 from ipex_llm.transformers.models.utils import init_kv_cache, extend_kv_cache, \
     append_kv_cache, is_enough_kv_cache_room_4_31
 from ipex_llm.transformers.models.utils import apply_rotary_pos_emb
 from ipex_llm.transformers.models.utils import apply_rotary_pos_emb_no_cache_xpu
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def internlm_attention_forward(
     self,
     hidden_states: torch.Tensor,
     attention_mask: Optional[torch.Tensor]=None,
     position_ids: Optional[torch.LongTensor]=None,
```

## ipex_llm/transformers/models/llama.py

```diff
@@ -79,15 +79,15 @@
     batch, num_key_value_heads, slen, head_dim = hidden_states.shape
     if n_rep == 1:
         return hidden_states
     hidden_states = hidden_states[:, :, None, :, :].expand(batch, num_key_value_heads,
                                                            n_rep, slen, head_dim)
     return hidden_states.reshape(batch, num_key_value_heads * n_rep, slen, head_dim)
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 _ipex_version = None
 
 
 def get_ipex_version():
```

## ipex_llm/transformers/models/mistral.py

```diff
@@ -59,15 +59,15 @@
 try:
     from transformers.cache_utils import Cache
 except ImportError:
     Cache = Tuple[torch.Tensor]
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def repeat_kv(hidden_states: torch.Tensor, n_rep: int) -> torch.Tensor:
     """
     This is the equivalent of torch.repeat_interleave(x, dim=1, repeats=n_rep).
     The hidden states go from (batch, num_key_value_heads, seqlen, head_dim)
     to (batch, num_attention_heads, seqlen, head_dim)
```

## ipex_llm/transformers/models/mixtral.py

```diff
@@ -56,15 +56,15 @@
 from ipex_llm.transformers.models.mistral import should_use_fuse_rope, use_decoding_fast_path
 from ipex_llm.transformers.models.utils import use_flash_attention, use_esimd_sdp
 from ipex_llm.transformers.models.utils import mlp_fusion_check, SILU
 from ipex_llm.transformers.low_bit_linear import IQ2_XXS
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def repeat_kv(hidden_states: torch.Tensor, n_rep: int) -> torch.Tensor:
     """
     This is the equivalent of torch.repeat_interleave(x, dim=1, repeats=n_rep).
     The hidden states go from (batch, num_key_value_heads, seqlen, head_dim)
     to (batch, num_attention_heads, seqlen, head_dim)
```

## ipex_llm/transformers/models/mpt.py

```diff
@@ -23,15 +23,15 @@
 import math
 import torch.nn.functional as F
 from ipex_llm.utils.common import invalidInputError
 from ipex_llm.transformers.models.utils import extend_kv_cache, init_kv_cache, append_kv_cache
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def mpt_multihead_attention_forward(self, x, past_key_value=None, attn_bias=None,
                                     attention_mask=None, is_causal=True,
                                     needs_weights=False, rotary_emb_w_meta_info=None,
                                     **kwargs):
     qkv = self.Wqkv(x)
```

## ipex_llm/transformers/models/phixtral.py

```diff
@@ -50,15 +50,15 @@
     apply_rotary_pos_emb_no_cache_xpu, is_enough_kv_cache_room_4_36
 from ipex_llm.transformers.models.mistral import should_use_fuse_rope, use_decoding_fast_path
 from ipex_llm.transformers.models.utils import use_flash_attention
 from ipex_llm.transformers.models.utils import mlp_fusion_check
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def repeat_kv(hidden_states: torch.Tensor, n_rep: int) -> torch.Tensor:
     """
     This is the equivalent of torch.repeat_interleave(x, dim=1, repeats=n_rep).
     The hidden states go from (batch, num_key_value_heads, seqlen, head_dim)
     to (batch, num_attention_heads, seqlen, head_dim)
```

## ipex_llm/transformers/models/qwen.py

```diff
@@ -52,15 +52,15 @@
 
 flash_attn_unpadded_func = None
 
 logger = logging.get_logger(__name__)
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 SUPPORT_TORCH2 = hasattr(torch, '__version__') and int(torch.__version__.split(".")[0]) >= 2
 
 
 def apply_rotary_pos_emb(t, freqs):
     cos, sin = freqs
     rot_dim = freqs[0].shape[-1]
     cos, sin = freqs
```

## ipex_llm/transformers/models/qwen2.py

```diff
@@ -67,15 +67,15 @@
 from transformers import logging
 
 
 logger = logging.get_logger(__name__)
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def should_use_fuse_rope(self, query_states, position_ids):
     use_fuse_rope = query_states.device.type == "xpu"
     use_fuse_rope = use_fuse_rope and not (self.training and query_states.requires_grad)
     use_fuse_rope = use_fuse_rope and position_ids is not None
     return use_fuse_rope
```

## ipex_llm/transformers/models/qwen_vl.py

```diff
@@ -33,15 +33,15 @@
 from ipex_llm.transformers.models.utils import extend_kv_cache, init_kv_cache, append_kv_cache
 from ipex_llm.transformers.models.utils import rotate_half
 from ipex_llm.transformers.models.utils import use_esimd_sdp
 from ipex_llm.transformers.models.utils import decoding_fast_path_qtype_check
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def apply_rotary_pos_emb(t, freqs):
     cos, sin = freqs
     rot_dim = freqs[0].shape[-1]
     t_, t_pass_ = t[..., :rot_dim], t[..., rot_dim:]
     t_ = t_.float()
```

## ipex_llm/transformers/models/stablelm.py

```diff
@@ -58,15 +58,15 @@
 try:
     from transformers.cache_utils import Cache
 except ImportError:
     Cache = Tuple[torch.Tensor]
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def merge_qkv(module: torch.nn.Module):
     if isinstance(module, StableLmAttention):
         new_weight = torch.cat([
             module.q_proj.weight.data,
             module.k_proj.weight.data,
```

## ipex_llm/transformers/models/yuan.py

```diff
@@ -36,15 +36,15 @@
     restore_fp8_kv_cache, use_quantize_kv_cache
 from ipex_llm.transformers.models.utils import is_enough_kv_cache_room_4_31, SILU
 from ipex_llm.transformers.low_bit_linear import SYM_INT4, FP8E5
 from ipex_llm.transformers.models.utils import decoding_fast_path_qtype_check
 
 import os
 
-KV_CACHE_ALLOC_BLOCK_LENGTH = os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256)
+KV_CACHE_ALLOC_BLOCK_LENGTH = int(os.environ.get("KV_CACHE_ALLOC_BLOCK_LENGTH", 256))
 
 
 def use_decoding_fast_path(proj, use_fuse_rope, enough_kv_room, bs):
     return decoding_fast_path_qtype_check(proj) and \
         use_fuse_rope and enough_kv_room and bs == 1 \
         and not proj.enable_xetla
```

## Comparing `ipex_llm-2.1.0b20240415.data/scripts/llm-chat.ps1` & `ipex_llm-2.1.0b20240416.data/scripts/llm-chat.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240415.data/scripts/llm-cli.ps1` & `ipex_llm-2.1.0b20240416.data/scripts/llm-cli.ps1`

 * *Files identical despite different names*

## Comparing `ipex_llm-2.1.0b20240415.dist-info/METADATA` & `ipex_llm-2.1.0b20240416.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipex-llm
-Version: 2.1.0b20240415
+Version: 2.1.0b20240416
 Summary: Large Language Model Develop Toolkit
 Home-page: https://github.com/intel-analytics/BigDL
 Author: BigDL Authors
 Author-email: bigdl-user-group@googlegroups.com
 License: Apache License, Version 2.0
 Platform: windows
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 Requires-Dist: transformers (==4.31.0) ; extra == 'all'
 Requires-Dist: sentencepiece ; extra == 'all'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'all'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'all'
 Requires-Dist: tabulate ; extra == 'all'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'all'
 Provides-Extra: cpp
-Requires-Dist: bigdl-core-cpp (==2.5.0b20240415) ; extra == 'cpp'
+Requires-Dist: bigdl-core-cpp (==2.5.0b20240416) ; extra == 'cpp'
 Provides-Extra: serving
 Requires-Dist: py-cpuinfo ; extra == 'serving'
 Requires-Dist: fschat[model_worker,webui] (==0.2.36) ; extra == 'serving'
 Requires-Dist: protobuf ; extra == 'serving'
 Provides-Extra: xpu
 Requires-Dist: py-cpuinfo ; extra == 'xpu'
 Requires-Dist: protobuf ; extra == 'xpu'
@@ -39,47 +39,47 @@
 Requires-Dist: sentencepiece ; extra == 'xpu'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu'
 Requires-Dist: tabulate ; extra == 'xpu'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240415) ; extra == 'xpu'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240415) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240416) ; extra == 'xpu'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240416) ; extra == 'xpu'
 Provides-Extra: xpu-2-0
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-0'
 Requires-Dist: protobuf ; extra == 'xpu-2-0'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-0'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-0'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-0'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-0'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-0'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-0'
 Requires-Dist: tabulate ; extra == 'xpu-2-0'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-0'
 Requires-Dist: torch (==2.0.1a0) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Requires-Dist: torchvision (==0.15.2a0) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Requires-Dist: intel-extension-for-pytorch (==2.0.110+xpu) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe (==2.5.0b20240415) ; (platform_system == "Linux") and extra == 'xpu-2-0'
-Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240415) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe (==2.5.0b20240416) ; (platform_system == "Linux") and extra == 'xpu-2-0'
+Requires-Dist: bigdl-core-xe-esimd (==2.5.0b20240416) ; (platform_system == "Linux") and extra == 'xpu-2-0'
 Provides-Extra: xpu-2-1
 Requires-Dist: py-cpuinfo ; extra == 'xpu-2-1'
 Requires-Dist: protobuf ; extra == 'xpu-2-1'
 Requires-Dist: mpmath (==1.3.0) ; extra == 'xpu-2-1'
 Requires-Dist: numpy (==1.26.4) ; extra == 'xpu-2-1'
 Requires-Dist: transformers (==4.31.0) ; extra == 'xpu-2-1'
 Requires-Dist: sentencepiece ; extra == 'xpu-2-1'
 Requires-Dist: tokenizers (==0.13.3) ; extra == 'xpu-2-1'
 Requires-Dist: accelerate (==0.21.0) ; extra == 'xpu-2-1'
 Requires-Dist: tabulate ; extra == 'xpu-2-1'
 Requires-Dist: torch (==2.1.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: torchvision (==0.16.0a0) ; extra == 'xpu-2-1'
 Requires-Dist: intel-extension-for-pytorch (==2.1.10+xpu) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240415) ; extra == 'xpu-2-1'
-Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240415) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-21 (==2.5.0b20240416) ; extra == 'xpu-2-1'
+Requires-Dist: bigdl-core-xe-esimd-21 (==2.5.0b20240416) ; extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu-2-1'
 Requires-Dist: intel-openmp ; (platform_machine == "x86_64" or platform_machine == "AMD64") and extra == 'xpu'
 
 
 IPEX LLM
```

## Comparing `ipex_llm-2.1.0b20240415.dist-info/RECORD` & `ipex_llm-2.1.0b20240416.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -38,68 +38,69 @@
 ipex_llm/langchain/embeddings/bigdlllm.py,sha256=auNueZ-S5RQrngss_huXlYdWImX2vPYfuEVOZsx35rk,13589
 ipex_llm/langchain/embeddings/transformersembeddings.py,sha256=hBtqBfGmGg_xjb4Us7hLNfyvbLMo5mJk9a0iooOWtPM,7225
 ipex_llm/langchain/llms/__init__.py,sha256=vBCl9JF45vnk9CWBG1k8lp8J6F8OCR9UY2E-idkkm5Y,1636
 ipex_llm/langchain/llms/bigdlllm.py,sha256=FAZG6cAIJhRgbxm16gMq-cyBwLe-u165zE7yyxD7r9E,24438
 ipex_llm/langchain/llms/transformersllm.py,sha256=7eaIkJi1CbTCSgNxBCoZTe-o_5FYjD1GTYPWpn0Ccr4,10576
 ipex_llm/langchain/llms/transformerspipelinellm.py,sha256=vm522YPPwWxxAPVvQBtxRfBinC4hIbXdKW6VjHDaFXY,7379
 ipex_llm/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ipex_llm/libs/bloom-api.dll,sha256=8vyckLdcy5usLjN5HKB5ofkCGgakEvw1VAkz5715Gj8,36352
-ipex_llm/libs/bloom.dll,sha256=RGvTZIbTJGrkKYt4JVhfiz3Y9DUHydPd4mdVIb05CgU,440320
-ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=w1pKCuXpV2NOb3szsZTOdIdm6dYc7bjovHLx7QwqqKQ,852992
-ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=STr-7enDMMFjZKF1-vEZcEsaEkCmux41XKoEKn4Gn4c,856064
-ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=of3wpx37VOAE9dBaLw2kFPmoxaYXJRfAG20X6a2CtUY,843776
-ipex_llm/libs/gptneox-api.dll,sha256=K1GvA0L25GcRyCOYmsKEIsm1TD5UMs-VGlZBssWyCUU,24576
-ipex_llm/libs/gptneox.dll,sha256=2T7sBNcNd54ziSeQvLtgVbU8Y18kRh4TY680264N9_Y,500224
-ipex_llm/libs/libbloom_avx.dll,sha256=5RoWp3XkTepWmStPuNP6AnKu47fBd3ynFcrtEKBHhIE,464384
-ipex_llm/libs/libbloom_vnni.dll,sha256=pMqWhEB5bRDlFr4FkQcB5ENlz_YtPbeFRm7mUS2JOv4,441344
-ipex_llm/libs/libgptneox_avx.dll,sha256=MkHGzd9rNVWsIzRRBMIgGZwAdsU6mLhYwX8y6DNM30g,524800
-ipex_llm/libs/libgptneox_vnni.dll,sha256=uwG1VQ014f-J7ndjxOV1Uxplkh6mdR439PhiG8y3yu8,501248
-ipex_llm/libs/libllama_avx.dll,sha256=QtpiFc5jP88uFoPsQcQ-QQaO8xP5542A_0v6kJVUv4k,519168
-ipex_llm/libs/libllama_vnni.dll,sha256=DYNkYa-iQVpR-NLGRdgdwKSWCaOB8WrWTWWGRZXOUek,495104
-ipex_llm/libs/libstarcoder_avx.dll,sha256=hHuOE7tasizCKy7abmQTEMeDQ-Sa2QUAXeH0JY3-Sa4,555520
-ipex_llm/libs/libstarcoder_vnni.dll,sha256=HmVwXDklJATiX63pROW6_EdyWpC0t3uwvasHD4c197Q,531968
-ipex_llm/libs/llama-api.dll,sha256=ItQTsUTdSkjOetYfUe23qJRLN6IoQjd0OdtX0eRLIOk,25088
-ipex_llm/libs/llama.dll,sha256=PX9QUbITe5HZzh3WUSHRuVSSL3awJnuCpASMqZfnWK0,494080
-ipex_llm/libs/main-bloom.exe,sha256=kPDW7odwG01XWnn5M1mqhXSDOBqO9lhuSOddo75QqVM,103424
-ipex_llm/libs/main-chatglm_vnni.exe,sha256=sZqnNhDFBmx-N8NywVNruHE-RQ-jGHvat8K6HtPFt0c,726016
-ipex_llm/libs/main-gptneox.exe,sha256=f2d--q00eM8GT94ySDLmTNMTDuXyindpHMo8EygIK_g,98816
-ipex_llm/libs/main-llama.exe,sha256=drliiPLAhbLRF5Co89Dwk1fy1CCaZH7VYkS0CiuxmKY,99840
-ipex_llm/libs/main-starcoder.exe,sha256=6De0OrEPg2f1_BGRF_NQ_mxhBg7-ckzHdO7Dfj4_S7U,157696
-ipex_llm/libs/quantize-bloom.exe,sha256=SBd-jJHXEiU1l_7nekN9ox5Ywok1MF5S_ku5VzNiF8Y,125952
-ipex_llm/libs/quantize-bloom_vnni.exe,sha256=lGYLDwZL6CNRoM1n1QiDuYXwotjJKQarkmQOCkmYJkQ,126976
-ipex_llm/libs/quantize-gptneox.exe,sha256=Syfdd7RuyiLlpN0WWhun8UJBeqU7risJM6aPA5Idlo4,103936
-ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=nFZtD34fapPLVUIshu0HAa7TtlYKi3O-Owx0SsyRk4Y,104448
-ipex_llm/libs/quantize-llama.exe,sha256=_PEtJXTu23wpBIf8KPlaDQCP3WhRo9EUB9tiYmw95A0,108544
-ipex_llm/libs/quantize-llama_vnni.exe,sha256=ARuSian_CU_OPQZrRFV_FAKUidzD4xZAGKhZNL-pRW0,109568
-ipex_llm/libs/quantize-starcoder.exe,sha256=SSBDX7AerA1PGxm18mkFaSlsQN-IiaaR8kelXHdLyho,126976
-ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=1--KJ_N58lgbSMnc3QbcxR_7bUePZUElvEKk04YvPSM,128000
-ipex_llm/libs/starcoder-api.dll,sha256=KuCK9WdLBLrVo3QfHLxIdnqtwrwJGLO3SIJhnBVud4k,21504
-ipex_llm/libs/starcoder.dll,sha256=NYw49Mzif7bR9J5Khh7m1FjmrBtBIrwWcLa0czPwp6c,531456
+ipex_llm/libs/bloom-api.dll,sha256=1eQcwK0wrDigeXsgeSrqHzHLewaAh9Bx5RPqX0D7Eg4,36352
+ipex_llm/libs/bloom.dll,sha256=xXEtPNqegXwAVzgjS0KHOd85WAsdIQj6xuxyKxoYJXk,440320
+ipex_llm/libs/chatglm_C.cp310-win_amd64.pyd,sha256=NqeSPGJHWWppNgZE7qnmrWzD7N3HHic5AHULQdwZNG8,852992
+ipex_llm/libs/chatglm_C.cp311-win_amd64.pyd,sha256=ZdF6fBZ5uTKH23ekseGkeV-02Lo61KTDEamdzbbBGSU,856064
+ipex_llm/libs/chatglm_C.cp39-win_amd64.pyd,sha256=ZeXYJ9ckbEeC02pha-wBbXSjLxUKhV4A1GVNx-9UwT8,843776
+ipex_llm/libs/gptneox-api.dll,sha256=NA__Wf37pt1AbM_mJVcxxfI123R5yKdbsphmWuEW_xA,24576
+ipex_llm/libs/gptneox.dll,sha256=n_cUv80peobdR8mPzwCsBc5_xU9xsgBaZmbm0nli--o,500224
+ipex_llm/libs/libbloom_avx.dll,sha256=RLw4St9KbLZ4h4X0sQfVQg47d-IlmaTn5bM84i8_NF8,464384
+ipex_llm/libs/libbloom_vnni.dll,sha256=HV29gfBoIhmCeVTEylkn6cdG1oPqWahY_RVjQQFj1bs,441344
+ipex_llm/libs/libgptneox_avx.dll,sha256=q5gsIArMAzIXThDKrFyveQ4si_gz84lzeVyhJUW8stE,524800
+ipex_llm/libs/libgptneox_vnni.dll,sha256=iSkk3bw-HHmAxeECd9wpFn5hpeq9G88LhNdmXm5YELc,501248
+ipex_llm/libs/libllama_avx.dll,sha256=52tScXr4FKplocnuqZzjbkOnXguL2jo9ZLugtX_ghwk,519168
+ipex_llm/libs/libllama_vnni.dll,sha256=m17L8Xd0lMEWtr-ntQKYy-0E08dLuxi0kmqG8x0VqQ8,495104
+ipex_llm/libs/libstarcoder_avx.dll,sha256=S7iBg2sd8ll41DG9OSuxUgzrHKufiyiHRUn-X_ctHl8,555520
+ipex_llm/libs/libstarcoder_vnni.dll,sha256=lK5kJENzvVe-n1BIlnLESbWmzGdLCvrSNfjvoOak6og,531968
+ipex_llm/libs/llama-api.dll,sha256=Cx-Rw68URiwpoS-EiqX0fsT37QQVkAL6R2jsg0npiZE,25088
+ipex_llm/libs/llama.dll,sha256=HtHPJ5WeEs6i_28H_BSlZULJqIZn0dLWdOT1svKdgAs,494080
+ipex_llm/libs/main-bloom.exe,sha256=JjJBxWyNt2K9gdarlAe40CVPQo7bNrYSADJxCKh9y34,103424
+ipex_llm/libs/main-chatglm_vnni.exe,sha256=GvVsba098Y8VfiNBp8ka4TPn4mOl89zxh5q8vGOecJU,726016
+ipex_llm/libs/main-gptneox.exe,sha256=6jutxF2G_q9pwjpg2p1zsdxDYWDWQnNl9Tcz0iQDeF8,98816
+ipex_llm/libs/main-llama.exe,sha256=KEfafKkFIS0lqw1NcAKsMm8wQLEZkiBZUPJbxWPEzPM,99840
+ipex_llm/libs/main-starcoder.exe,sha256=RwXHxbWbb48biHoY7bindt1aABMQEbnlRwPxIzR0GB4,157696
+ipex_llm/libs/quantize-bloom.exe,sha256=PjltIFW99JoCFjEdY-n4J_O3UQ14fWX2CMqFYdfsRkE,125952
+ipex_llm/libs/quantize-bloom_vnni.exe,sha256=PDsPwTTaVvkUHLKhsFlYMu2mUJAxBbJbqXXoLDVrhoI,126976
+ipex_llm/libs/quantize-gptneox.exe,sha256=-Y-xBEOgfqH-aa4HoopxnATw9zDOpsrfvn8PC-B87Go,103936
+ipex_llm/libs/quantize-gptneox_vnni.exe,sha256=yycwzPIT9qbTDYzszSB2DYjziOXGm1aqzaBEE8WzWiE,104448
+ipex_llm/libs/quantize-llama.exe,sha256=GVYX2Iz1pVhrMRTzqi7xLo7vsLmqUjULzeCXLjQ7FVc,108544
+ipex_llm/libs/quantize-llama_vnni.exe,sha256=yXsVvzgIoUgUfDiMrWoSmulNOkGtrRrPSeihtulccPQ,109568
+ipex_llm/libs/quantize-starcoder.exe,sha256=dQNikLi0rpvvgr4KDQBMRGT74YCQK-tsQp2FS_x47io,126976
+ipex_llm/libs/quantize-starcoder_vnni.exe,sha256=rS7fbOaLKrgt3MZxbK2kTRIm6k4NfmQdcQFzL-xoVl0,128000
+ipex_llm/libs/starcoder-api.dll,sha256=wuxodteXCULpoi9KFL7XpZxzBg_uP1QAtgoUn8CsAFI,21504
+ipex_llm/libs/starcoder.dll,sha256=iW_V5X1VkT8ZT_l_E1U7h50s2MTfsYnD9_52KGGuTy8,531456
 ipex_llm/llamaindex/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/llamaindex/llms/__init__.py,sha256=KP1lEdGqDuxPoxL1ZSH25Pm2kKMPJBWUTLR0ckSLMIU,1139
 ipex_llm/llamaindex/llms/bigdlllm.py,sha256=FQBzq1KOjfc6uofTXAha3O7TqpJkNfOFepXQmOVlbnI,26314
 ipex_llm/serving/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/serving/fastchat/bigdl_llm_model.py,sha256=NXEN_3EPmcP3dDnvug4MokEXXE2zVUnENgBYxfubqic,10084
 ipex_llm/serving/fastchat/ipex_llm_worker.py,sha256=LNMHFYgJqna-4TfIYH7zfKElUXIYMqE0J0ICHpvMGPk,11371
 ipex_llm/serving/fastchat/model_worker.py,sha256=qJSLyWNkP6z70ysq4AV5SqHzXPJJiX2tz7AORB6jEvM,16649
 ipex_llm/serving/fastchat/vllm_worker.py,sha256=x22OLdf0IdvuzHHVspczXb4q6bq4GNldtc3YdZsNGUs,8692
 ipex_llm/transformers/__init__.py,sha256=8zrY1AGBb2_AeKGDWHY4PCJyzelYA4KwahD54jPoiPg,1005
 ipex_llm/transformers/bmm.py,sha256=BlYrXqeJuw-m136Nf_ST9i6WtZrX6BiTG_psTe1M3Y0,1213
-ipex_llm/transformers/convert.py,sha256=N9ckj329AQJEpkTaC9NzZ1M_I3TIGbwjVKFlIE8eVfE,67035
+ipex_llm/transformers/convert.py,sha256=XEJNjIv_-tpLOSgs4OzwAWs0U42IDhHF3dwExDUULWQ,67086
 ipex_llm/transformers/convert_ipex.py,sha256=HcG4efY4nK_uFHCVL9wYKlINHTcXdWYQEMrJNcmjQRE,14274
 ipex_llm/transformers/embedding.py,sha256=f3crD31fEq0pT-d4FV_fS_9uLhgW64BofAxhHSO1QbE,4613
 ipex_llm/transformers/kv.py,sha256=rllcXh7wQAtyLsXWg8BxAYJuIwTBp9aRElnKifCFWRg,4533
 ipex_llm/transformers/loader.py,sha256=mC9-RuJGIvpSdP0eyDQ3OY2q1SFTwM-TDlcv2ZSVNIo,5429
+ipex_llm/transformers/lookup.py,sha256=nrwSMPKClyjnHbe94dSOlJpKHRecBKsLhCCbnQ1HRYI,13535
 ipex_llm/transformers/low_bit_linear.py,sha256=kzN42_YnwOK0xjL-8GCbf5jKuOoZhT_VojULcT7Yxfc,38310
-ipex_llm/transformers/model.py,sha256=Fdc13SEGFmaOZ7SGwVQ9lGyTDaLO2pfwxZsCnv9x5nA,35408
+ipex_llm/transformers/model.py,sha256=KQI-P3kPAMKk4HpDlvcmhp1CdluY30xF2fuLyRdprLQ,35750
 ipex_llm/transformers/modelling_bigdl.py,sha256=AqbRwpSAiHmKUo2FGOiwKtytlh-35NWb6eDy7YyNzoo,6921
 ipex_llm/transformers/qlora.py,sha256=WwHn2NXwx8SM6k7_xK1veppWiwL3g5PKihrbC3SPm-g,14770
 ipex_llm/transformers/relora.py,sha256=-dYzUV0P-IhO2jFdnzN9-v_sFzJpRj3ZwN9eCJzOoCw,16567
-ipex_llm/transformers/speculative.py,sha256=9BfwAElx5pIlDc4oCqB2u42yvryfMHHi_w02gsUn9v4,53041
+ipex_llm/transformers/speculative.py,sha256=uGHgwn5qKDIWySo6ocKKGw3U_jJUEwiYOU1YaDxxriI,54368
 ipex_llm/transformers/training_patch.py,sha256=4_eQ2uCtGOnRVC2iPkzquuYnvERdneBb7Ovu_pc-VCA,8404
 ipex_llm/transformers/utils.py,sha256=kqjrM83Ir8o9fdhZ6Ks-XZ-x-xDyBVjGh6q9Wnlo5Io,13781
 ipex_llm/transformers/xpu_customize_fwd.py,sha256=wFpIhs5F6tkNs8gBOrLxWdhLzO3EDHovVkERPIAoAvg,7611
 ipex_llm/transformers/awq/__init__.py,sha256=Du5gu3-eeAkeDO_dEMBTzrDBA66DSN3uL3-rn8WGXQw,875
 ipex_llm/transformers/awq/act.py,sha256=YwomJzOOKwkKtzGrm4L4kwBstBLO1Z8SK4CKi8PSYVQ,2172
 ipex_llm/transformers/awq/awq.py,sha256=cGyRQJWwAEJtOtdSbsBoQ33KX_Ie0pv5OJHC0ACEELE,8861
 ipex_llm/transformers/awq/awq_config.py,sha256=SDZJUCAxuphwwnGqjLrbCJIo4KmFmiNgZOeKJI4DmvY,4422
@@ -124,43 +125,43 @@
 ipex_llm/transformers/gguf/models/model_implement/falcon/tokenizer.json,sha256=Co_Ab5ygJdOT6lV05zuTWQKHbCpI8Bi80vgTCTR71tg,4060
 ipex_llm/transformers/gguf/models/model_implement/mpt/tokenizer.json,sha256=WGcZZnjOvPYwCslk4aZOTw_7yj_taeMv4-k3_yHZ8jk,7311
 ipex_llm/transformers/gguf/models/model_implement/yuan2/__init__.py,sha256=b2IXvVqQ5cItki021h8s3ymW12RPu8QNPprq4Mn3bDM,586
 ipex_llm/transformers/gguf/models/model_implement/yuan2/configuration_yuan.py,sha256=PDCUoD7z5cR-61oBjMc5uBCzgtiLx7sbTZ6nTnDU49A,2192
 ipex_llm/transformers/gguf/models/model_implement/yuan2/yuan_hf_model.py,sha256=_AOGMV65XHxgTxIib7lgs49InopcecTzRwgtYR8NTUg,51084
 ipex_llm/transformers/layers/rope_embedding.py,sha256=aL36BVCsjrWSi9DyMWsPOgj5VUNDooYsaO2HDaWAEzs,2658
 ipex_llm/transformers/models/__init__.py,sha256=tp2DcVkKg1-QvdYk7DY7rZvQWCDQ4ZjU8NAQ7Fclrpg,584
-ipex_llm/transformers/models/aquila.py,sha256=MsKstQfjgM3D_aLi3RjZMIuPzNnrPIOY_MMuI5UZufQ,7410
-ipex_llm/transformers/models/baichuan.py,sha256=UV-TEweC2vAJ_zEo2Yhg2cBhBV4P-6-zNlJwn782bKY,24483
-ipex_llm/transformers/models/baichuan2.py,sha256=RGZ8fOPQtZ3TxeG5L3nWJoP-c8AKhAD972eYGJcSxWM,27209
+ipex_llm/transformers/models/aquila.py,sha256=xLMxa8EOtpXDdyT9fAc0If_DkuH8Knzmi0Logrv0Jdk,7415
+ipex_llm/transformers/models/baichuan.py,sha256=Q8mEr3BubdhtW6sV_qMWYcvp_Uavvy8A7_2RcMSrOvg,24488
+ipex_llm/transformers/models/baichuan2.py,sha256=sskdX_cSuSY6IYIjBlp6L1feFK2B__41mEJB-0r5anc,27214
 ipex_llm/transformers/models/bert.py,sha256=bJNic2pt1kph0kBwdK5MRGyWupFfx2Ts0V3D1L-5kWo,6085
-ipex_llm/transformers/models/bloom.py,sha256=5bT-4Q7OmEGg9oM7E46F0SJKPtU05LVmWZF8lKoKRUo,8966
-ipex_llm/transformers/models/chatglm.py,sha256=zJ4kae-6ofYUEt0TnnIJh5MLVv-SpyXKeoBRVfhKRp0,13738
-ipex_llm/transformers/models/chatglm2.py,sha256=vyZzP2hM7GglmERgC2eAFGS3HSyd1VdnfNG3I2Fukqo,32035
-ipex_llm/transformers/models/chatglm2_32k.py,sha256=uLt2XtR9alp0p0hU9RKe8woOyo4P03G_dWDgHoofl-M,8692
-ipex_llm/transformers/models/decilm.py,sha256=vaFD8GFYImR66TC9__TbMAj3KVtS8ObJgBXsDxsPrp8,8649
-ipex_llm/transformers/models/falcon.py,sha256=tJZuujh2k8PAqdfWwPb_PVSW4Amc8AAKWvn5MlCOTzI,33544
-ipex_llm/transformers/models/gemma.py,sha256=1LwSXIbNOvfxW-zzXWvLdvOzZb_mzJi8yCcnwaLwPTw,12589
+ipex_llm/transformers/models/bloom.py,sha256=IfR1rEwQb157lY2yIBQmrsS185jsBpKhgPYXEeLDQVQ,8971
+ipex_llm/transformers/models/chatglm.py,sha256=crFSh7Df1xSpND27PPBtuDUOzT1aniNjW7xMHUiIcis,13743
+ipex_llm/transformers/models/chatglm2.py,sha256=7POlTOCeelx-chyud7e7ZRf6j6rtovThubkciSYYhwY,32040
+ipex_llm/transformers/models/chatglm2_32k.py,sha256=ch9Mw7T4haXcXMgqqubIi-mIQvlsdZ8gw6RhSbaUrao,8697
+ipex_llm/transformers/models/decilm.py,sha256=oAKyfB2_9GWheuqi3SyQXCBcRd6ixr6jeuYhN1z_d6A,8654
+ipex_llm/transformers/models/falcon.py,sha256=f5BzMbv4E-R5Pete8zBscbgiueXGIaWGs-5RbcMlUo4,33549
+ipex_llm/transformers/models/gemma.py,sha256=taxBCbyCj6HzwnCqLgrimoFFaB-MIK65yptVHkzwAvw,12594
 ipex_llm/transformers/models/gptbigcode.py,sha256=93l2PRLk1aLEhCGpio_7Y93amALS4SPrD5VXWiRl6hs,4342
-ipex_llm/transformers/models/gptj.py,sha256=I4ChjOkxgpJu1ZMOBF6pKxQP1fuEzISivxGr6OTj1vk,17968
-ipex_llm/transformers/models/gptneox.py,sha256=83g_WbiFxP-AECQgUtNJ1jvT3-cU4_rL6cg2yz17M2A,6214
-ipex_llm/transformers/models/internlm.py,sha256=CEcdWvc9-tEOYVWIYZKLnEiGnvSoLsoJ2iVoNQeexx8,11642
-ipex_llm/transformers/models/llama.py,sha256=o4BjBAwwX_DULIihg9MN_nUeCS3y85pd2Z2fUmgw3Po,96035
-ipex_llm/transformers/models/mistral.py,sha256=Pxyi4nFJZxnpsuH1-2vBBI5LZwEhuc027l_akITqLUA,45326
-ipex_llm/transformers/models/mixtral.py,sha256=XSDz-1r6W7zuayqLxaus4TSDv2HnIbKA-FlP4dhnCTo,27293
-ipex_llm/transformers/models/mpt.py,sha256=bvE9LTZRurZAkq4LQyMBgu2xQsmNosgDcNdamWfBVqM,9535
-ipex_llm/transformers/models/phixtral.py,sha256=_oB4PbeI5EdfkTZT_3v7AGpa9vlBmlXCh4FxDEK7ST4,6287
-ipex_llm/transformers/models/qwen.py,sha256=eAJOzOAL4XgvuPVojLcdm8YlSV6rQYDvdJcL2BaBWJU,32330
-ipex_llm/transformers/models/qwen2.py,sha256=nhFJWzBLNGzvM3LaAB4Y_ykOrPETMHCyFNnhBdBP-0g,32600
-ipex_llm/transformers/models/qwen_vl.py,sha256=Hb3abt-1RMsqOgGsft9QCyvf_2sRNYO3uXaYrPMaCO0,11813
+ipex_llm/transformers/models/gptj.py,sha256=TTIx461X2nOcIkrAcZhEf7d7mjJ3yvEC9KLVc1-hrpc,17973
+ipex_llm/transformers/models/gptneox.py,sha256=MVVdTbxV2oGzpCCzBMUy6oysVlnMtohJkl7SiC0xMAA,6219
+ipex_llm/transformers/models/internlm.py,sha256=mHyKQswtAHpT8R44gVvH7N57jjbk_GNtxjZWJy7ioog,11647
+ipex_llm/transformers/models/llama.py,sha256=EK7jre4G65MMc6gy4MwtHu_aXy_qbxfZbFv5nr0hwLI,96040
+ipex_llm/transformers/models/mistral.py,sha256=mIBM0SPQW-XqD-ZOD5AlUWHYFtRPDRLK88oLvM9_ZPA,45331
+ipex_llm/transformers/models/mixtral.py,sha256=PyPDLwpTI3a5D106YkRhVrxtEQQRSod_otQsEDxcCKE,27298
+ipex_llm/transformers/models/mpt.py,sha256=z02NwHogJZVh-Mk4sYoIzR90SFIKhoNN_-ifsD907TQ,9540
+ipex_llm/transformers/models/phixtral.py,sha256=ilc3bzey_L4MnkEnSCGxrq250LUZ9fQWx8p_Qp2gARM,6292
+ipex_llm/transformers/models/qwen.py,sha256=7vTTe3LdBCo4hf43wH6zl7ZQG5Qt2x3EwbTpMoStGU0,32335
+ipex_llm/transformers/models/qwen2.py,sha256=8jgOjK4niyEdZ64ZMsB3Lv7YJ5a4RQzGTc2D9J2AAFE,32605
+ipex_llm/transformers/models/qwen_vl.py,sha256=CM9DBrEp3z_r5Ext5yPCGYmgIw-5gvhJf03MYSeuJ1g,11818
 ipex_llm/transformers/models/rwkv4.py,sha256=Kzu6QlEi0KDXiJrfoZ71TI_D2nju2-sOeaKSZqdJz8U,6135
 ipex_llm/transformers/models/rwkv5.py,sha256=nNtWQROVAUc82SClzHrbaYVsr6CALnlVos0I2TX0YUc,10722
-ipex_llm/transformers/models/stablelm.py,sha256=FXyeVMKhj7ZqJi2UwY1Pcr0BvEhHjB7u6qE8IMKB91I,21120
+ipex_llm/transformers/models/stablelm.py,sha256=xmupwXKzswNhDQRLJcuVMzBM86v0JqNX3_Wn7tKKRng,21125
 ipex_llm/transformers/models/starcoder2.py,sha256=gQSoT4T3lM8Ve1A7CiOlIp7PMwKF2fyD2uCMQUvrY1I,8822
 ipex_llm/transformers/models/utils.py,sha256=Yu0zhCkKGlafzhsbPhQ4dpbrFBbHyecZlzpSQWE44Kg,17660
-ipex_llm/transformers/models/yuan.py,sha256=5oXNHU40lPW7wqO0cVvnFUjjKtlM66dK7yU4uWDEptY,20630
+ipex_llm/transformers/models/yuan.py,sha256=GVmOOx7SGb-S4sDyJx_d54qRl6_le5IkMA257innquI,20635
 ipex_llm/utils/__init__.py,sha256=T-EbRT6GJ_8RCu-iLmSzcftOimXSPQf2d5X72AUAy2Y,874
 ipex_llm/utils/convert_chatglm.py,sha256=YLbpJIbqnQOd8aJSijG5q4xBudNi_QR5sYVjCtYoVkY,18074
 ipex_llm/utils/convert_util.py,sha256=X1eLTdF9crlca6jPEQKymEITRx_57i_87dhl1htPEhc,72612
 ipex_llm/utils/glibc_checker.py,sha256=bm6kN6gbpA7GKtnUgsCE6K16iZZyil-Ylp55SoRvHG8,2093
 ipex_llm/utils/ipex_importer.py,sha256=sZro19_QZGr7oKiTq4P_i0CMUrDFlQkc7Ple9mV38CA,2477
 ipex_llm/utils/isa_checker.py,sha256=SisZ32B1G7meZvgRKZcani1WevIhMwum7nilZ3sHgXY,2259
 ipex_llm/utils/lazy_load_torch.py,sha256=MCZZr1NWwxOZQt-3OthNBxMxdN2jiRbvyXwJkrIKAhM,7129
@@ -197,14 +198,14 @@
 ipex_llm/vllm/model_executor/models/bigdl_llama.py,sha256=8mjFjUWXql-pmoibwlGLWpPmHAD-_bpwcnAm8V1GIxA,11428
 ipex_llm/vllm/model_executor/models/bigdl_mistral.py,sha256=slF_zjHXFrQUxB-Qsl_vc0AKbnnfC_ahfdDAKGGt7HE,8770
 ipex_llm/vllm/model_executor/models/bigdl_mixtral.py,sha256=AKRYNG366ZMpjORC30IOak2OdctqKS0TG1Y4FKv7XdE,8675
 ipex_llm/vllm/model_executor/models/bigdl_model.py,sha256=ysQ3UNwUDLIZVEPtVd_ADQHeRCN2INYQeFlVIZP8qy4,7699
 ipex_llm/vllm/transformers_utils/__init__.py,sha256=tp2DcVkKg1-QvdYk7DY7rZvQWCDQ4ZjU8NAQ7Fclrpg,584
 ipex_llm/vllm/transformers_utils/tokenizer.py,sha256=PKmEi1ROhf9dKRa-7AuKYwvAY-htP-ZIAz4HhNqhokU,8707
 ipex_llm/vllm/worker/worker.py,sha256=eifKuzefL9HC1R62P0mCYBsZlclo_5hQf01vFgc6mFA,13950
-ipex_llm-2.1.0b20240415.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
-ipex_llm-2.1.0b20240415.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
-ipex_llm-2.1.0b20240415.dist-info/METADATA,sha256=BsQ_lD7Jy0nTzP--qrdGNHhkSR2hFwwYm_C-39xE1Y4,4400
-ipex_llm-2.1.0b20240415.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-ipex_llm-2.1.0b20240415.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
-ipex_llm-2.1.0b20240415.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
-ipex_llm-2.1.0b20240415.dist-info/RECORD,,
+ipex_llm-2.1.0b20240416.data/scripts/llm-chat.ps1,sha256=6qrs-hGVAV8IKh7Jx8nq_XrnZcjd7qGU5wndArM7Yag,2769
+ipex_llm-2.1.0b20240416.data/scripts/llm-cli.ps1,sha256=3qBtTLs_EjYDnM8YyCpJhzLnGCKTEGssu9UNqfkjVXs,3009
+ipex_llm-2.1.0b20240416.dist-info/METADATA,sha256=NEQh45XYpiptv8FeXSjyPS1_DCp3kHXBXh_4Ims7FAY,4400
+ipex_llm-2.1.0b20240416.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+ipex_llm-2.1.0b20240416.dist-info/entry_points.txt,sha256=TiUyBB2MRmfF3ko-pyAEzqeBCRnyhu27bNOAsWPp3e8,61
+ipex_llm-2.1.0b20240416.dist-info/top_level.txt,sha256=CGCMHM-SyqUabU4h8RqJ2KTYckQUO3LvIWwmUQ6Qbzw,9
+ipex_llm-2.1.0b20240416.dist-info/RECORD,,
```

