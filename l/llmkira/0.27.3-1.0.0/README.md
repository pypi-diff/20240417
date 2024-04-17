# Comparing `tmp/llmkira-0.27.3.tar.gz` & `tmp/llmkira-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmkira-0.27.3.tar", last modified: Wed Jan 17 03:14:57 2024, max compression
+gzip compressed data, was "llmkira-1.0.0.tar", last modified: Wed Apr 17 06:20:08 2024, max compression
```

## Comparing `llmkira-0.27.3.tar` & `llmkira-1.0.0.tar`

### file list

```diff
@@ -1,149 +1,54 @@
--rw-r--r--   0        0        0    35149 2023-11-15 16:57:12.168727 llmkira-0.27.3/LICENSE
--rw-r--r--   0        0        0     1709 2023-11-13 07:08:42.929660 llmkira-0.27.3/NOTICE.MD
--rw-r--r--   0        0        0     8306 2023-11-25 15:25:17.445987 llmkira-0.27.3/README.md
--rw-r--r--   0        0        0      653 2023-10-17 02:36:48.806694 llmkira-0.27.3/llmkira/__init__.py
--rw-r--r--   0        0        0       31 2024-01-17 02:36:42.928989 llmkira-0.27.3/llmkira/elara.db
--rw-r--r--   0        0        0     3236 2023-12-23 03:39:29.018691 llmkira-0.27.3/llmkira/error.py
--rw-r--r--   0        0        0      130 2023-11-13 07:54:44.691343 llmkira-0.27.3/llmkira/external/__init__.py
--rw-r--r--   0        0        0      751 2023-11-13 07:57:56.694965 llmkira-0.27.3/llmkira/external/plugin.py
--rw-r--r--   0        0        0     1362 2023-11-14 02:42:10.695214 llmkira-0.27.3/llmkira/external/schema.py
--rw-r--r--   0        0        0      132 2023-10-14 16:33:30.471390 llmkira-0.27.3/llmkira/extra/__init__.py
--rw-r--r--   0        0        0      127 2023-10-26 15:33:49.274477 llmkira-0.27.3/llmkira/extra/plugins/__init__.py
--rw-r--r--   0        0        0     4518 2023-11-12 09:33:00.705843 llmkira-0.27.3/llmkira/extra/plugins/_finish.py
--rw-r--r--   0        0        0     8231 2023-11-14 08:59:17.243614 llmkira-0.27.3/llmkira/extra/plugins/_translate_doc.py
--rw-r--r--   0        0        0     6643 2023-11-14 16:14:16.511788 llmkira-0.27.3/llmkira/extra/plugins/alarm/__init__.py
--rw-r--r--   0        0        0     8768 2024-01-17 02:38:52.332291 llmkira-0.27.3/llmkira/extra/plugins/search.py
--rw-r--r--   0        0        0     7070 2023-11-14 16:14:16.508454 llmkira-0.27.3/llmkira/extra/plugins/sticker.py
--rw-r--r--   0        0        0     5334 2023-11-12 05:48:04.857796 llmkira-0.27.3/llmkira/extra/user/__init__.py
--rw-r--r--   0        0        0     1941 2023-11-14 08:55:15.789953 llmkira-0.27.3/llmkira/extra/user/client.py
--rw-r--r--   0        0        0     5922 2023-11-12 13:15:29.669913 llmkira-0.27.3/llmkira/extra/user/schema.py
--rw-r--r--   0        0        0      130 2023-10-14 16:33:30.474723 llmkira-0.27.3/llmkira/middleware/__init__.py
--rw-r--r--   0        0        0     2905 2023-11-19 04:55:25.153671 llmkira-0.27.3/llmkira/middleware/chain_box/__init__.py
--rw-r--r--   0        0        0     2699 2024-01-17 02:29:29.065493 llmkira-0.27.3/llmkira/middleware/chain_box/schema.py
--rw-r--r--   0        0        0     2849 2023-11-14 06:30:06.599711 llmkira-0.27.3/llmkira/middleware/env_virtual/__init__.py
--rw-r--r--   0        0        0     2679 2023-11-15 15:22:54.252562 llmkira-0.27.3/llmkira/middleware/func_reorganize/__init__.py
--rw-r--r--   0        0        0     2493 2023-11-14 08:55:15.803285 llmkira-0.27.3/llmkira/middleware/llm_provider.py
--rw-r--r--   0        0        0    10742 2023-11-24 02:28:52.152796 llmkira-0.27.3/llmkira/middleware/llm_task.py
--rw-r--r--   0        0        0      181 2023-11-14 07:05:54.512402 llmkira-0.27.3/llmkira/middleware/nlp_utils/__init__.py
--rw-r--r--   0        0        0     1920 2023-11-14 07:05:54.515735 llmkira-0.27.3/llmkira/middleware/router/__init__.py
--rw-r--r--   0        0        0     2143 2023-11-14 07:13:43.627120 llmkira-0.27.3/llmkira/middleware/router/schema.py
--rw-r--r--   0        0        0     1579 2023-11-09 14:46:35.339580 llmkira-0.27.3/llmkira/middleware/service_provider/__init__.py
--rw-r--r--   0        0        0      126 2023-10-29 04:45:17.280263 llmkira-0.27.3/llmkira/middleware/service_provider/kamiya.py
--rw-r--r--   0        0        0     1681 2023-11-08 05:51:00.867669 llmkira-0.27.3/llmkira/middleware/service_provider/private.py
--rw-r--r--   0        0        0     2867 2023-11-14 06:30:06.623036 llmkira-0.27.3/llmkira/middleware/service_provider/public.py
--rw-r--r--   0        0        0     1756 2023-11-12 13:15:29.686579 llmkira-0.27.3/llmkira/middleware/service_provider/schema.py
--rw-r--r--   0        0        0      175 2023-10-14 16:33:30.474723 llmkira-0.27.3/llmkira/receiver/__init__.py
--rw-r--r--   0        0        0     1685 2023-11-14 08:47:18.553946 llmkira-0.27.3/llmkira/receiver/app.py
--rw-r--r--   0        0        0     1218 2023-11-11 14:30:31.292669 llmkira-0.27.3/llmkira/receiver/aps.py
--rw-r--r--   0        0        0     8790 2023-11-12 11:59:17.952472 llmkira-0.27.3/llmkira/receiver/discord/__init__.py
--rw-r--r--   0        0        0    10892 2024-01-17 02:29:29.068826 llmkira-0.27.3/llmkira/receiver/function.py
--rw-r--r--   0        0        0     7666 2023-11-14 15:37:50.171732 llmkira-0.27.3/llmkira/receiver/kook/__init__.py
--rw-r--r--   0        0        0     1122 2023-10-20 09:53:09.716139 llmkira-0.27.3/llmkira/receiver/kook/http_client.py
--rw-r--r--   0        0        0    15444 2023-11-28 14:49:16.683945 llmkira-0.27.3/llmkira/receiver/receiver_client.py
--rw-r--r--   0        0        0      126 2023-10-21 14:35:22.272412 llmkira-0.27.3/llmkira/receiver/schema.py
--rw-r--r--   0        0        0     6849 2023-11-12 11:59:17.972471 llmkira-0.27.3/llmkira/receiver/slack/__init__.py
--rw-r--r--   0        0        0     2754 2023-10-21 12:13:57.992356 llmkira-0.27.3/llmkira/receiver/slack/creat_message.py
--rw-r--r--   0        0        0     7671 2024-01-17 02:15:24.107085 llmkira-0.27.3/llmkira/receiver/telegram/__init__.py
--rw-r--r--   0        0        0     3795 2023-11-14 06:39:08.329650 llmkira-0.27.3/llmkira/receiver/telegram/md2tgmd.py
--rw-r--r--   0        0        0      129 2023-10-17 14:02:43.400613 llmkira-0.27.3/llmkira/receiver/util_func.py
--rw-r--r--   0        0        0     6566 2023-11-13 13:51:08.967454 llmkira-0.27.3/llmkira/schema.py
--rw-r--r--   0        0        0      481 2023-11-14 05:46:55.788241 llmkira-0.27.3/llmkira/sdk/__init__.py
--rw-r--r--   0        0        0     2318 2023-11-12 14:30:58.757218 llmkira-0.27.3/llmkira/sdk/adapter.py
--rw-r--r--   0        0        0     3897 2023-11-14 08:48:12.271320 llmkira-0.27.3/llmkira/sdk/cache/__init__.py
--rw-r--r--   0        0        0      857 2023-11-14 08:47:18.523948 llmkira-0.27.3/llmkira/sdk/cache/base.py
--rw-r--r--   0        0        0     1528 2023-10-28 08:37:29.891900 llmkira-0.27.3/llmkira/sdk/cache/elara.py
--rw-r--r--   0        0        0     3297 2023-11-14 15:37:50.185065 llmkira-0.27.3/llmkira/sdk/cache/mongo.py
--rw-r--r--   0        0        0     2501 2024-01-14 06:14:22.922396 llmkira-0.27.3/llmkira/sdk/cache/redis.py
--rw-r--r--   0        0        0      454 2023-11-09 08:11:11.108856 llmkira-0.27.3/llmkira/sdk/endpoint/__init__.py
--rw-r--r--   0        0        0    12730 2023-11-14 06:50:22.546285 llmkira-0.27.3/llmkira/sdk/endpoint/openai/__init__.py
--rw-r--r--   0        0        0     3108 2023-11-12 13:02:38.894411 llmkira-0.27.3/llmkira/sdk/endpoint/schema.py
--rw-r--r--   0        0        0     3170 2023-11-14 07:39:34.637928 llmkira-0.27.3/llmkira/sdk/endpoint/tee.py
--rw-r--r--   0        0        0     4254 2023-11-12 15:11:15.683680 llmkira-0.27.3/llmkira/sdk/endpoint/tokenizer.py
--rw-r--r--   0        0        0      596 2023-10-30 08:27:22.531130 llmkira-0.27.3/llmkira/sdk/error.py
--rw-r--r--   0        0        0      268 2023-11-11 15:42:41.458855 llmkira-0.27.3/llmkira/sdk/filter/__init__.py
--rwxr-xr-x   0        0        0    11357 2023-10-14 16:33:30.474723 llmkira-0.27.3/llmkira/sdk/filter/api/LICENSE
--rwxr-xr-x   0        0        0      527 2023-10-14 16:33:30.474723 llmkira-0.27.3/llmkira/sdk/filter/api/README.md
--rwxr-xr-x   0        0        0      128 2023-10-14 16:33:30.474723 llmkira-0.27.3/llmkira/sdk/filter/api/__init__.py
--rw-r--r--   0        0        0    14678 2023-10-14 16:33:30.474723 llmkira-0.27.3/llmkira/sdk/filter/api/data/stop_words.txt
--rw-r--r--   0        0        0  7957390 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/api/data/synonym.json
--rwxr-xr-x   0        0        0      136 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/api/keyphrase/__init__.py
--rwxr-xr-x   0        0        0     3256 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/api/keyphrase/keyphrase.py
--rwxr-xr-x   0        0        0      198 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/api/keywords/__init__.py
--rwxr-xr-x   0        0        0      463 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/api/keywords/tfidf.py
--rw-r--r--   0        0        0       44 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/api/requirements.txt
--rw-r--r--   0        0        0      332 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/api/solo.py
--rwxr-xr-x   0        0        0      198 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/api/summarization/__init__.py
--rwxr-xr-x   0        0        0     2947 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/api/summarization/textrank_summarization.py
--rwxr-xr-x   0        0        0     2024 2023-11-11 15:42:41.448855 llmkira-0.27.3/llmkira/sdk/filter/api/summarization/tfidf_summarization.py
--rwxr-xr-x   0        0        0      198 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/api/text_similarity/__init__.py
--rwxr-xr-x   0        0        0     2056 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/api/text_similarity/cosion.py
--rwxr-xr-x   0        0        0      561 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/api/text_similarity/edit.py
--rwxr-xr-x   0        0        0     2328 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/api/text_similarity/simhash.py
--rw-r--r--   0        0        0     8880 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/evaluate.py
--rw-r--r--   0        0        0     1070 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/langdetect_fasttext/LICENSE
--rw-r--r--   0        0        0    13073 2023-10-14 16:38:46.115773 llmkira-0.27.3/llmkira/sdk/filter/langdetect_fasttext/README.md
--rw-r--r--   0        0        0       73 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/langdetect_fasttext/__init__.py
--rw-r--r--   0        0        0     2281 2023-10-31 02:48:40.593283 llmkira-0.27.3/llmkira/sdk/filter/langdetect_fasttext/detect.py
--rw-r--r--   0        0        0     1064 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/langdetect_unicode/LICENSE
--rw-r--r--   0        0        0      176 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/langdetect_unicode/__init__.py
--rw-r--r--   0        0        0     3400 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/langdetect_unicode/langdetect.py
--rw-r--r--   0        0        0     2811 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/filter/reduce.py
--rw-r--r--   0        0        0     4095 2023-10-31 02:48:01.434646 llmkira-0.27.3/llmkira/sdk/filter/sublimate.py
--rw-r--r--   0        0        0     1069 2023-10-14 16:33:30.501387 llmkira-0.27.3/llmkira/sdk/func_calling/LICENSE
--rw-r--r--   0        0        0     4383 2023-11-11 13:02:45.552263 llmkira-0.27.3/llmkira/sdk/func_calling/__init__.py
--rw-r--r--   0        0        0      496 2023-10-14 16:33:30.504720 llmkira-0.27.3/llmkira/sdk/func_calling/error.py
--rw-r--r--   0        0        0     3358 2023-10-14 16:33:30.504720 llmkira-0.27.3/llmkira/sdk/func_calling/loader.py
--rw-r--r--   0        0        0     9615 2023-11-11 15:42:41.448855 llmkira-0.27.3/llmkira/sdk/func_calling/model.py
--rw-r--r--   0        0        0     3365 2023-11-15 14:59:28.519422 llmkira-0.27.3/llmkira/sdk/func_calling/register.py
--rw-r--r--   0        0        0    10238 2023-11-26 12:52:04.898414 llmkira-0.27.3/llmkira/sdk/func_calling/schema.py
--rw-r--r--   0        0        0      130 2023-10-14 16:33:30.504720 llmkira-0.27.3/llmkira/sdk/memory/__init__.py
--rw-r--r--   0        0        0     1069 2023-10-26 14:11:15.657677 llmkira-0.27.3/llmkira/sdk/memory/redis/LICENSE
--rw-r--r--   0        0        0     2789 2023-11-12 12:18:55.856601 llmkira-0.27.3/llmkira/sdk/memory/redis/__init__.py
--rw-r--r--   0        0        0     6192 2023-11-11 15:42:41.442188 llmkira-0.27.3/llmkira/sdk/memory/redis/utils.py
--rw-r--r--   0        0        0     4759 2023-11-11 15:42:41.462188 llmkira-0.27.3/llmkira/sdk/network.py
--rw-r--r--   0        0        0      130 2023-10-23 11:43:58.996883 llmkira-0.27.3/llmkira/sdk/openapi/__init__.py
--rw-r--r--   0        0        0     2684 2023-11-25 12:42:15.597010 llmkira-0.27.3/llmkira/sdk/openapi/fuse/__init__.py
--rw-r--r--   0        0        0     4252 2023-11-13 12:42:20.447235 llmkira-0.27.3/llmkira/sdk/openapi/transducer/__init__.py
--rw-r--r--   0        0        0      797 2023-10-26 08:46:20.272481 llmkira-0.27.3/llmkira/sdk/openapi/transducer/default_factory.py
--rw-r--r--   0        0        0     1226 2023-11-07 13:48:59.771405 llmkira-0.27.3/llmkira/sdk/openapi/transducer/schema.py
--rw-r--r--   0        0        0     2096 2023-11-09 14:49:19.864125 llmkira-0.27.3/llmkira/sdk/openapi/trigger/__init__.py
--rw-r--r--   0        0        0      419 2023-10-30 08:36:07.716571 llmkira-0.27.3/llmkira/sdk/openapi/trigger/default_trigger.py
--rw-r--r--   0        0        0    23655 2023-11-14 16:35:26.633782 llmkira-0.27.3/llmkira/sdk/schema.py
--rw-r--r--   0        0        0     4556 2023-11-13 16:14:49.273505 llmkira-0.27.3/llmkira/sdk/utils.py
--rw-r--r--   0        0        0      176 2023-10-18 05:15:38.671491 llmkira-0.27.3/llmkira/sender/__init__.py
--rw-r--r--   0        0        0     1685 2023-11-14 08:47:18.553946 llmkira-0.27.3/llmkira/sender/app.py
--rw-r--r--   0        0        0    21025 2023-11-14 16:11:56.795239 llmkira-0.27.3/llmkira/sender/discord/__init__.py
--rw-r--r--   0        0        0      987 2023-10-30 07:49:44.471478 llmkira-0.27.3/llmkira/sender/discord/event.py
--rw-r--r--   0        0        0    20132 2023-11-14 16:11:56.798572 llmkira-0.27.3/llmkira/sender/kook/__init__.py
--rw-r--r--   0        0        0     1773 2023-10-27 17:37:52.534430 llmkira-0.27.3/llmkira/sender/kook/event.py
--rw-r--r--   0        0        0      161 2023-10-17 14:05:59.441649 llmkira-0.27.3/llmkira/sender/rss/__init__.py
--rw-r--r--   0        0        0     5879 2023-11-14 06:30:06.603043 llmkira-0.27.3/llmkira/sender/rss/rss.py
--rw-r--r--   0        0        0     1254 2023-10-23 16:44:07.471499 llmkira-0.27.3/llmkira/sender/schema.py
--rw-r--r--   0        0        0    24237 2023-11-14 16:11:56.788572 llmkira-0.27.3/llmkira/sender/slack/__init__.py
--rw-r--r--   0        0        0     2925 2023-11-12 09:27:01.134289 llmkira-0.27.3/llmkira/sender/slack/event.py
--rw-r--r--   0        0        0     3705 2023-11-14 06:39:08.316319 llmkira-0.27.3/llmkira/sender/slack/schema.py
--rw-r--r--   0        0        0    23494 2023-11-14 16:11:56.801905 llmkira-0.27.3/llmkira/sender/telegram/__init__.py
--rw-r--r--   0        0        0      779 2023-10-27 17:42:01.667980 llmkira-0.27.3/llmkira/sender/telegram/event.py
--rw-r--r--   0        0        0     2578 2024-01-17 02:23:03.097485 llmkira-0.27.3/llmkira/sender/util_func.py
--rw-r--r--   0        0        0     1038 2023-11-12 09:27:00.901026 llmkira-0.27.3/llmkira/setting/__init__.py
--rw-r--r--   0        0        0     1225 2023-11-14 07:56:19.172405 llmkira-0.27.3/llmkira/setting/discord.py
--rw-r--r--   0        0        0      848 2023-11-14 07:56:19.155740 llmkira-0.27.3/llmkira/setting/kook.py
--rw-r--r--   0        0        0     1659 2023-11-14 08:47:18.537280 llmkira-0.27.3/llmkira/setting/rabbitmq.py
--rw-r--r--   0        0        0     1813 2023-11-14 08:49:36.963791 llmkira-0.27.3/llmkira/setting/slack.py
--rw-r--r--   0        0        0     2322 2023-11-14 07:56:19.169072 llmkira-0.27.3/llmkira/setting/telegram.py
--rw-r--r--   0        0        0     4850 2023-11-14 03:43:04.608876 llmkira-0.27.3/llmkira/task/__init__.py
--rw-r--r--   0        0        0    30399 2023-12-03 14:39:09.115618 llmkira-0.27.3/llmkira/task/schema.py
--rw-r--r--   0        0        0     3877 2023-11-11 15:42:41.405520 llmkira-0.27.3/llmkira/tutorial.py
--rw-r--r--   0        0        0     2652 2024-01-17 03:14:57.342786 llmkira-0.27.3/pyproject.toml
--rw-r--r--   0        0        0       37 2023-11-14 02:20:12.969673 llmkira-0.27.3/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-11-14 02:20:12.969673 llmkira-0.27.3/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2023-11-14 02:20:12.966340 llmkira-0.27.3/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0       39 2023-11-14 09:18:28.673247 llmkira-0.27.3/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      207 2023-11-14 09:18:28.673247 llmkira-0.27.3/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-11-14 09:18:28.673247 llmkira-0.27.3/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      932 2024-01-17 02:51:12.798469 llmkira-0.27.3/tests/test_chain_box.py
--rw-r--r--   0        0        0     1121 2023-11-14 10:08:56.863571 llmkira-0.27.3/tests/test_external.py
--rw-r--r--   0        0        0      274 2023-11-14 10:22:46.530719 llmkira-0.27.3/tests/test_file.py
--rw-r--r--   0        0        0      417 2023-11-14 10:22:46.540720 llmkira-0.27.3/tests/test_message.py
--rw-r--r--   0        0        0      569 2024-01-17 02:15:43.218454 llmkira-0.27.3/tests/test_router.py
--rw-r--r--   0        0        0    11287 1970-01-01 00:00:00.000000 llmkira-0.27.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-17 06:19:52.611194 llmkira-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1030 2024-04-17 06:19:52.611194 llmkira-1.0.0/NOTICE.MD
+-rw-r--r--   0        0        0     6859 2024-04-17 06:19:52.611194 llmkira-1.0.0/README.md
+-rw-r--r--   0        0        0      730 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/__init__.py
+-rw-r--r--   0        0        0      209 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/_exception.py
+-rw-r--r--   0        0        0     3760 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/cache/__init__.py
+-rw-r--r--   0        0        0     1216 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/cache/elara_runtime.py
+-rw-r--r--   0        0        0     1426 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/cache/redis_runtime.py
+-rw-r--r--   0        0        0     1118 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/cache/runtime_schema.py
+-rw-r--r--   0        0        0     4235 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/doc_manager/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/extra/plugins/__init__.py
+-rw-r--r--   0        0        0     6726 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/extra/plugins/alarm/__init__.py
+-rw-r--r--   0        0        0     6510 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/extra/plugins/search/__init__.py
+-rw-r--r--   0        0        0     1774 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/extra/plugins/search/engine.py
+-rw-r--r--   0        0        0        0 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/kv_manager/__init__.py
+-rw-r--r--   0        0        0      626 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/kv_manager/_base.py
+-rw-r--r--   0        0        0     1750 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/kv_manager/env.py
+-rw-r--r--   0        0        0     4405 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/kv_manager/file.py
+-rw-r--r--   0        0        0      929 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/kv_manager/instruction.py
+-rw-r--r--   0        0        0     1070 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/kv_manager/tool_call.py
+-rw-r--r--   0        0        0      637 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/memory/__init__.py
+-rw-r--r--   0        0        0      729 2024-04-17 06:19:52.631193 llmkira-1.0.0/llmkira/memory/_base.py
+-rw-r--r--   0        0        0     2324 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/memory/local_storage.py
+-rw-r--r--   0        0        0     1070 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/memory/redis_storage/LICENSE
+-rw-r--r--   0        0        0     2840 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/memory/redis_storage/__init__.py
+-rw-r--r--   0        0        0     6192 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/memory/redis_storage/utils.py
+-rw-r--r--   0        0        0      522 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openai/__init__.py
+-rw-r--r--   0        0        0     3431 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openai/_excption.py
+-rw-r--r--   0        0        0     7440 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openai/cell.py
+-rw-r--r--   0        0        0     7811 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openai/request.py
+-rw-r--r--   0        0        0      130 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openapi/__init__.py
+-rw-r--r--   0        0        0     2729 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openapi/fuse/__init__.py
+-rw-r--r--   0        0        0     4285 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openapi/transducer/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openapi/transducer/default_factory.py
+-rw-r--r--   0        0        0     1229 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openapi/transducer/schema.py
+-rw-r--r--   0        0        0     2079 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openapi/trigger/__init__.py
+-rw-r--r--   0        0        0      419 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/openapi/trigger/default_trigger.py
+-rw-r--r--   0        0        0      321 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/__init__.py
+-rw-r--r--   0        0        0     1069 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/tools/LICENSE
+-rw-r--r--   0        0        0     4501 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/tools/__init__.py
+-rw-r--r--   0        0        0      496 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/tools/error.py
+-rw-r--r--   0        0        0     3373 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/tools/loader.py
+-rw-r--r--   0        0        0     9551 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/tools/model.py
+-rw-r--r--   0        0        0     3286 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/tools/register.py
+-rw-r--r--   0        0        0    10397 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/tools/schema.py
+-rw-r--r--   0        0        0     4233 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/sdk/utils.py
+-rw-r--r--   0        0        0     4848 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/task/__init__.py
+-rw-r--r--   0        0        0    22287 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/task/schema.py
+-rw-r--r--   0        0        0      219 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/task/snapshot/__init__.py
+-rw-r--r--   0        0        0      422 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/task/snapshot/_base.py
+-rw-r--r--   0        0        0     1237 2024-04-17 06:19:52.635193 llmkira-1.0.0/llmkira/task/snapshot/local.py
+-rw-r--r--   0        0        0     2835 2024-04-17 06:20:08.495237 llmkira-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1485 2024-04-17 06:19:52.635193 llmkira-1.0.0/tests/pydantic_error.py
+-rw-r--r--   0        0        0    10079 1970-01-01 00:00:00.000000 llmkira-1.0.0/PKG-INFO
```

### Comparing `llmkira-0.27.3/llmkira/extra/plugins/alarm/__init__.py` & `llmkira-1.0.0/llmkira/extra/plugins/alarm/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,206 +1,210 @@
 # -*- coding: utf-8 -*-
-
-
 __package__name__ = "llmkira.extra.plugins.alarm"
 __plugin_name__ = "set_alarm_reminder"
-__openapi_version__ = "20231111"
-
-from llmkira.sdk.func_calling import verify_openapi_version
-
-verify_openapi_version(__package__name__, __openapi_version__)
-
-from pydantic import field_validator, ConfigDict
-
-from llmkira.sdk.schema import Function
+__openapi_version__ = "20240416"
 
 import datetime
 import re
+from typing import Optional, Union, Type
 
-from loguru import logger
-from pydantic import BaseModel
+from llmkira.openai.cell import Tool, ToolCall, class_tool
+from llmkira.sdk.tools import verify_openapi_version
+from llmkira.sdk.utils import sync
+from llmkira.task.schema import Location, EventMessage, Sign, ToolResponse
 
-from llmkira.receiver.aps import SCHEDULER
-from llmkira.schema import RawMessage
-from llmkira.sdk.func_calling import PluginMetadata, BaseTool
-from llmkira.sdk.func_calling.schema import FuncPair
-from llmkira.task import Task, TaskHeader
-
-from typing import TYPE_CHECKING, Optional
-
-if TYPE_CHECKING:
-    from llmkira.sdk.schema import TaskBatch
-
-alarm = Function(name=__plugin_name__, description="Set a timed reminder (only for minutes)")
-alarm.add_property(
-    property_name="delay",
-    property_description="The delay time, in minutes",
-    property_type="integer",
-    required=True
-)
-alarm.add_property(
-    property_name="content",
-    property_description="reminder content",
-    property_type="string",
-    required=True
-)
+verify_openapi_version(__package__name__, __openapi_version__)  # noqa
+from llmkira.sdk.tools import PluginMetadata  # noqa
+from llmkira.sdk.tools.schema import FuncPair, BaseTool  # noqa
+from loguru import logger  # noqa
+from pydantic import BaseModel, Field  # noqa
+from pydantic import field_validator, ConfigDict  # noqa
+
+from app.receiver.aps import SCHEDULER  # noqa
+
+from llmkira.task import Task, TaskHeader  # noqa
+from pytz import utc  # noqa
 
 
-class Alarm(BaseModel):
-    delay: int
-    content: str
+class SetAlarm(BaseModel):
+    delay: int = Field(description="The delay time, in minutes")
+    content: str = Field(description="reminder content")
     model_config = ConfigDict(extra="allow")
 
     @field_validator("delay")
     def delay_validator(cls, v):
         if v < 0:
             raise ValueError("delay must be greater than 0")
         return v
 
 
-async def send_notify(_platform, _meta, _sender: dict, _receiver: dict, _user, _chat, _content: str):
-    await Task(queue=_platform).send_task(
-        task=TaskHeader(
-            sender=TaskHeader.Location.model_validate(_sender),  # 继承发送者
-            receiver=TaskHeader.Location.model_validate(_receiver),  # 因为可能有转发，所以可以单配
-            task_meta=TaskHeader.Meta.model_validate(_meta),
-            message=[
-                RawMessage(
-                    user_id=_user,
-                    chat_id=_chat,
-                    text=_content
-                )
-            ]
+def send_notify(
+    _platform, _meta, _sender: dict, _receiver: dict, _user, _chat, _content: str
+):
+    sync(
+        Task.create_and_send(
+            queue_name=_platform,
+            task=TaskHeader(
+                sender=Location.model_validate(_sender),  # 继承发送者
+                receiver=Location.model_validate(
+                    _receiver
+                ),  # 因为可能有转发，所以可以单配
+                task_sign=Sign.model_validate(_meta),
+                message=[EventMessage(user_id=_user, chat_id=_chat, text=_content)],
+            ),
         )
     )
 
 
 class AlarmTool(BaseTool):
     """
     搜索工具
     """
+
     silent: bool = False
-    function: Function = alarm
-    keywords: list = ["闹钟", "提醒", "定时", "到点", '分钟']
-    pattern: Optional[re.Pattern] = re.compile(r"(\d+)(分钟|小时|天|周|月|年)后提醒我(.*)")
+    function: Union[Tool, Type[BaseModel]] = SetAlarm
+    keywords: list = ["闹钟", "提醒", "定时", "到点", "分钟", "小时"]
+    pattern: Optional[re.Pattern] = re.compile(
+        r"(\d+)(分钟|小时|天|周|月|年)后提醒我(.*)"
+    )
     require_auth: bool = True
 
     # env_required: list = ["SCHEDULER", "TIMEZONE"]
 
-    def pre_check(self):
-        return True
-
     def func_message(self, message_text, **kwargs):
         """
         如果合格则返回message，否则返回None，表示不处理
         """
         for i in self.keywords:
             if i in message_text:
                 return self.function
         # 正则匹配
         if self.pattern:
             match = self.pattern.match(message_text)
             if match:
                 return self.function
         return None
 
-    async def failed(self,
-                     task: "TaskHeader", receiver: "TaskHeader.Location",
-                     exception,
-                     env: dict,
-                     arg: dict, pending_task: "TaskBatch", refer_llm_result: dict = None,
-                     **kwargs
-                     ):
-        _meta = task.task_meta.reply_notify(
+    async def failed(
+        self,
+        task: "TaskHeader",
+        receiver: "Location",
+        exception,
+        env: dict,
+        arg: dict,
+        pending_task: "ToolCall",
+        refer_llm_result: dict = None,
+        **kwargs,
+    ):
+        _meta = task.task_sign.notify(
             plugin_name=__plugin_name__,
-            callback=[TaskHeader.Meta.Callback.create(
-                name=__plugin_name__,
-                function_response=f"Timer Run Failed: {exception}",
-                tool_call_id=pending_task.get_batch_id()
-            )],
-            write_back=True,
-            release_chain=True
+            tool_response=[
+                ToolResponse(
+                    name=__plugin_name__,
+                    function_response=f"Timer Run Failed: {exception}",
+                    tool_call_id=pending_task.id,
+                    tool_call=pending_task,
+                )
+            ],
+            memory_able=True,
+            response_snapshot=True,
         )
-        await Task(queue=receiver.platform).send_task(
+        await Task.create_and_send(
+            queue_name=receiver.platform,
             task=TaskHeader(
                 sender=task.sender,
                 receiver=receiver,
-                task_meta=_meta,
+                task_sign=_meta,
                 message=[
-                    RawMessage(
+                    EventMessage(
                         user_id=receiver.user_id,
                         chat_id=receiver.chat_id,
-                        text=f"{__plugin_name__} Run failed {exception}"
+                        text=f"{__plugin_name__} Run failed {exception}",
                     )
-                ]
-            )
+                ],
+            ),
         )
 
-    async def callback(self,
-                       task: "TaskHeader", receiver: "TaskHeader.Location",
-                       env: dict,
-                       arg: dict, pending_task: "TaskBatch", refer_llm_result: dict = None,
-                       **kwargs
-                       ):
+    async def callback(
+        self,
+        task: "TaskHeader",
+        receiver: "Location",
+        env: dict,
+        arg: dict,
+        pending_task: "ToolCall",
+        refer_llm_result: dict = None,
+        **kwargs,
+    ):
         return None
 
-    async def run(self,
-                  task: "TaskHeader", receiver: "TaskHeader.Location",
-                  arg: dict, env: dict, pending_task: "TaskBatch", refer_llm_result: dict = None,
-                  ):
+    async def run(
+        self,
+        task: "TaskHeader",
+        receiver: "Location",
+        arg: dict,
+        env: dict,
+        pending_task: "ToolCall",
+        refer_llm_result: dict = None,
+    ):
         """
         处理message，返回message
         """
-        _set = Alarm.model_validate(arg)
-        _meta = task.task_meta.reply_message(
+        argument = SetAlarm.model_validate(arg)
+        _meta = task.task_sign.reply(
             plugin_name=__plugin_name__,
-            callback=[
-                TaskHeader.Meta.Callback.create(
+            tool_response=[
+                ToolResponse(
                     name=__plugin_name__,
                     function_response="Timer Run Success",
-                    tool_call_id=pending_task.get_batch_id()
+                    tool_call_id=pending_task.id,
+                    tool_call=pending_task,
                 )
-            ]
+            ],
         )
 
-        logger.debug("Plugin --set_alarm {} minutes".format(_set.delay))
+        logger.debug("Plugin --set_alarm {} minutes".format(argument.delay))
+        # 这里假设您的任务应该在UTC时间下执行，如果需要在其他时区执行，根据实际情况更改tz变量
+        tz = utc
+        run_time = datetime.datetime.now() + datetime.timedelta(minutes=argument.delay)
+        # 将本地时间转换为设定的时区
+        run_time = tz.localize(run_time)
         SCHEDULER.add_job(
             func=send_notify,
             id=receiver.uid,
             trigger="date",
             replace_existing=True,
             misfire_grace_time=1000,
-            run_date=datetime.datetime.now() + datetime.timedelta(minutes=_set.delay),
+            run_date=run_time,
             args=[
                 task.receiver.platform,
                 _meta.model_dump(),
-                task.sender.model_dump(), receiver.model_dump(),
-                receiver.user_id, receiver.chat_id,
-                _set.content
-            ]
+                task.sender.model_dump(),
+                receiver.model_dump(),
+                receiver.user_id,
+                receiver.chat_id,
+                argument.content,
+            ],
         )
         await Task(queue=receiver.platform).send_task(
             task=TaskHeader(
                 sender=task.sender,  # 继承发送者
                 receiver=receiver,  # 因为可能有转发，所以可以单配
-                task_meta=_meta,
+                task_sign=_meta,
                 message=[
-                    RawMessage(
+                    EventMessage(
                         user_id=receiver.user_id,
                         chat_id=receiver.chat_id,
-                        text=f"🍖 The alarm is now set,just wait for {_set.delay} min"
+                        text=f"🍖 The alarm is now set,just wait for {argument.delay} min",
                     )
-                ]
+                ],
             )
         )
 
 
 __plugin_meta__ = PluginMetadata(
     name=__plugin_name__,
     description="Set a timed reminder (only for minutes)",
     usage="直接说，以分钟为单位，如：10分钟后提醒我吃饭",
     openapi_version=__openapi_version__,
-    function={
-        FuncPair(function=alarm, tool=AlarmTool)
-    },
-    homepage="https://github.com/LlmKira"
+    function={FuncPair(function=class_tool(SetAlarm), tool=AlarmTool)},
+    homepage="https://github.com/LlmKira",
 )
```

### Comparing `llmkira-0.27.3/llmkira/extra/plugins/search.py` & `llmkira-1.0.0/llmkira/extra/plugins/search/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,53 @@
 # -*- coding: utf-8 -*-
+from typing import Union, Type, List
+
 from pydantic import ConfigDict
 
 __package__name__ = "llmkira.extra.plugins.search"
 __plugin_name__ = "search_in_google"
-__openapi_version__ = "20231111"
+__openapi_version__ = "20240416"
+
+from llmkira.sdk.tools import verify_openapi_version  # noqa: E402
+from pydantic import BaseModel, Field  # noqa: E402
 
-from llmkira.extra.user import CostControl, UserCost
-from llmkira.middleware.llm_provider import GetAuthDriver
-from llmkira.sdk import resign_plugin_executor
-from llmkira.sdk.endpoint import openai
-from llmkira.sdk.func_calling import verify_openapi_version
-
-verify_openapi_version(__package__name__, __openapi_version__)
-from loguru import logger  # noqa: E402
-from pydantic import BaseModel  # noqa: E402
-
-from llmkira.schema import RawMessage  # noqa: E402
-from llmkira.sdk.func_calling import BaseTool, PluginMetadata  # noqa: E402
-from llmkira.sdk.func_calling.schema import FuncPair  # noqa: E402
-from llmkira.sdk.schema import create_short_task, Function  # noqa: E402
+verify_openapi_version(__package__name__, __openapi_version__)  # noqa: E402
+from llmkira.openai.cell import Tool, ToolCall, class_tool  # noqa: E402
+from llmkira.openapi.fuse import resign_plugin_executor  # noqa: E402
+from llmkira.sdk.tools import PluginMetadata  # noqa: E402
+from llmkira.sdk.tools.schema import FuncPair, BaseTool  # noqa: E402
 from llmkira.task import Task, TaskHeader  # noqa: E402
-from typing import TYPE_CHECKING  # noqa: E402
+from llmkira.task.schema import Location, ToolResponse, EventMessage  # noqa: E402
+from .engine import SerperSearchEngine, build_search_tips  # noqa: E402
 
-if TYPE_CHECKING:
-    from llmkira.sdk.schema import TaskBatch
-search = Function(
-    name=__plugin_name__,
-    description="Search/validate on google.com.[ONLY IF NECESSARY]",
-).update_config(
-    config=Function.FunctionExtra(
-        system_prompt="Search only if necessary",
-    )
-)
-search.add_property(
-    property_name="keywords",
-    property_description="question entered in the search website",
-    property_type="string",
-    required=True,
-)
 
+class Search(BaseModel):
+    keywords: str = Field(description="question entered in the search website")
+    model_config = ConfigDict(extra="allow")
 
-@resign_plugin_executor(function=search)
-def search_on_duckduckgo(search_sentence: str, key_words: str = None):
-    logger.debug(f"Plugin --search_on_duckduckgo {search_sentence}")
-    from duckduckgo_search import DDGS
-
-    # 内存优化抛弃 NLP
-    # from llmkira.sdk.filter import Sublimate
-    sort_text = []
-    link_refer = {}
-    with DDGS(timeout=20) as ddgs:
-        search_result = ddgs.text(search_sentence)
-        for r in search_result:
-            _title = r.get("title")
-            _href = r.get("href")
-            _body = r.get("body")
-            link_refer[_body] = _href
-            sort_text.append((_body, _title, _href))
-    # must_key = [key_words] if key_words else None
-    sorted_result = sort_text
-    # sorted_result = Sublimate(sort_text).valuation(match_sentence=search_sentence, match_keywords=must_key)
-    valuable_result = [item[0] for item in sorted_result[:4]]
-    # 构建单条内容
-    clues = []
-    for key, item in enumerate(valuable_result):
-        clues.append(
-            f"\nPage #{key}\n🔍Contents:{item}\n"
-            f"🔗Source:{link_refer.get(item, 'https://google.com/')}\n"
-        )
-    content = "\n".join(clues)
-    return (
-        "[🔍SearchPage]\n"
-        + content
-        + (
-            "\n[Page End]"
-            "\n[ReplyFormat:`$summary_answer \n [$index]($source_link) * num` to mark links]"
-        )
-    )
+
+@resign_plugin_executor(tool=Search)
+async def search_on_serper(search_sentence: str, api_key: str):
+    result = await SerperSearchEngine(api_key=api_key).search(search_sentence)
+    return build_search_tips(search_items=result)
 
 
 class Search(BaseModel):
     keywords: str
     model_config = ConfigDict(extra="allow")
 
 
 class SearchTool(BaseTool):
     """
     搜索工具
     """
 
     silent: bool = False
-    function: Function = search
+    function: Union[Tool, Type[BaseModel]] = Search
+    require_auth: bool = True
     keywords: list = [
         "怎么",
         "How",
         "件事",
         "牢大",
         "作用",
         "知道",
@@ -136,26 +89,30 @@
         "搜索",
         "百度",
         "谷歌",
         "bing",
         "谁是",
         "上网",
     ]
+    env_required: List[str] = ["API_KEY"]
+    env_prefix: str = "SERPER_"
 
-    def pre_check(self):
-        try:
-            from duckduckgo_search import DDGS  # noqa: F401
-
-            # from llmkira.sdk.filter import Sublimate
-            return True
-        except ImportError as e:
-            logger.warning(
-                f"plugin:package <duckduckgo_search> not found,please install it first:{e}"
+    @classmethod
+    def env_help_docs(cls, empty_env: List[str]) -> str:
+        """
+        Provide help message for environment variables
+        :param empty_env: The environment variable list that not configured
+        :return: The help message
+        """
+        message = ""
+        if "SERPER_API_KEY" in empty_env:
+            message += (
+                "You need to configure https://serper.dev/ to start use this tool"
             )
-            return False
+        return message
 
     def func_message(self, message_text, **kwargs):
         """
         如果合格则返回message，否则返回None，表示不处理
         """
         for i in self.keywords:
             if i in message_text:
@@ -166,131 +123,110 @@
             if match:
                 return self.function
         return None
 
     async def failed(
         self,
         task: "TaskHeader",
-        receiver: "TaskHeader.Location",
+        receiver: "Location",
         exception,
         env: dict,
         arg: dict,
-        pending_task: "TaskBatch",
+        pending_task: "ToolCall",
         refer_llm_result: dict = None,
         **kwargs,
     ):
-        _meta = task.task_meta.reply_notify(
+        meta = task.task_sign.notify(
             plugin_name=__plugin_name__,
-            callback=[
-                TaskHeader.Meta.Callback.create(
+            tool_response=[
+                ToolResponse(
                     name=__plugin_name__,
                     function_response=f"Run Failed {exception}",
-                    tool_call_id=pending_task.get_batch_id(),
+                    tool_call_id=pending_task.id,
+                    tool_call=pending_task,
                 )
             ],
-            write_back=True,
-            release_chain=True,
+            memory_able=True,
+            response_snapshot=True,
         )
-        await Task(queue=receiver.platform).send_task(
+        await Task.create_and_send(
+            queue_name=receiver.platform,
             task=TaskHeader(
                 sender=task.sender,
                 receiver=receiver,
-                task_meta=_meta,
+                task_sign=meta,
                 message=[
-                    RawMessage(
+                    EventMessage(
                         user_id=receiver.user_id,
                         chat_id=receiver.chat_id,
                         text=f"🍖{__plugin_name__} Run Failed：{exception}",
                     )
                 ],
-            )
+            ),
         )
 
-    @staticmethod
-    async def llm_task(plugin_name, task: TaskHeader, task_desc: str, raw_data: str):
-        assert task_desc == raw_data, "STOP USE THE FUNCTION"
-        # TODO: 转换为通用
-        logger.info("llm_tool:{}".format(task_desc))
-        auth_client = GetAuthDriver(uid=task.sender.uid)
-        driver = await auth_client.get()
-        endpoint = openai.Openai.init(
-            driver=driver,
-            temperature=0.1,
-            messages=create_short_task(task_desc=task_desc, refer=raw_data),
-        )
-        # 调用Openai
-        result = await endpoint.create()
-        # 记录消耗
-        await CostControl.add_cost(
-            cost=UserCost.create_from_function(
-                uid=task.sender.uid,
-                request_id=result.id,
-                cost_by=plugin_name,
-                token_usage=result.usage.total_tokens,
-                token_uuid=driver.uuid,
-                model_name=driver.model,
-            )
-        )
-        assert result.default_message.content, "llm_task.py:llm_task:content is None"
-        return result.default_message.content
-
     async def callback(
         self,
         task: "TaskHeader",
-        receiver: "TaskHeader.Location",
+        receiver: "Location",
         env: dict,
         arg: dict,
-        pending_task: "TaskBatch",
+        pending_task: "ToolCall",
         refer_llm_result: dict = None,
         **kwargs,
     ):
         return True
 
     async def run(
         self,
         task: "TaskHeader",
-        receiver: "TaskHeader.Location",
+        receiver: "Location",
         arg: dict,
         env: dict,
-        pending_task: "TaskBatch",
+        pending_task: "ToolCall",
         refer_llm_result: dict = None,
     ):
         """
         处理message，返回message
         """
 
         _set = Search.model_validate(arg)
-        _search_result = search_on_duckduckgo(_set.keywords)
+        _search_result = await search_on_serper(
+            search_sentence=_set.keywords,
+            api_key=env.get("serper_api_key"),
+        )
         # META
-        _meta = task.task_meta.reply_raw(
+        _meta = task.task_sign.reprocess(
             plugin_name=__plugin_name__,
-            callback=[
-                TaskHeader.Meta.Callback.create(
+            tool_response=[
+                ToolResponse(
                     name=__plugin_name__,
                     function_response=str(_search_result),
-                    tool_call_id=pending_task.get_batch_id(),
+                    tool_call_id=pending_task.id,
+                    tool_call=pending_task,
                 )
             ],
         )
-        await Task(queue=receiver.platform).send_task(
+        await Task.create_and_send(
+            queue_name=receiver.platform,
             task=TaskHeader(
                 sender=task.sender,  # 继承发送者
                 receiver=receiver,  # 因为可能有转发，所以可以单配
-                task_meta=_meta,
+                task_sign=_meta,
                 message=[
-                    RawMessage(
+                    EventMessage(
                         user_id=receiver.user_id,
                         chat_id=receiver.chat_id,
                         text="🔍 Searching Done",
                     )
                 ],
-            )
+            ),
         )
 
 
 __plugin_meta__ = PluginMetadata(
     name=__plugin_name__,
     description="Search fact on google.com",
     usage="以问号结尾的句子即可触发",
     openapi_version=__openapi_version__,
-    function={FuncPair(function=search, tool=SearchTool)},
+    function={FuncPair(function=class_tool(Search), tool=SearchTool)},
 )
```

### Comparing `llmkira-0.27.3/llmkira/sdk/cache/__init__.py` & `llmkira-1.0.0/llmkira/cache/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,118 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2023/7/10 下午9:42
-# @Author  : sudoskys
-# @File    : __init__.py.py
-# @Software: PyCharm
 import os
+import pathlib
 from typing import Optional
 
 from dotenv import load_dotenv
 from loguru import logger
 
-from .base import singleton, BaseRuntime
-from .mongo import MongoClientWrapper
-from .redis import RedisClientWrapper
-from ..utils import sync
+from .elara_runtime import ElaraClientAsyncWrapper
+from .redis_runtime import RedisClientWrapper
+from .runtime_schema import singleton, BaseRuntime
 
 
 @singleton
-class MongodbRuntime(BaseRuntime):
-    client: Optional["MongoClientWrapper"] = None
+class ElaraRuntime(BaseRuntime):
+    client: Optional["ElaraClientAsyncWrapper"] = None
     init_already = False
     dsn = None
 
     @staticmethod
-    def check_mongodb_dsn(dsn):
-        client = MongoClientWrapper(dsn)
-        assert sync(client.ping()), f"MongoDB {dsn} Disconnect"
+    def check_client_dsn(dsn):
+        """
+        :raise ValueError: Please Use Local Path
+        """
+        if "://" in dsn:
+            raise ValueError("Please Use Local Path")
+
+    def check_client(self):
+        if self.dsn is None:
+            pathlib.Path().cwd().joinpath(".cache").mkdir(exist_ok=True)
+            self.dsn = pathlib.Path().cwd().joinpath(".cache") / "elara.db"
+        self.client = ElaraClientAsyncWrapper(str(self.dsn))
+        logger.debug(f"🍩 ElaraClientWrapper Loaded --dsn {self.dsn}")
+        return True
 
-    def check_mongodb(self):
-        load_dotenv()
-        self.dsn = os.getenv('MONGODB_DSN', "mongodb://admin:8a8a8a@localhost:27017/?authSource=admin")
-        try:
-            self.check_mongodb_dsn(self.dsn)
-        except Exception as e:
-            logger.error(f'\n⚠️ Mongodb DISCONNECT, pls set MONGODB_DSN in .env\n--error {e} \n--dsn {self.dsn}')
-            raise e
-        else:
-            logger.success(f'🍩 MongoClientWrapper Loaded --dsn {self.dsn}')
-            self.client = MongoClientWrapper(self.dsn)
-            if "mongodb://admin:8a8a8a@" in self.dsn:
-                logger.warning(
-                    f"\n⚠️ You Are Using The Default MongoDB Password"
-                    f"\nMake Sure You Handle The Port `27017` And Set Firewall Rules"
-                )
-
-    def init_mongodb(self,
-                     verbose=False):
+    def init_client(self, verbose=False):
         if verbose:
-            logger.info("Try To Connect To MongoDb")
-        self.check_mongodb()
+            logger.info("Try To Connect To ElaraClient")
+        self.check_client()
         self.init_already = True
-        assert isinstance(self.client, MongoClientWrapper), f"MongoDb type error {type(self.client)}"
+        assert isinstance(
+            self.client, ElaraClientAsyncWrapper
+        ), f"ElaraClient type error {type(self.client)}"
         return self.client
 
-    def get_mongodb(self) -> "MongoClientWrapper":
+    def get_client(self) -> "ElaraClientAsyncWrapper":
         if not self.init_already:
-            self.init_mongodb()
-            assert isinstance(self.client, MongoClientWrapper), f"MongoDb error {type(self.client)}"
+            self.init_client()
+            assert isinstance(
+                self.client, ElaraClientAsyncWrapper
+            ), f"ElaraClient error {type(self.client)}"
         else:
-            assert isinstance(self.client, MongoClientWrapper), f"Inited MongoDb error {type(self.client)}"
+            assert isinstance(
+                self.client, ElaraClientAsyncWrapper
+            ), f"Inited ElaraClient error {type(self.client)}"
         return self.client
 
 
 @singleton
 class RedisRuntime(BaseRuntime):
     client: Optional["RedisClientWrapper"] = None
     init_already = False
     dsn = None
 
     @staticmethod
-    def check_redis_dsn(dsn):
+    def check_client_dsn(dsn):
         import redis
+
         r = redis.from_url(dsn)
         assert r.ping() is True
 
-    def check_redis(self):
+    def check_client(self):
         load_dotenv()
-        self.dsn = os.getenv('REDIS_DSN', 'redis://localhost:6379/0')
+        self.dsn = os.getenv("REDIS_DSN", "redis://localhost:6379/0")
         try:
-            self.check_redis_dsn(self.dsn)
+            self.check_client_dsn(self.dsn)
         except Exception as e:
-            logger.error(f'\n⚠️ Redis Disconnect, Please set `REDIS_DSN` env  --error {e} --dsn {self.dsn}')
-            raise e
+            logger.debug(
+                f"\n⚠️ Redis Disconnect, Please set `REDIS_DSN` env  --error {e} --dsn {self.dsn}"
+            )
+            return False
         else:
-            logger.success(f'🍩 RedisClientWrapper Loaded --dsn {self.dsn}')
+            logger.debug(f"🍩 RedisClientWrapper Loaded --dsn {self.dsn}")
             self.client = RedisClientWrapper(self.dsn)
-            if self.dsn == 'redis://localhost:6379/0':
-                logger.warning("\n⚠️ You are using a non-password-protected local REDIS database.")
+            if self.dsn == "redis://localhost:6379/0":
+                logger.warning(
+                    "\n⚠️ You are using a non-password-protected local REDIS database."
+                )
+            return True
 
-    def init_cache(self,
-                   verbose=False) -> "RedisClientWrapper":
+    def init_client(self, verbose=False) -> "RedisClientWrapper":
         if verbose:
             logger.info("Try To Connect To Cache")
-        self.check_redis()
+        self.check_client()
         self.init_already = True
-        assert isinstance(self.client, RedisClientWrapper), f"Cache type error {type(self.client)}"
+        assert isinstance(
+            self.client, RedisClientWrapper
+        ), f"Cache type error {type(self.client)}"
         return self.client
 
-    def get_redis(self) -> "RedisClientWrapper":
+    def get_client(self) -> "RedisClientWrapper":
         if not self.init_already:
-            self.init_cache()
-            assert isinstance(self.client, RedisClientWrapper), f"Cache type error {type(self.client)}"
+            self.init_client()
+            assert isinstance(
+                self.client, RedisClientWrapper
+            ), f"Cache type error {type(self.client)}"
         else:
-            assert isinstance(self.client, RedisClientWrapper), f"Inited cache type error {type(self.client)}"
+            assert isinstance(
+                self.client, RedisClientWrapper
+            ), f"Inited cache type error {type(self.client)}"
         return self.client
 
 
-global_cache_runtime: RedisRuntime = RedisRuntime()
-global_mongodb_runtime: MongodbRuntime = MongodbRuntime()
+if RedisRuntime().check_client():
+    global_cache_runtime: BaseRuntime = RedisRuntime()
+else:
+    global_cache_runtime: BaseRuntime = ElaraRuntime()
```

### Comparing `llmkira-0.27.3/llmkira/sdk/cache/base.py` & `llmkira-1.0.0/llmkira/cache/runtime_schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2023/7/10 下午9:43
-# @Author  : sudoskys
-# @File    : base.py
-# @Software: PyCharm
 from abc import abstractmethod, ABC
 from typing import Any
 
-PREFIX = 'base_bot:'
+PREFIX = "oai_bot:"
 
 
 def singleton(cls):
     _instance = {}
 
     def _singleton(*args, **kargs):
         if cls not in _instance:
@@ -21,25 +18,37 @@
 
 
 class BaseRuntime(ABC):
     init_already = False
     client = None
     dsn = None
 
+    @staticmethod
+    def check_client_dsn(dsn):
+        raise NotImplementedError
 
-class AbstractDataClass(ABC):
+    def check_client(self) -> bool:
+        raise NotImplementedError
+
+    def init_client(self, verbose=False):
+        raise NotImplementedError
+
+    def get_client(self) -> "AbstractDataClass":
+        raise NotImplementedError
 
+
+class AbstractDataClass(ABC):
     @abstractmethod
     async def ping(self):
         return True
 
     @abstractmethod
     def update_backend(self, backend):
         pass
 
     @abstractmethod
-    async def set_data(self, key: str, value: Any, **kwargs) -> Any:
+    async def set_data(self, key: str, value: Any, timeout: int = None) -> Any:
         pass
 
     @abstractmethod
     async def read_data(self, key: str) -> Any:
         pass
```

### Comparing `llmkira-0.27.3/llmkira/sdk/cache/redis.py` & `llmkira-1.0.0/llmkira/cache/redis_runtime.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2023/7/10 下午9:43
-# @Author  : sudoskys
-# @File    : redis.py
-# @Software: PyCharm
 import json
-from typing import Optional, Tuple, List, Union
+from typing import Optional, Union
 
 import redis
 from loguru import logger
 from redis.asyncio.client import Redis
 from redis.asyncio.connection import ConnectionPool
 
-from .base import AbstractDataClass, PREFIX
+from .runtime_schema import AbstractDataClass, PREFIX
 
 
 class RedisClientWrapper(AbstractDataClass):
     """
     Redis 数据类
     """
 
@@ -42,38 +39,8 @@
     async def read_data(self, key) -> Optional[Union[str, dict, int]]:
         data = await self._redis.get(self.prefix + str(key))
         if data is not None:
             try:
                 data = json.loads(data)
             except Exception as ex:
                 logger.trace(ex)
-                pass
         return data
-
-    async def lpush_data(self, key, value):
-        """
-        从左侧插入数据
-        :param key: str
-        :param value: json
-        """
-        # 验证是否可以被json序列化
-        if isinstance(value, (dict, list)):
-            value = json.dumps(value)
-        return await self._redis.lpush(self.prefix + str(key), value)
-
-    async def lpop_data(self, key) -> Optional[dict]:
-        _data = await self._redis.lpop(self.prefix + str(key))
-        if _data:
-            _data = _data.decode("utf-8")
-            try:
-                _data = json.loads(_data)
-            except json.JSONDecodeError:
-                pass
-            return _data
-        return None
-
-    async def lrange_data(self, key, start_end: Tuple[int, int] = (0, -1)) -> List[str]:
-        _items = await self._redis.lrange(
-            self.prefix + str(key), start=start_end[0], end=start_end[1]
-        )
-        items = [m.decode("utf-8") for m in _items[::-1]]
-        return items
```

### Comparing `llmkira-0.27.3/llmkira/sdk/filter/api/LICENSE` & `llmkira-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmkira-0.27.3/llmkira/sdk/filter/langdetect_fasttext/LICENSE` & `llmkira-1.0.0/llmkira/memory/redis_storage/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
+The MIT License
 
-Copyright (c) 2021 Zafer Çavdar
+Copyright (c) Harrison Chase
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `llmkira-0.27.3/llmkira/sdk/filter/langdetect_unicode/LICENSE` & `llmkira-1.0.0/llmkira/sdk/tools/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 mudssky
+Copyright (c) 2020 NoneBot Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `llmkira-0.27.3/llmkira/sdk/func_calling/__init__.py` & `llmkira-1.0.0/llmkira/sdk/tools/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,40 +20,36 @@
 
 
 class FrameworkInfo(BaseModel):
     support: bool
     exception: Optional[str] = None
 
 
-_current_openapi_version_: str = "20231111"
+_current_openapi_version_: str = "20240416"
 _openapi_version_: Dict[str, "FrameworkInfo"] = {
-    _current_openapi_version_: FrameworkInfo(
-        support=True,
-        exception=None
+    _current_openapi_version_: FrameworkInfo(support=True, exception=None),
+    "20231111": FrameworkInfo(
+        support=False, exception="Broken Changes in ver.20231111,pls refer docs"
     ),
-    "20231027": FrameworkInfo(
-        support=False,
-        exception="Broken Changes in ver.20231111,pls refer docs"
-    )
 }
 
 
 def verify_openapi_version(name: str, openapi_version: str):
     """
     验证框架接口版本
     """
     if not openapi_version:
         return None
     frame = _openapi_version_.get(openapi_version, None)
     if not frame:
         raise OpenApiError(
-            f"OpenApiError:Plugin<{name}> --error {openapi_version} not support")
+            f"OpenApiError:Plugin<{name}> --error {openapi_version} not support"
+        )
     if not frame.support:
-        raise OpenApiError(
-            f"OpenApiError:Plugin<{name}> --error {frame.exception}")
+        raise OpenApiError(f"OpenApiError:Plugin<{name}> --error {frame.exception}")
 
 
 def path_to_module_name(path: Path) -> str:
     rel_path = path.resolve().relative_to(Path("").resolve())
     if rel_path.stem == "__init__":
         return ".".join(rel_path.parts[:-1])
     else:
@@ -74,14 +70,15 @@
 def get_loaded_plugins() -> Set["Plugin"]:
     """获取当前已导入的所有插件。"""
     return set(_plugins.values())
 
 
 def get_entrypoint_plugins(group="llmkira.extra.plugin") -> Set[str]:
     import importlib_metadata
+
     hook = importlib_metadata.entry_points().select(group=group)
     plugins = [item.module for item in hook]
     return {*plugins}
 
 
 def get_available_plugin_names() -> Set[str]:
     """获取当前所有可用的插件名（包含尚未加载的插件）。"""
@@ -94,15 +91,17 @@
             return manager
 
 
 def _module_name_to_plugin_name(module_name: str) -> str:
     return module_name.rsplit(".", 1)[-1]
 
 
-def _new_plugin(module_name: str, module: ModuleType, manager: "PluginManager") -> "Plugin":
+def _new_plugin(
+    module_name: str, module: ModuleType, manager: "PluginManager"
+) -> "Plugin":
     """
     Create a new plugin
     """
     plugin_name = _module_name_to_plugin_name(module_name)
     if plugin_name in _plugins:
         raise RuntimeError("Plugin already exists! Check your plugin name.")
     plugin = Plugin(plugin_name, module, module_name, manager)
@@ -120,22 +119,20 @@
         raise RuntimeError("Plugin not found!")
     del _plugins[plugin.name]
     parent_plugin = plugin.parent_plugin
     if parent_plugin:
         parent_plugin.sub_plugins.remove(plugin)
 
 
-from .loader import PluginManager
-from .schema import Plugin as Plugin, BaseTool
-from .loader import require as require
-from .loader import load_plugin as load_plugin
-from .loader import load_plugins as load_plugins
-from .loader import load_all_plugins as load_all_plugins
-from .loader import load_builtin_plugin as load_builtin_plugin
-from .loader import load_builtin_plugins as load_builtin_plugins
-from .loader import load_from_entrypoint as load_from_entrypoint
-from .loader import PluginManager as PluginManager
-
-from .model import Plugin as Plugin
-from .model import PluginMetadata as PluginMetadata
-
-from .register import ToolRegister as ToolRegister
+from .loader import PluginManager  # noqa 402
+from .schema import Plugin as Plugin  # noqa 402
+from .loader import require as require  # noqa 402
+from .loader import load_plugin as load_plugin  # noqa 402
+from .loader import load_plugins as load_plugins  # noqa 402
+from .loader import load_all_plugins as load_all_plugins  # noqa 402
+from .loader import load_builtin_plugin as load_builtin_plugin  # noqa 402
+from .loader import load_builtin_plugins as load_builtin_plugins  # noqa 402
+from .loader import load_from_entrypoint as load_from_entrypoint  # noqa 402
+from .loader import PluginManager as PluginManager  # noqa 402
+from .model import Plugin as Plugin  # noqa 402
+from .model import PluginMetadata as PluginMetadata  # noqa 402
+from .register import ToolRegister as ToolRegister  # noqa 402
```

### Comparing `llmkira-0.27.3/llmkira/sdk/func_calling/loader.py` & `llmkira-1.0.0/llmkira/sdk/tools/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,25 @@
 from types import ModuleType
 from typing import Optional, Set, Iterable, Union
 
 from . import (
     _managers,
     _current_plugin_chain,
     _module_name_to_plugin_name,
-    path_to_module_name, _find_manager_by_name, get_plugin,
+    path_to_module_name,
+    _find_manager_by_name,
+    get_plugin,
 )
 from .model import PluginManager
 from .schema import Plugin
 
 
-def load_all_plugins(module_path: Iterable[str], plugin_dir: Iterable[str]) -> Set[Plugin]:
+def load_all_plugins(
+    module_path: Iterable[str], plugin_dir: Iterable[str]
+) -> Set[Plugin]:
     """
     导入指定列表中的插件以及指定目录下多个插件，以 `_` 开头的插件不会被导入!
     :param module_path: 指定插件集合
     :param plugin_dir: 指定文件夹路径集合
     """
     manager = PluginManager(module_path, plugin_dir)
     _managers.append(manager)
@@ -66,14 +70,15 @@
     manager = PluginManager([module_path])
     _managers.append(manager)
     return manager.load_plugin(module_path)
 
 
 def load_from_entrypoint(group="llmkira.extra.plugin") -> Set[Plugin]:
     import importlib_metadata
+
     hook = importlib_metadata.entry_points().select(group=group)
     plugins = [item.module for item in hook]
     return load_all_plugins(plugins, [])
 
 
 def require(name: str) -> ModuleType:
     """
```

### Comparing `llmkira-0.27.3/llmkira/sdk/func_calling/model.py` & `llmkira-1.0.0/llmkira/sdk/tools/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,32 +17,32 @@
 
 from . import (
     _managers,
     _new_plugin,
     _revert_plugin,
     _current_plugin_chain,
     _module_name_to_plugin_name,
-    path_to_module_name
+    path_to_module_name,
 )
 from .error import escape_tag, OpenApiError
 from .schema import Plugin, PluginMetadata
 
 
 class PluginManager:
     """插件管理器。
 
     参数:
         plugins: 独立插件模块名集合。
         search_path: 插件搜索路径（文件夹）。
     """
 
     def __init__(
-            self,
-            plugins: Optional[Iterable[str]] = None,
-            search_path: Optional[Iterable[str]] = None,
+        self,
+        plugins: Optional[Iterable[str]] = None,
+        search_path: Optional[Iterable[str]] = None,
     ):
         # simple plugin not in search path
         self.plugins: Set[str] = set(plugins or [])
         self.search_path: Set[str] = set(search_path or [])
 
         # cache plugins
         self._third_party_plugin_names: Dict[str, str] = {}
@@ -98,17 +98,17 @@
         # check plugins in search path
         for module_info in pkgutil.iter_modules(self.search_path):
             # ignore if startswith "_"
             if module_info.name.startswith("_"):
                 continue
 
             if (
-                    module_info.name in searched_plugins
-                    or module_info.name in previous_plugins
-                    or module_info.name in third_party_plugins
+                module_info.name in searched_plugins
+                or module_info.name in previous_plugins
+                or module_info.name in third_party_plugins
             ):
                 raise RuntimeError(
                     f"Plugin already exists: {module_info.name}! Check your plugin name"
                 )
             #
             module_spec = module_info.module_finder.find_spec(module_info.name, None)
             if not module_spec:
@@ -170,44 +170,43 @@
     @property
     def searched_plugin_names(self):
         return self._searched_plugin_names
 
 
 class PluginFinder(MetaPathFinder):
     def find_spec(
-            self,
-            fullname: str,
-            path: Optional[Sequence[str]],
-            target: Optional[ModuleType] = None,
+        self,
+        fullname: str,
+        path: Optional[Sequence[str]],
+        target: Optional[ModuleType] = None,
     ):
         if _managers:
             module_spec = PathFinder.find_spec(fullname, path, target)
             if not module_spec:
                 return
             module_origin = module_spec.origin
             if not module_origin:
                 return
             module_path = Path(module_origin).resolve()
 
             for manager in reversed(_managers):
                 # use path instead of name in case of submodule name conflict
                 if (
-                        fullname in manager.plugins
-                        or module_path in manager.searched_plugin_names.values()
+                    fullname in manager.plugins
+                    or module_path in manager.searched_plugin_names.values()
                 ):
                     # print("find_spec",manager, fullname, module_origin)
                     # print(f"module_origin:{module_origin}")
                     module_spec.loader = PluginLoader(manager, fullname, module_origin)
                     return module_spec
         return
 
 
 class PluginLoader(SourceFileLoader):
-    def __init__(self,
-                 manager: PluginManager, fullname: str, path) -> None:
+    def __init__(self, manager: PluginManager, fullname: str, path) -> None:
         self.manager = manager
         self.loaded = False
         super().__init__(fullname, path)
 
     def create_module(self, spec) -> Optional[ModuleType]:
         # check self.name in sys.modules to avoid import loop
         if self.name in sys.modules:
```

### Comparing `llmkira-0.27.3/llmkira/sdk/func_calling/register.py` & `llmkira-1.0.0/llmkira/sdk/tools/register.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 # @File    : func_call.py
 # @Software: PyCharm
 import threading
 from typing import List, Dict
 from typing import Optional, Type
 from typing import TYPE_CHECKING
 
-from llmkira.sdk.func_calling import PluginMetadata
-from . import _openapi_version_, BaseTool, get_loaded_plugins, Plugin, get_plugin
-from .schema import FuncPair
-from ..schema import Function, File
+from llmkira.kv_manager.file import File
+from llmkira.openai.cell import Tool
+from llmkira.sdk.tools import PluginMetadata
+from llmkira.sdk.tools import _openapi_version_, get_loaded_plugins
+from llmkira.sdk.tools.schema import FuncPair, BaseTool
 
 if TYPE_CHECKING:
-    from ...schema import RawMessage
+    from ...task.schema import EventMessage
 
 threading_lock = threading.Lock()
 
 
 class ToolRegister(object):
     """
     扩展对 _plugins 字段的操作,需要实例化以获取数据
@@ -37,44 +38,48 @@
                 self.pair_function[sub_item.name] = sub_item
 
     def get_tool(self, name: str) -> Optional[Type[BaseTool]]:
         if not self.pair_function.get(name, None):
             return None
         return self.pair_function[name].tool
 
-    def get_plugin(self, name: str) -> Optional[Plugin]:
-        return get_plugin(name)
-
     @property
     def get_plugins_meta(self) -> List[PluginMetadata]:
         return [item.metadata for item in get_loaded_plugins() if item.metadata]
 
     @property
-    def functions(self) -> Dict[str, Function]:
-        _item: Dict[str, Function] = {}
+    def tools(self) -> Dict[str, Tool]:
+        """
+        Return the tools schema
+        """
+        _item: Dict[str, Tool] = {}
         for item in self.plugins:
             for sub_item in item.metadata.function:
                 _item[sub_item.name] = sub_item.function
         return _item
 
     @property
-    def tools(self) -> List[Type[BaseTool]]:
+    def tools_runtime(self) -> List[Type[BaseTool]]:
+        """
+        Return the tools runtime
+        """
         _item: List[Type[BaseTool]] = []
         for item in self.plugins:
             for sub_item in item.metadata.function:
                 _item.append(sub_item.tool)
         return _item
 
-    def filter_pair(self,
-                    key_phrases: str,
-                    message_raw: "RawMessage" = None,
-                    file_list: List[File] = None,
-                    address: tuple = None,
-                    ignore: List[str] = None
-                    ) -> List[Function]:
+    def filter_pair(
+        self,
+        key_phrases: str,
+        message_raw: "EventMessage" = None,
+        file_list: List[File] = None,
+        address: tuple = None,
+        ignore: List[str] = None,
+    ) -> List[Tool]:
         """
         过滤group中的函数
         """
         if ignore is None:
             ignore = []
         if file_list is None:
             file_list = []
@@ -84,18 +89,17 @@
             for file in _file_list:
                 if _tool.file_match_required.match(file.file_name):
                     return True
             return False
 
         for func_name, pair_cls in self.pair_function.items():
             _tool_cls = pair_cls.tool()
-            if _tool_cls.func_message(message_text=key_phrases,
-                                      message_raw=message_raw,
-                                      address=address
-                                      ):
+            if _tool_cls.func_message(
+                message_text=key_phrases, message_raw=message_raw, address=address
+            ):
                 # 关键词大类匹配成功
                 if func_name in ignore:
                     continue  # 忽略函数
                 if _tool_cls.file_match_required:
                     if not _match_file(_tool_cls, file_list):
                         continue
                 function_list.append(pair_cls.function)
```

### Comparing `llmkira-0.27.3/llmkira/sdk/func_calling/schema.py` & `llmkira-1.0.0/llmkira/sdk/tools/schema.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,243 +1,277 @@
 # -*- coding: utf-8 -*-
 import os
 import re
 from abc import abstractmethod, ABC
 from dataclasses import dataclass, field
 from types import ModuleType
-from typing import Optional, Type, Dict, Any, List, Union, Set, final, Literal
+from typing import Optional, Type, Dict, Any, List, Union, Set, final
 from typing import TYPE_CHECKING
 
 from loguru import logger
-from pydantic import field_validator, BaseModel, Field, model_validator, PrivateAttr
+from pydantic import field_validator, BaseModel, Field, model_validator
+
+from llmkira.openai.cell import Tool, ToolCall
+from llmkira.openai.request import OpenAIResult
 
 if TYPE_CHECKING:
-    from ...task import TaskHeader
-    from ..schema import Function, TaskBatch
+    from llmkira.task.schema import TaskHeader, Location
     from .model import PluginManager
 
 
 class BaseTool(ABC, BaseModel):
     """
     基础工具类，所有工具类都应该继承此类
     """
 
     __slots__ = ()
-    silent: bool = Field(False, description="是否静默")
-    function: "Function" = Field(..., description="功能")
-    keywords: List[str] = Field([], description="关键词")
-    pattern: Optional[re.Pattern] = Field(None, description="正则匹配")
-    require_auth: bool = Field(False, description="是否需要授权")
-    repeatable: bool = Field(False, description="是否可重复使用")
-    deploy_child: Literal[0, 1] = Field(1, description="如果为0，终结于此链点，不再向下传递")
-    require_auth_kwargs: dict = {}
+    silent: bool = False
+    """If True, the tool will not be displayed in the help message"""
+
+    function: Union[Tool, Type[BaseModel]]
+    """The function schema to be executed"""
+
+    @final
+    @field_validator("function", mode="after")
+    def _check_function(cls, v):
+        if issubclass(v, BaseModel):
+            v = Tool(function=v)
+        elif isinstance(v, Tool):
+            pass
+        else:
+            raise ValueError(f"function must be Tool or BaseModel, got {type(v)}")
+        return v
+
+    keywords: List[str] = []
+    """The keyword list to be matched to load tools in session"""
+
+    @final
+    @field_validator("keywords")
+    def _check_keywords(cls, v):
+        for i in v:
+            if len(i) < 2:
+                logger.warning(f"keyword should be more than 2 characters, got {i}")
+        return v
+
+    pattern: Optional[re.Pattern] = None
+    """The pattern to be matched to load tools in session"""
+
+    require_auth: bool = False
+    """Is user authentication required"""
+
     env_required: List[str] = Field([], description="环境变量要求,ALSO NEED env_prefix")
+    """Pre-required environment variables, you should provide env_prefix"""
+
     env_prefix: str = Field("", description="环境变量前缀")
-    file_match_required: Optional[re.Pattern] = Field(None, description="re.compile 文件名正则")
-    extra_arg: Dict[Any, Any] = Field({}, description="额外参数")
-    __run_arg: Dict[Any, Any] = PrivateAttr(default_factory=dict)
+    """Environment variable prefix"""
 
-    # exp: re.compile(r"file_id=([a-z0-9]{8})")
+    file_match_required: Optional[re.Pattern] = Field(
+        None, description="re.compile 文件名正则"
+    )
+    """File name regular expression to use the tool, exp: re.compile(r"file_id=([a-z0-9]{8})")"""
 
     @final
     def get_os_env(self, env_name):
         """
-        获取 PLUGIN_+ 公共环境变量
+        Get environment variables from os.environ
         """
         env = os.getenv("PLUGIN_" + env_name, None)
         return env
 
     @final
     @property
     def env_list(self):
         """
-        #🍪# If you think its shouldnt be final, you can issue it.
+        Return the env_prefix+env_name list
+        #🍪# If you think its cant be final, you can issue it.
         """
-        return [f"{self.env_prefix}{i}" for i in self.env_required]
+        return [f"{self.env_prefix}{env_name}" for env_name in self.env_required]
 
     @final
     @property
     def name(self):
         """
-        工具名称
+        Tool name
         """
-        return self.function.name
+        return self.function.function.name
 
     @final
     @model_validator(mode="after")
     def _check_conflict(self):
         if self.silent and self.env_required:
             # raise ValueError("silent and env_required can not be True at the same time")
             logger.warning(
                 "\n Plugin `silent` And `env_required` Should Not Be True Same Time"
                 "Please Validate `env_required` In Execute Manual, Or Provide Callback To User Instead"
             )
         if self.env_required and not self.env_prefix:
             raise ValueError("env_required must be used with env_prefix")
         return self
 
-    @final
-    @field_validator("keywords", mode="before")
-    def _check_keywords(cls, v):
-        for i in v:
-            if not isinstance(i, str):
-                raise ValueError(f"keyword must be str, got {type(i)}")
-            if len(i) > 20:
-                raise ValueError(f"keyword must be less than 20 characters, got {len(i)}")
-            if len(i) < 2:
-                raise ValueError(f"keyword must be more than 2 characters, got {len(i)}")
-        return v
-
     @classmethod
-    def env_help_docs(cls, empty_env: List[str]) -> str:
+    def env_help_docs(cls, empty_env: List[str]) -> Optional[str]:
         """
-        环境变量帮助文档
-        :param empty_env: 未被配置的环境变量列表
-        :return: 帮助文档/警告
+        Provide help message for environment variables
+        :param empty_env: The environment variable list that not configured
+        :return: The help message or None
         """
         assert isinstance(empty_env, list), "empty_env must be list"
+        if not empty_env:
+            return None
         return "You need to configure ENV to start use this tool"
 
     @abstractmethod
-    def pre_check(self) -> Union[bool, str]:
-        """
-        预检查，如果不合格则返回 False，合格则返回 True
-        返回字符串表示不合格，且有原因
-        """
-        return ...
-
-    @abstractmethod
     def func_message(self, message_text, **kwargs):
         """
-        如果合格则返回message，否则返回None，表示不处理
-        message_text: 消息文本
-        message_raw: 消息原始数据 `RawMessage`
+        If the message_text contains the keyword, return the function to be executed, otherwise return None
+        :param message_text: 消息文本
+        :param kwargs :
+        message_raw: 消息原始数据 `EventMessage`
         address: 消息地址 `tuple(sender,receiver)`
         """
-        for i in self.keywords:
-            if i in message_text:
+        for word in self.keywords:
+            if word in message_text:
                 return self.function
-        # 正则匹配
+        # Regrex Match
         if self.pattern:
             match = self.pattern.match(message_text)
             if match:
                 return self.function
+        _ignore = kwargs
         return None
 
     @abstractmethod
-    async def failed(self,
-                     task: "TaskHeader", receiver: "TaskHeader.Location",
-                     exception, env: dict,
-                     arg: dict, pending_task: "TaskBatch", refer_llm_result: dict = None,
-                     ):
+    async def failed(
+        self,
+        task: "TaskHeader",
+        receiver: "Location",
+        exception,
+        env: dict,
+        arg: dict,
+        pending_task: "ToolCall",
+        refer_llm_result: dict = None,
+    ):
         """
         通常为 回写消息+通知消息
         :param task: 任务
         :param receiver: 接收者
         :param exception: 异常
         :param env: 环境变量
         :param arg: 参数
         :param pending_task: 任务批次
         :param refer_llm_result: 上一次的结果
         """
+        _ignore = task, receiver, env, arg, pending_task, refer_llm_result, exception
         return ...
 
     @abstractmethod
-    async def callback(self,
-                       task: "TaskHeader", receiver: "TaskHeader.Location",
-                       env: dict,
-                       arg: dict, pending_task: "TaskBatch", refer_llm_result: dict = None
-                       ):
+    async def callback(
+        self,
+        task: "TaskHeader",
+        receiver: "Location",
+        env: dict,
+        arg: dict,
+        pending_task: "ToolCall",
+        refer_llm_result: dict = None,
+    ):
         """
         运行成功会调用此函数
         :param task: 任务
         :param receiver: 接收者
         :param arg: 参数
         :param env: 环境变量
         :param pending_task: 任务批次
         :param refer_llm_result: 上一次的结果
         """
+        _ignore = task, receiver, env, arg, pending_task, refer_llm_result
         return ...
 
     @abstractmethod
-    async def run(self, *,
-                  task: "TaskHeader", receiver: "TaskHeader.Location",
-                  arg: dict, env: dict, pending_task: "TaskBatch", refer_llm_result: dict = None,
-                  ):
+    async def run(
+        self,
+        *,
+        task: "TaskHeader",
+        receiver: "Location",
+        arg: dict,
+        env: dict,
+        pending_task: "ToolCall",
+        refer_llm_result: dict = None,
+    ):
         """
         处理函数并返回回写结果
         :param task: 任务
         :param receiver: 接收者
         :param arg: 参数
         :param env: 环境变量
         :param pending_task: 任务批次
         :param refer_llm_result: 上一次的结果
         """
+        _ignore = task, receiver, env, arg, pending_task, refer_llm_result
         return ...
 
     @final
-    async def load(self, *,
-                   task: "TaskHeader", receiver: "TaskHeader.Location",
-                   arg: dict, env: dict = None, pending_task: "TaskBatch", refer_llm_result: dict = None,
-                   **kwargs
-                   ) -> dict:
+    async def load(
+        self,
+        *,
+        task: "TaskHeader",
+        receiver: "Location",
+        arg: dict,
+        env: dict = None,
+        pending_task: "ToolCall",
+        refer_llm_result: Union[OpenAIResult, dict] = None,
+        **kwargs,
+    ) -> dict:
         """
         加载工具，执行前的准备工作
         :param task: 任务
         :param receiver: 接收者
         :param arg: 参数
         :param env: 环境变量
         :param pending_task: 任务批次
         :param refer_llm_result: 上一次的结果
         :param kwargs: 额外参数
         :return: 运行结果
         """
         if not env:
             env = {}
         # 拒绝循环引用, 复制一份传递
-        self.__run_arg = {
+        run_pipe = {
             "task": task.model_copy(deep=True),
             "receiver": receiver.model_copy(deep=True),
             "arg": arg,
             "env": env,
             "pending_task": pending_task.model_copy(deep=True),
-            "refer_llm_result": refer_llm_result
+            "refer_llm_result": refer_llm_result,
         }
-        self.__run_arg.update(kwargs)
+        run_pipe.update(kwargs)
         try:
-            run_result = await self.run(
-                **self.__run_arg
-            )
+            run_result = await self.run(**run_pipe)
         except Exception as e:
             logger.exception(e)
             logger.error(f"ToolExecutor:run error: {e}")
-            self.__run_arg["exception"] = str(e)
-            await self.failed(
-                **self.__run_arg
-            )
+            run_pipe["exception"] = str(e)
+            await self.failed(**run_pipe)
         else:
-            self.__run_arg["result"] = run_result
+            run_pipe["result"] = run_result
             try:
-                await self.callback(
-                    **self.__run_arg
-                )
+                await self.callback(**run_pipe)
             except Exception as e:
                 logger.error(f"ToolExecutor:callback error: {e}")
-        return self.__run_arg
+        return run_pipe
 
 
 @dataclass(eq=False)
 class FuncPair:
-    function: "Function"
+    function: Union[Tool]
     tool: Type[BaseTool]
     extra_arg: Dict[Any, Any] = field(default_factory=dict)
 
     @property
     def name(self):
-        return self.function.name
+        return self.function.function.name
 
 
 class PluginMetadata(BaseModel):
     """
     插件元信息，由插件编写者提供
     """
 
@@ -294,8 +328,9 @@
     parent_plugin: Optional["Plugin"] = None
     """父插件"""
     sub_plugins: Set["Plugin"] = field(default_factory=set)
     """子插件集合"""
     metadata: Optional[PluginMetadata] = None
     """插件元信息"""
 
+
 # 探针插件加载机制 参考 nonebot2 项目设计
```

### Comparing `llmkira-0.27.3/llmkira/sdk/memory/redis/__init__.py` & `llmkira-1.0.0/llmkira/memory/redis_storage/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,79 +1,82 @@
 # -*- coding: utf-8 -*-
 # Source: https://github.com/langchain-ai/langchain/blob/master/libs/langchain/langchain/utilities/redis.py
 from __future__ import annotations
 
 import json
+from typing import List
 
 import redis
 from loguru import logger
+from pydantic import BaseModel
 from pydantic import Field, model_validator
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
-from llmkira.sdk.schema import Message, parse_message_dict
-from .utils import get_client
+from llmkira.memory._base import BaseMessageStorage
+from llmkira.memory.redis_storage.utils import get_client
 
 
-class RedisChatMessageHistory(object):
-    class RedisSettings(BaseSettings):
-        redis_url: str = Field("redis://localhost:6379/0", validation_alias="REDIS_DSN")
-        redis_key_prefix: str = "llm_message_store_1:"
-        model_config = SettingsConfigDict(env_file='.env', env_file_encoding='utf-8', extra="ignore")
-
-        @model_validator(mode="after")
-        def redis_is_connected(self):
-            redis_url = self.redis_url
-            try:
-                get_client(redis_url=redis_url)
-            except redis.exceptions.ConnectionError as error:
-                logger.error(error)
-                raise ValueError("Could not connect to Redis")
-            else:
-                logger.info("Core:Created Redis client successfully")
-            return self
-
-    def __init__(
-            self,
-            session_id: str,
-            ttl: int,
-            redis_config: RedisSettings = RedisSettings(),
-    ):
+class RedisSettings(BaseSettings):
+    redis_url: str = Field("redis://localhost:6379/0", validation_alias="REDIS_DSN")
+    redis_key_prefix: str = "llm_message_store:"
+    model_config = SettingsConfigDict(
+        env_file=".env", env_file_encoding="utf-8", extra="ignore"
+    )
+
+    @model_validator(mode="after")
+    def redis_is_connected(self):
+        redis_url = self.redis_url
+        try:
+            redis_client = get_client(redis_url=redis_url)
+            redis_client.ping()
+        except redis.exceptions.ConnectionError as error:
+            logger.warning(f"Could not connect to Redis: {error}")
+            raise ValueError("Could not connect to Redis")
+        else:
+            logger.debug("Core: Connect to Redis")
+        return self
+
+
+class RedisChatMessageHistory(BaseMessageStorage):
+    def __init__(self, session_id: str, ttl: int, redis_config: RedisSettings = None):
+        if redis_config is None:
+            redis_config = RedisSettings()
         try:
             import redis
         except ImportError:
             raise ImportError(
-                "Could not import redis python package. "
-                "Please install it with `pip install redis`."
+                "Could not import redis python package. Please install it with `pip install redis`."
             )
-
         try:
             self.redis_client = get_client(redis_url=redis_config.redis_url)
         except redis.exceptions.ConnectionError as error:
             logger.error(error)
-
         self.session_id = session_id
         self.key_prefix = redis_config.redis_key_prefix
         self.ttl = ttl
 
+    def update_session(self, session_id: str):
+        self.session_id = session_id
+        return self
+
     @property
     def key(self) -> str:
-        """Construct the record key to use"""
         return self.key_prefix + self.session_id
 
-    @property
-    def messages(self) -> List[BaseMessage]:  # type: ignore
-        """Retrieve the messages_box from Redis"""
-        _items = self.redis_client.lrange(self.key, 0, -1)
+    async def read(self, lines: int) -> List[str]:
+        _items = self.redis_client.lrange(self.key, 0, lines - 1)
         items = [json.loads(m.decode("utf-8")) for m in _items[::-1]]
-        messages = [parse_message_dict(m) for m in items]
-        messages = [m for m in messages if m is not None]
-        return messages
-
-    def add_message(self, message: Message) -> None:
-        """Append the message to the record in Redis"""
-        self.redis_client.lpush(self.key, message.model_dump_json())
-        if self.ttl:
-            self.redis_client.expire(self.key, self.ttl)
+        return items
+
+    async def append(self, message: List[BaseModel]):
+        for m in message:
+            message_json = m.json()
+            await self.redis_client.lpush(self.key, message_json)
+            if self.ttl:
+                await self.redis_client.expire(self.key, self.ttl)
+
+    async def write(self, message: List[BaseModel]):
+        self.clear()
+        await self.append(message)
 
     def clear(self) -> None:
-        """Clear session memory from Redis"""
         self.redis_client.delete(self.key)
```

### Comparing `llmkira-0.27.3/llmkira/sdk/memory/redis/utils.py` & `llmkira-1.0.0/llmkira/memory/redis_storage/utils.py`

 * *Files identical despite different names*

### Comparing `llmkira-0.27.3/llmkira/sdk/openapi/fuse/__init__.py` & `llmkira-1.0.0/llmkira/openapi/fuse/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 # @Software: PyCharm
 
 ####
 # 此包包含错误计数器，用于统计错误次数，标记错误次数过多的插件。
 # 在构造阶段读取用户数据库，合并至 ignore 中。
 # 注意，注意回调的实现。
 ####
-from typing import Dict
-from typing import TYPE_CHECKING
+from typing import Dict, Union, Type
 
 import wrapt
 from loguru import logger
+from pydantic import BaseModel
 
-if TYPE_CHECKING:
-    from ...schema import Function
+from llmkira.openai.cell import Tool, class_tool
 
 __error_table__: Dict[str, int] = {}
 
 
 def get_error_plugin(error_times: int = 10) -> list:
     """
     获取错误次数过多的插件
@@ -35,31 +34,33 @@
     恢复错误插件
     :param function_name:
     :return:
     """
     __error_table__[function_name] = 0
 
 
-def resign_plugin_executor(function: "Function",
-                           *,
-                           handle_exceptions: tuple = (Exception,),
-                           exclude_exceptions: tuple = ()
-                           ):
+def resign_plugin_executor(
+    tool: Union[Tool, Type[BaseModel]],
+    *,
+    handle_exceptions: tuple = (Exception,),
+    exclude_exceptions: tuple = (),
+):
     """
     装饰器，先判断是否排除，再判断是否处理
-    :param function: 被装饰的函数
+    :param tool: 被装饰的函数
     :param handle_exceptions: 处理的异常，只有在此列表中的异常才会被计数
     :param exclude_exceptions: 排除的异常，不会被计数。不可以是宽泛的异常，如 Exception
     :return: 装饰器
     """
+    tool = class_tool(tool)
     if not handle_exceptions:
         handle_exceptions = (Exception,)
     if Exception in exclude_exceptions or BaseException in exclude_exceptions:
         raise ValueError("Exception and BaseException cant be exclude")
-    logger.success(f"📦 [Plugin exception hook] {function.name}")
+    logger.success(f"📦 [Plugin exception hook] {tool.function.name}")
 
     @wrapt.decorator  # 保留被装饰函数的元信息
     def wrapper(wrapped, instance, args, kwargs):
         """
         :param wrapped: 被装饰的函数
         :param instance: https://wrapt.readthedocs.io/en/latest/
         :param args: 被装饰函数的参数
@@ -69,15 +70,19 @@
         try:
             res = wrapped(*args, **kwargs)
         except Exception as e:
             if e in exclude_exceptions:
                 logger.exception(e)
                 return {}
             if e in handle_exceptions:
-                __error_table__[function.name] = __error_table__.get(function.name, 0) + 1
+                __error_table__[tool.function.name] = (
+                    __error_table__.get(tool.function.name, 0) + 1
+                )
                 logger.exception(e)
-            logger.warning(f"📦 [Plugin Not Handle Exception Hook] {function.name} {e}")
+            logger.warning(
+                f"📦 [Plugin Not Handle Exception Hook] {tool.function.name} {e}"
+            )
         else:
             return res
         return {}
 
     return wrapper
```

### Comparing `llmkira-0.27.3/llmkira/sdk/openapi/transducer/__init__.py` & `llmkira-1.0.0/llmkira/openapi/transducer/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,21 +55,21 @@
         message: "RawMessage"
         :return platform
         """
         _loop = []
         for _exec_ram in __builder__:
             _exec = _exec_ram()
             if not _exec.sign:
-                logger.error(f"receiver_loop metadata None:sign")
+                logger.error("receiver_loop metadata None:sign")
                 continue
             if not _exec.sign.platform:
-                logger.error(f"receiver_loop metadata None:platform")
+                logger.error("receiver_loop metadata None:platform")
                 continue
             if _exec.sign.priority is None:
-                logger.error(f"receiver_loop metadata None:priority")
+                logger.error("receiver_loop metadata None:priority")
                 continue
             if _exec.sign.agent != "receiver":
                 continue
             if _exec.sign.platform.match(platform_name):
                 _loop.append(_exec_ram)
         _loop.sort(key=lambda x: x.sign.priority, reverse=True)
         return _loop
@@ -81,49 +81,55 @@
         message: list, file: List[File]
         :return platform
         """
         _loop = []
         for _exec_ram in __parser__:
             _exec = _exec_ram()
             if not _exec.sign:
-                logger.error(f"sender_loop metadata None:sign")
+                logger.error("sender_loop metadata None:sign")
                 continue
             if not _exec.sign.platform:
-                logger.error(f"sender_loop metadata None:platform")
+                logger.error("sender_loop metadata None:platform")
                 continue
             if _exec.sign.priority is None:
-                logger.error(f"sender_loop metadata None:priority")
+                logger.error("sender_loop metadata None:priority")
                 continue
             if _exec.sign.agent == "sender":
                 continue
             if _exec.sign.platform.match(platform_name):
                 _loop.append(_exec_ram)
         _loop.sort(key=lambda x: x.sign.priority, reverse=True)
         return _loop
 
     @property
     def result_pipe_arg(self):
         if not self.pipe_arg:
-            raise ValueError(f"pipe_arg is None")
+            raise ValueError("pipe_arg is None")
         return self.pipe_arg
 
-    async def exec_loop(self, pipe: List[Type[AbstractTransfer]], pipe_arg: dict, validator: Callable = None):
+    async def exec_loop(
+        self,
+        pipe: List[Type[AbstractTransfer]],
+        pipe_arg: dict,
+        validator: Callable = None,
+    ):
         """
         exec loop
         """
         self.pipe_arg = pipe_arg
         for loop in pipe:
             try:
                 if validator:
                     validator(**self.pipe_arg)
                 new_pipe_arg = await loop().pipe(self.pipe_arg)
             except Exception as e:
                 # logger.info(f"{loop.__name__} exec_loop error {e}, for sign:{loop.sign}")
-                logger.debug(f"{loop.__name__} exec_loop error {e}, for sign:{loop.sign}, pipe_arg:{pipe_arg}")
+                logger.debug(
+                    f"{loop.__name__} exec_loop error {e}, for sign:{loop.sign}, pipe_arg:{pipe_arg}"
+                )
                 # 不更新 pipe_arg
             else:
                 # logger.info(f"{loop.__name__} exec_loop success, for sign:{loop.sign}")
-                logger.debug(f"{loop.__name__} exec_loop success, for sign:{loop.sign}, new_pipe_arg:{new_pipe_arg}")
+                logger.debug(
+                    f"{loop.__name__} exec_loop success, for sign:{loop.sign}, new_pipe_arg:{new_pipe_arg}"
+                )
                 self.pipe_arg = new_pipe_arg
-
-
-from .default_factory import DefaultMessageBuilder, DefaultMessageParser
```

### Comparing `llmkira-0.27.3/llmkira/sdk/openapi/transducer/default_factory.py` & `llmkira-1.0.0/llmkira/openapi/transducer/default_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 @resign_transfer()
 class DefaultMessageBuilder(Builder):
     sign = TransferMata(
         platform=re.compile(r".*"),  # 匹配所有
         plugin_name="default",
         agent="receiver",
-        priority=0
+        priority=0,
     )
 
     async def pipe(self, arg) -> Any:
         return arg
 
 
 @resign_transfer()
 class DefaultMessageParser(Parser):
     sign = TransferMata(
         platform=re.compile(r".*"),  # 匹配所有
         plugin_name="default",
         agent="sender",
-        priority=0
+        priority=0,
     )
 
     async def pipe(self, arg) -> Any:
         return arg
```

### Comparing `llmkira-0.27.3/llmkira/sdk/openapi/transducer/schema.py` & `llmkira-1.0.0/llmkira/openapi/transducer/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pydantic import BaseModel, Field
 
 
 class TransferMata(BaseModel):
     """
     注册标头
     """
+
     platform: re.Pattern
     plugin_name: str
     # 优先级
     priority: int = Field(default=0, ge=-100, le=100)
     # 适用端 (sender/receiver)
     agent: Literal["sender", "receiver", None] = Field(default=None)
 
@@ -26,14 +27,15 @@
 
 
 class Builder(AbstractTransfer):
     """
     Receiver Parser
     消息对象转媒体文件
     """
+
     sign: TransferMata
 
     @abstractmethod
     async def pipe(self, arg: dict) -> Any:
         """
         change only_send_file to `True` for send file only
         :return 是否要回复文本,文件列表
@@ -42,14 +44,15 @@
 
 
 class Parser(AbstractTransfer):
     """
     Sender Parser
     媒体文件对象转消息对象
     """
+
     sign: TransferMata
 
     @abstractmethod
     async def pipe(self, arg: dict) -> Any:
         """
         change file list to RawMessage,pls return few message
         :return 回环消息列表,文件列表
```

### Comparing `llmkira-0.27.3/llmkira/sdk/openapi/trigger/__init__.py` & `llmkira-1.0.0/llmkira/openapi/trigger/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,20 +60,19 @@
     """
 
     def decorator(func):
         if inspect.iscoroutinefunction(func):
             __trigger_phrases__.append(trigger.update_func(func))
             logger.success(f"📦 [Plugin trigger hook] {trigger.__repr__()}")
         else:
-            raise ValueError(f"Resign Trigger Error for func {func} is not async function")
+            raise ValueError(
+                f"Resign Trigger Error for func {func} is not async function"
+            )
 
         @wraps(func)
         async def wrapper(*args, **kwargs):
             # 调用执行函数，中间人
             return func(*args, **kwargs)
 
         return wrapper
 
     return decorator
-
-
-from .default_trigger import on_chat_message
```

### Comparing `llmkira-0.27.3/llmkira/sdk/schema.py` & `llmkira-1.0.0/llmkira/task/schema.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,724 +1,657 @@
 # -*- coding: utf-8 -*-
-# @Time    : 2023/8/16 上午11:06
+# @Time    : 2023/10/14 下午2:16
 # @Author  : sudoskys
-# @File    : components.py
+# @File    : schema.py
 # @Software: PyCharm
-import base64
-import hashlib
-import pickle
 import time
-from abc import abstractmethod, ABC
-from io import BytesIO
-from typing import Literal, Optional, List, Type, Union
-from typing import TYPE_CHECKING
+from enum import Enum
+from typing import TYPE_CHECKING, Dict
+from typing import Tuple, List, Union, Optional
 
-import aiohttp
+import hikari
+import khl
 import shortuuid
-from docstring_parser import parse
 from loguru import logger
-from pydantic import model_validator, BaseModel, Field, PrivateAttr, ConfigDict
+from pydantic import model_validator, ConfigDict, Field, BaseModel
 
-from .cache import global_cache_runtime
-from .error import ValidationError, CheckError
-from .utils import sync, aiohttp_download_file
+from llmkira.kv_manager.file import File
+from llmkira.openai.cell import UserMessage, ToolMessage, ToolCall, Message
+from llmkira.openai.request import OpenAIResult
 
 if TYPE_CHECKING:
     pass
 
 
-# ATTENTION:禁止调用上层任何schema包，否则会导致循环引用
-
-def generate_uid():
-    return shortuuid.uuid()[0:8].upper()
-
-
-class File(BaseModel):
+class EventMessage(BaseModel):
     """
-    请求体
-    可提供标准化的文件定义。
-    但是不能直接提供接口标准化，因为文件上传需要特殊处理
+    Event Message for mq database
     """
 
-    class Data(BaseModel):
-        file_name: str
-        file_data: bytes = Field(None, description="文件数据")
-
-        @property
-        def pair(self):
-            return self.file_name, self.file_data
-
-    file_name: str = Field(..., description="文件名，不一定和数据匹配")
-    file_id: Optional[str] = Field(None, description="文件的数据库ID，用于索引文件数据，所以没有数据就不要填")
-    file_url: Optional[str] = Field(None, description="文件URL，不一定有")
-    caption: Optional[str] = Field(default='', description="文件注释，展示给LLM")
-    created_by: str = Field(default=None, description="Uploader **UID**")
-    created_at: int = Field(default=int(time.time()))
-    bytes_length: Optional[int] = Field(default=None, description="File Size")
-
-    @model_validator(mode="after")
-    def file_id_validator(self):
-        if self.file_id:
-            assert len(self.file_id) <= 8, "file_id must be less than 8"
-            assert isinstance(self.file_id, str), "file_id must be str"
-        if self.created_by:
-            assert ":" in self.created_by, "created_by must be uid, include `:` ,like `discord:123456`"
-        return self
-
-    def __eq__(self, other):
-        if isinstance(other, File):
-            return (self.file_id == other.file_id) and (self.file_name == other.file_name)
-        else:
-            return False
-
-    def __ne__(self, other):
-        return not self.__eq__(other)
-
-    def __hash__(self):
-        return hash(self.file_id) + hash(self.file_name)
-
-    def is_user_upload(self, uid: str):
-        """
-        判断是否是某个用户上传的
-        """
-        return self.created_by == uid
-
-    @property
-    def file_prompt(self):
-        """
-        FOR LLM
-        """
-        _comment = '('
-        for key, value in self.model_dump().items():
-            if value:
-                _comment += f"{key}={value},"
-            else:
-                if key == "file_id":
-                    _comment += f"{key}=MissingAlertNeeded,"
-        return f"[Attachment{_comment[:-1]})]"
-
-    @staticmethod
-    async def download_file_by_id(
-            file_id: str,
-    ) -> Optional[Data]:
-        cache = global_cache_runtime.get_redis()
-        file = await cache.read_data(file_id)
-        if not file:
-            return None
-        file_obj: File.Data = pickle.loads(file)
-        return file_obj
-
-    async def raw_file(
-            self,
-    ) -> Optional[Data]:
-        cache = global_cache_runtime.get_redis()
-        if not self.file_id:
-            return None
-        file = await cache.read_data(self.file_id)
-        if not file:
-            return None
-        file_obj: File.Data = pickle.loads(file)
-        return file_obj
-
-    @classmethod
-    async def upload_file(cls,
-                          file_name: str,
-                          file_data: Union[bytes, BytesIO],
-                          creator_uid: str,
-                          caption: str = "",
-                          file_id: str = None,
-                          size_limit: int = 1024 * 1024 * 10,
-                          ):
-        """
-        上传文件，要求用户使用 UID
-        """
-        assert isinstance(file_data, bytes) or isinstance(file_data, BytesIO), "file_data must be bytes or BytesIO"
-        if file_id is None:
-            file_id = str(generate_short_md5(file_data))
-        cache = global_cache_runtime.get_redis()
-        _byte_length = len(file_data)
-        if _byte_length > size_limit:
-            raise CheckError(f"file size must be less than {size_limit}")
-        await cache.set_data(
-            key=file_id,
-            value=pickle.dumps(File.Data(file_name=file_name, file_data=file_data)),
-            timeout=60 * 60 * 24 * 7
+    user_id: Union[str] = Field(None, description="User id")
+    chat_id: Union[str] = Field(None, description="Chat id")
+    thread_id: Optional[Union[str]] = Field(
+        None, description="Channel ID(slack thread)"
+    )
+    text: str = Field("", description="Text of message")
+    files: List[File] = Field([], description="File(ID*) of message")
+    created_at: str = Field(
+        default_factory=lambda: str(int(time.time())), description="Create time"
+    )
+
+    model_config = ConfigDict(arbitrary_types_allowed=False, extra="allow")
+
+    # only_send_file: bool = Field(default=False, description="Send file only")
+    # sign_loop_end: bool = Field(default=False, description="要求其他链条不处理此消息，用于拦截器开发")
+    # sign_fold_docs: bool = Field(default=False, description="是否获取元数据")
+
+    def format_user_message(self, name: str = None) -> UserMessage:
+        """Format message to UserMessage"""
+        return UserMessage(
+            role="user",
+            name=name,
+            content=self.text,
         )
-        assert len(file_id) <= 8, "file_id must be less than 8"
-        assert isinstance(file_id, str), "file_id must be str"
-        return cls(file_id=file_id,
-                   file_name=file_name,
-                   bytes=_byte_length,
-                   created_by=creator_uid,
-                   caption=caption,
-                   )
 
     @classmethod
-    async def upload_file_only_url(cls,
-                                   file_name,
-                                   file_url,
-                                   created_by: str,
-                                   caption: str = "",
-                                   ):
-        return cls(file_id=None,
-                   file_url=file_url,
-                   file_name=file_name,
-                   created_by=created_by,
-                   caption=caption,
-                   )
-
-    @classmethod
-    async def upload_file_by_download_url(cls,
-                                          file_name,
-                                          file_url,
-                                          created_by: str,
-                                          caption: str = "",
-                                          size_limit: int = 1024 * 1024 * 10,
-                                          headers: dict = None,
-                                          session: aiohttp.ClientSession = None,
-                                          ):
-        cache = global_cache_runtime.get_redis()
-        file_data = await aiohttp_download_file(file_url,
-                                                session=session,
-                                                timeout=20,
-                                                size_limit=size_limit,
-                                                headers=headers
-                                                )
-        _byte_length = len(file_data)
-        _key = generate_short_md5(file_data)
-        await cache.set_data(
-            key=_key,
-            value=pickle.dumps(File.Data(file_name=file_name, file_data=file_data)),
-            timeout=60 * 60 * 24 * 7
+    def from_openai_message(
+        cls, message: Message, locate: "Location"
+    ) -> "EventMessage":
+        """
+        用于 OpenAI 消息转换回复给用户
+        """
+        return cls(
+            user_id=locate.user_id,
+            text=message.content,
+            chat_id=locate.chat_id,
+            created_at=str(int(time.time())),
         )
-        return cls(file_id=_key,
-                   file_name=file_name,
-                   bytes=_byte_length,
-                   created_by=created_by,
-                   caption=caption,
-                   )
 
 
-class BaseFunction(BaseModel):
+class ToolResponse(BaseModel):
     """
-    请求体
-    只供 Choice 使用
+    Tool Callback for plugin tool
+    # TODO:携带自身工具，供我们重组上下文工具时mock使用。
     """
 
-    class FunctionExtra(BaseModel):
-        system_prompt: Optional[str] = Field(None, description="系统提示")
+    name: str = Field(description="功能名称", pattern=r"^[a-zA-Z0-9_]+$")
+    function_response: str = Field("[empty response]", description="工具响应内容")
+    tool_call_id: str = Field(description="工具调用ID")
+    tool_call: ToolCall = Field(description="工具调用")
 
-        @classmethod
-        def default(cls):
-            return cls(system_prompt=None)
+    def format_tool_message(self) -> Union[ToolMessage]:
+        if self.tool_call_id:
+            return ToolMessage(
+                tool_call_id=self.tool_call_id, content=self.function_response
+            )
+        raise ValueError("tool_call_id is empty")
 
-    _config: FunctionExtra = FunctionExtra.default()
-    name: Optional[str] = Field(None, description="函数名称", pattern=r"^[a-zA-Z0-9_]+$")
 
-    def update_config(self, config: "FunctionExtra") -> "BaseFunction":
-        self._config = config
-        return self
+class Router(Enum):
+    REPLIES = "replies"  # 回复消息
+    DELIVER = "deliver"  # 只通知，不重组函数和初始化任何东西。
+    REPROCESS = "reprocess"  # 回写消息，释放任务链，要求再次处理
+    ANSWER = "answer"  # 回复消息
 
-    def update_system_prompt(self, prompt: str) -> "BaseFunction":
-        self._config.system_prompt = prompt
-        return self
 
-    @property
-    def config(self) -> "FunctionExtra":
-        return self._config
+class Sign(BaseModel):
+    sign_as: Tuple[int, str, str, str] = Field(
+        default=(0, "root", "default", str(shortuuid.uuid()).upper()[:5]),
+        description="签名",
+    )
+    """当前链条的层级"""
 
-    def request_final(self,
-                      *,
-                      schema_model: str):
-        return self.model_copy(deep=True)
+    instruction: Optional[str] = Field(None, description="指令")
+    """System Prompt"""
 
+    disable_tool_action: bool = False
+    """Toolcall 是否被禁用"""
 
-class Function(BaseFunction):
-    """
-    请求体
-    供外部模组定义并注册函数
-    """
+    tool_response: List["ToolResponse"] = Field(
+        default=[], description="用于回写，插件返回的消息头，标识 function 的名字"
+    )
+    """工具响应"""
 
-    class Parameters(BaseModel):
-        type: str = "object"
-        properties: dict = {}
-        required: List[str] = Field(default=[], description="必填参数")
-        model_config = ConfigDict(extra="ignore")
-
-    name: Optional[str] = Field(None, description="函数名称", pattern=r"^[a-zA-Z0-9_]+$")
-    description: Optional[str] = None
-    parameters: "Parameters" = Field(default_factory=lambda: Function.Parameters(), description="参数")
-    model_config = ConfigDict(extra="ignore")
-
-    def request_final(self,
-                      *,
-                      schema_model: str):
-        """
-        标准化
-        :param schema_model: 适配的模型
-        """
-        if schema_model.startswith("gpt-"):
-            return self.model_copy(deep=True)
-        elif schema_model.startswith("chatglm"):
-            return self.model_copy(deep=True)
-        else:
-            raise CheckError(f"unknown model {schema_model}, cant classify model type")
-
-    def add_property(self,
-                     property_name: str,
-                     property_type: Literal["string", "integer", "number", "boolean", "object", "array"],
-                     property_description: str,
-                     enum: Optional[tuple] = None,
-                     required: bool = False
-                     ):
-        """
-        加注属性
-        """
-        self.parameters.properties[property_name] = {}
-        self.parameters.properties[property_name]['type'] = property_type
-        self.parameters.properties[property_name]['description'] = property_description
-        if enum:
-            self.parameters.properties[property_name]['enum'] = tuple(enum)
-        if required:
-            self.parameters.required.append(property_name)
+    memory_able: bool = False
+    """是否写回数据库"""
 
-    @classmethod
-    def parse_from_pydantic(cls,
-                            schema_model: Type[BaseModel],
-                            plugin_name: str = None,
-                            ):
-        """
-        解析 pydantic 的 schema
-        """
-        schema = schema_model.model_json_schema()
-        docstring = parse(schema.__doc__ or "")
-        parameters = {
-            k: v for k, v in schema.items() if k not in ("title", "description")
-        }
-        for param in docstring.params:
-            name = param.arg_name
-            description = param.description
-            if (name in parameters["properties"]) and description:
-                if "description" not in parameters["properties"][name]:
-                    parameters["properties"][name]["description"] = description
+    router: Router = Field(Router.ANSWER, description="路由规则")
+    """路由规则"""
 
-        parameters["required"] = sorted(
-            k for k, v in parameters["properties"].items() if "default" not in v
-        )
+    response_snapshot: bool = Field(False, description="是否响应函数快照")
+    """接收器是否响应函数快照"""
 
-        if "description" not in schema:
-            if docstring.short_description:
-                schema["description"] = docstring.short_description
-            else:
-                schema["description"] = (
-                    f"Correctly extracted `{cls.__name__}` with all "
-                    f"the required parameters with correct types"
-                )
-        plugin_name = plugin_name or schema["title"]
-        return cls(
-            name=plugin_name,
-            description=schema["description"],
-            parameters=parameters,
-        )
+    # resign_next_step: bool = Field(False, description="函数集群是否可以继续拉起其他函数集群")
+    tool_calls_counter: int = Field(0, description="函数集群计数器")
+    """函数响应计数"""
 
+    tool_calls_limit: int = Field(5, description="函数集群计数器上限")
+    """函数响应限制"""
 
-class FunctionCallCompletion(BaseModel):
-    name: str
-    arguments: str
+    tool_calls_pending: List[ToolCall] = Field([], description="函数快照")
+    """待处理的函数响应"""
 
+    tool_calls_completed: List[Tuple[ToolCall, bool, Union[str, dict]]] = Field(
+        default=[], description="完成的节点状态"
+    )
+    """完成的函数响应"""
 
-class Tool(BaseModel):
-    """
-    请求体
-    """
-    type: str = Field(default="function")
-    function: "Function"
-
-    def request_final(
-            self,
-            *,
-            schema_model
-    ):
-        if schema_model.startswith("gpt-"):
-            return self
-        elif schema_model.startswith("chatglm"):
-            return self
-        else:
-            return self
-            # raise CheckError(f"unknown model {schema_model}, cant classify model type")
+    # tool_calls_completed: List[ToolCall] = Field([], description="完成的函数快照")
+    snapshot_credential: Optional[str] = Field(
+        None, description="认证链的UUID，根据此UUID和 Map 可以确定哪个需要执行"
+    )
+    """当前待处理的函数"""
 
+    certify_needed_map: Dict[str, ToolCall] = Field(
+        {}, description="Snapshot Map for uuid, toolcall"
+    )
+    """认证地图，需要快照"""
 
-class ToolChoice(BaseModel):
-    """
-    请求体
-    """
-    type: str = Field(default=None)
-    function: "BaseFunction" = Field(default=None)
+    llm_response: Optional[OpenAIResult] = Field(None, description="OpenAI Response")
+    """原生响应"""
 
+    model_config = ConfigDict(extra="ignore", arbitrary_types_allowed=False)
 
-class ToolCallCompletion(ToolChoice):
-    """
-    响应
-    """
-    id: str = Field(default=None)
-    type: str = Field(default=None)
-    function: "FunctionCallCompletion" = Field(default=None)
+    @property
+    def task_uuid(self):
+        return self.sign_as[3]
 
+    @model_validator(mode="after")
+    def validate_param(self):
+        # If it is the root node, it cannot be written back.
+        # Because the message posted by the user is always the root node.
+        # Writing back will cause duplicate messages.
+        if self.sign_as[0] == 0 and self.memory_able:
+            logger.warning("root node cant write back")
+            self.memory_able = False
+        return self
 
-class TaskBatch(BaseModel):
-    id: str = Field(default=None)
-    type: str = Field(default=None)
-    function: "FunctionCallCompletion" = Field(default=None)
+    def child(self, name: str) -> "Sign":
+        """
+        生成子节点，继承父节点的功能
+        """
+        self.sign_as = (self.sign_as[0] + 1, "child", name, self.sign_as[3])
+        return self.model_copy(deep=True)
 
-    @classmethod
-    def from_tool_call(cls, tool_call: "ToolCallCompletion"):
-        if not tool_call:
-            return None
-        return cls(
-            id=tool_call.id,
-            type=tool_call.type,
-            function=tool_call.function
-        )
+    def snapshot(self, name, memory_able: bool, response_snapshot: bool) -> "Sign":
+        """
+        快照
+        """
+        self.sign_as = (self.sign_as[0] + 1, "chain", name, self.sign_as[3])
+        self.router = Router.ANSWER
+        self.memory_able = memory_able
+        self.response_snapshot = response_snapshot
+        return self.model_copy(deep=True)
 
     @classmethod
-    def from_function_call(cls, function_call: "FunctionCallCompletion"):
-        if not function_call:
-            return None
+    def from_root(
+        cls,
+        response_snapshot: bool,
+        disable_tool_action: bool,
+        platform: str = "default",
+    ) -> "Sign":
+        """
+        构造函数，从根节点生成
+        :param response_snapshot: 是否响应函数快照
+        :param disable_tool_action: 是否禁用工具调用
+        :param platform: 平台
+        """
+        node_uuid = str(shortuuid.uuid()).upper()[:5]
         return cls(
-            id=None,
-            type="function",
-            function=function_call
+            sign_as=(0, "root", platform, node_uuid),
+            response_snapshot=response_snapshot,
+            disable_tool_action=disable_tool_action,
         )
 
-    def get_batch_name(self):
-        return self.function.name
-
-    def get_batch_args(self):
-        return self.function.arguments
+    def update_tool_calls(
+        self,
+        *,
+        tool_calls: List[ToolCall],
+        certify_needed_map: dict,
+    ) -> "Sign":
+        """
+        更新快照
+        :param tool_calls: 快照
+        :param certify_needed_map: 快照Map
+        :return: Sign
+        :raise ValueError: 快照不能为空
+        """
+        if not certify_needed_map:
+            certify_needed_map = self.certify_needed_map
+        if not tool_calls:
+            raise ValueError("plan_chain_pending can't be empty")
+        copy_model = self.model_copy(deep=True)
+        copy_model.certify_needed_map = certify_needed_map
+        copy_model.tool_calls_pending = tool_calls
+        return copy_model
+
+    def update_state(
+        self,
+        router: Router = None,
+        instruction: str = None,
+        disable_tool_action: bool = None,
+        memory_able: bool = None,
+        response_snapshot: bool = None,
+        tool_calls: List[ToolCall] = None,
+        tool_response: List[ToolResponse] = None,
+    ) -> "Sign":
+        """
+        更新状态，用于统一管理状态
+        """
+        if router:
+            self.router = router
+        if instruction:
+            self.instruction = instruction
+        if disable_tool_action is not None:
+            self.disable_tool_action = disable_tool_action
+        if memory_able is not None:
+            self.memory_able = memory_able
+        if response_snapshot is not None:
+            self.response_snapshot = response_snapshot
+        if tool_calls:
+            self.tool_calls_pending = tool_calls
+        if tool_response:
+            self.tool_response = tool_response
+        return self
 
-    def get_batch_id(self):
-        return self.id
+    def notify(
+        self,
+        *,
+        plugin_name: str,
+        tool_response: List[ToolResponse] = None,
+        response_snapshot: bool,
+        disable_tool_action: bool = False,
+        memory_able: bool = None,
+    ):
+        """
+        Deliver message, release task chain, reply message
+        :param plugin_name: Plugin name
+        :param tool_response: The response of the tool
+        :param memory_able : Whether to write back to history
+        :param response_snapshot: 是否释放任务链，是否释放任务链，比如插件运行失败，错误消息发送的同时需要释放任务链防止挖坟
+        :param disable_tool_action: If the robot is allowed to call tools again
+        :return: Sign
+        """
+        if tool_response is not None:
+            assert isinstance(tool_response, list), "callback must be list"
+        return self.child(plugin_name).update_state(
+            router=Router.DELIVER,
+            memory_able=memory_able,
+            response_snapshot=response_snapshot,
+            disable_tool_action=disable_tool_action,
+            tool_response=tool_response,
+        )
 
+    def reprocess(
+        self,
+        *,
+        plugin_name: str,
+        tool_response: List[ToolResponse],
+        disable_tool_action: bool = False,
+    ):
+        """
+        Reply message, reprocess message raw format, suitable for json/yaml response
+        :param plugin_name: Plugin name
+        :param tool_response: The response of the tool
+        :param disable_tool_action: If the robot is allowed to call tools again
+        """
+        assert isinstance(tool_response, list), "callback must be list"
+        return self.child(plugin_name).update_state(
+            tool_response=tool_response,
+            router=Router.REPROCESS,
+            memory_able=True,
+            response_snapshot=True,
+            disable_tool_action=disable_tool_action,
+        )
 
-class ContentParts(BaseModel):
-    """
-    请求体
-    """
+    def reply(
+        self,
+        *,
+        plugin_name: str,
+        tool_response: List[ToolResponse],
+        disable_tool_action: bool = False,
+    ):
+        """
+        决定路由规则
+        回写消息，释放任务链，回复消息
+        :param plugin_name: 插件名称
+        :param tool_response: 元信息
+        :param disable_tool_action: 是否允许机器人用函数再次处理
+        """
+        assert isinstance(tool_response, list), "callback must be list"
+        return self.child(plugin_name).update_state(
+            tool_response=tool_response,
+            router=Router.REPLIES,
+            memory_able=True,
+            response_snapshot=True,
+            disable_tool_action=disable_tool_action,
+        )
 
-    class Image(BaseModel):
-        url: str
-        detail: Optional[str] = None
+    async def get_pending_tool_call(
+        self, tool_calls_pending_now: str, return_default_if_empty: bool = False
+    ) -> Optional[ToolCall]:
+        """
+        获取当前待处理的函数
+        """
+        if not self.tool_calls_pending:
+            logger.debug("tool_calls is empty")
+            return None
+        if tool_calls_pending_now in self.certify_needed_map:
+            return self.certify_needed_map[tool_calls_pending_now]
+        if return_default_if_empty:
+            return self.tool_calls_pending[0]
+        return None
 
-    type: str
-    image_url: Optional[str]
-    text: Optional[str]
+    async def complete_task(
+        self, tool_calls: ToolCall, success_or_not: bool, run_result: Union[str, dict]
+    ) -> "Sign":
+        """
+        完成此集群
+        self.plan_chain_archive.append((task_batch, run_result))
+        if task_batch in self.plan_chain_pending:
+            self.plan_chain_pending.remove(task_batch)
+        if not self.plan_chain_pending:
+            self.plan_chain_complete = True
+        :return: Sign
+        """
+        self.tool_calls_completed.append((tool_calls, success_or_not, run_result))
+        if tool_calls in self.tool_calls_pending:
+            self.tool_calls_pending.remove(tool_calls)
+        return self
+
+    def get_snapshot_credential(self, tool_calls: ToolCall) -> Optional[str]:
+        """
+        从 Map 获取验证UUID
+        """
+        for key, item in self.certify_needed_map.items():
+            if item == tool_calls:
+                return key
+        return None
 
 
-class Message(BaseModel, ABC):
+class Location(BaseModel):
     """
-    请求体
-    响应体
+    here .... channel
     """
 
-    class Meta(BaseModel):
-        # message_class: Literal[None, "system", "user", "assistant", "tool", "function"] = Field(default="user")
-        index_id: str = Field(default_factory=generate_uid, description="消息ID")
-        """消息ID"""
-
-        datatime: str = Field(default=time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()), description="消息时间")
-        timestamp: int = Field(default=int(time.time()), description="消息时间戳")
-        """消息时间"""
-
-        retrieval: bool = Field(default=False, description="是否可检索")
-        """是否折叠(对抗过长消息，为小上下文模型设计)，同时证明我们可以在消息嵌入重整策略"""
-
-        extra: dict = Field(default_factory=dict, description="额外信息")
-        """额外信息"""
-
-        files: List["File"] = Field(default_factory=list, description="文件信息")
-        """文件信息"""
-
-        @classmethod
-        def default(cls, message_class):
-            return cls(message_class=message_class)
-
-    _meta: "Meta" = PrivateAttr(default=None)
-    """元数据"""
-    role: str
-    content: Union[str, List[ContentParts], List[dict]]
+    platform: str = Field(None, description="platform")
+    user_id: str = Field(None, description="user id")
+    chat_id: str = Field(None, description="guild id(channel in dm)/Telegram chat id")
+    thread_id: Optional[str] = Field(None, description="channel id/Telegram thread")
+    message_id: Optional[str] = Field(None, description="message id")
 
-    def get_meta(self) -> Meta:
-        return self._meta
-
-    def update_meta(self, meta: "Meta") -> "Message":
-        self._meta = meta
+    @model_validator(mode="after")
+    def to_string(self):
+        for key in ["user_id", "chat_id", "thread_id", "message_id"]:
+            if isinstance(getattr(self, key), int):
+                setattr(self, key, str(getattr(self, key)))
         return self
 
     @property
-    def fold(self) -> "Message":
-        return self
-
-    def get_functions(self) -> List["TaskBatch"]:
-        raise NotImplementedError
+    def uid(self):
+        return f"{self.platform}:{self.user_id}"
 
-    @abstractmethod
-    def request_final(self,
-                      schema_model: str,
 
-                      ) -> "Message":
-        """
-        Openai 请求标准格式最终转换根据 message_class 元信息锁定字段
-        :param schema_model: 适配的模型
-        """
-        raise NotImplementedError
+class Plugin(BaseModel):
+    name: str = Field(None, description="插件名称")
+    is_run_out: bool = Field(False, description="是否运行完毕")
+    token_usage: int = Field(0, description="Token 用量")
 
 
-class SystemMessage(Message):
-    role: str = Field(default="system")
-    content: str
-    name: Optional[str] = Field(default=None, description="speaker_name", pattern=r"^[a-zA-Z0-9_]+$")
-
-    def request_final(self,
-                      *,
-                      schema_model: str,
-                      ) -> "Message":
-        return self
-
-
-class UserMessage(Message):
-    role: str = Field(default="user")
-    content: Union[str, List["ContentParts"], List[dict]]
-    name: Optional[str] = Field(default=None, description="speaker_name", pattern=r"^[a-zA-Z0-9_]+$")
-
-    @property
-    def fold(self) -> "Message":
-        """
-        折叠过长特殊类型消息。消息类型为程序自有属性
-        插件定义 fold_id 引诱查询
-        :return: Message
-        """
-        metadata_str = (f"""[FoldText](fold_id={self._meta.index_id}"""
-                        f"""\ntimestamp={self._meta.datatime}"""
-                        f"""\ndescription={self.content[:20] + "..."})"""
-                        )
-        return self.model_copy(
-            update={
-                "content": metadata_str
-            },
-            deep=True
-        )
-
-    def request_final(self,
-                      *,
-                      schema_model: str,
-                      ) -> "Message":
-        """
-        Openai 请求标准格式最终转换根据 message_class 元信息锁定字段
-        :param schema_model: 适配的模型
-        """
-        if "vision" in schema_model:
-            if isinstance(self.content, str):
-                _new_content: List[ContentParts] = [ContentParts(
-                    type="text",
-                    text=self.content
-                )]
-                if self._meta.files:
-                    for file in self._meta.files:
-                        if file.file_url:
-                            _new_content.append(
-                                ContentParts(
-                                    type="image_url",
-                                    image_url=file.file_url
-                                )
-                            )
-                        elif file.file_id:
-                            if file.file_name.endswith(("jpg", "png", "jpeg", "gif", "webp", "svg")):
-                                base64_image = base64.b64encode(
-                                    sync(file.raw_file())
-                                ).decode('utf-8')
-                                _new_content.append(
-                                    ContentParts(
-                                        type="image_url",
-                                        image_url=f"data:image/png;base64,{base64_image}"
-                                    )
-                                )
-                        else:
-                            pass
-                self.content = _new_content
-        return self
-
+class TaskHeader(BaseModel):
+    """
+    任务链节点
+    """
 
-class AssistantMessage(Message):
-    role: str = Field(default="assistant")
-    content: Union[None, str] = Field(default='', description="assistant content")
-    name: Optional[str] = Field(default=None, description="speaker_name", pattern=r"^[a-zA-Z0-9_]+$")
-    tool_calls: Optional[List[ToolCallCompletion]] = Field(default=None, description="tool calls")
-    """a array of tools, for result"""
-    function_call: Optional[FunctionCallCompletion] = Field(default=None, description="Deprecated")
-    """Deprecated by openai ,for result"""
+    task_sign: Sign = Field(Sign(), description="任务元数据")
+    sender: Location = Field(..., description="发信人")
+    receiver: Location = Field(..., description="接收人")
+    message: List[EventMessage] = Field(None, description="消息内容")
 
-    @model_validator(mode="after")
-    def deprecate_validator(self):
-        if self.tool_calls and self.function_call:
-            raise ValidationError("sdk param validator:tool_calls and function_call cannot both be provided")
-        if self.function_call:
-            logger.warning("sdk param validator:function_call is deprecated")
-        if self.content is None:
-            self.content = ""
-        return self
-
-    def get_executor_batch(self) -> List[TaskBatch]:
+    @classmethod
+    def from_sender(
+        cls,
+        event_messages: List[EventMessage],
+        task_sign: Sign,
+        message_id: Optional[str],
+        chat_id: str,
+        user_id: str,
+        platform: str,
+    ):
         """
-        获取插件获取对应的无序函数列表，合并新旧标准
+        从telegram消息中构建任务
         """
-        _calls = []
-        if self.function_call:
-            _calls.append(TaskBatch.from_function_call(self.function_call))
-        _calls.extend([TaskBatch.from_tool_call(tools) for tools in self.tool_calls])
-        # 去None
-        _calls = [_x for _x in _calls if _x]
-        return _calls
+        return cls(
+            task_sign=task_sign,
+            sender=Location(
+                platform=platform,
+                chat_id=chat_id,
+                user_id=user_id,
+                message_id=message_id,
+            ),
+            receiver=Location(
+                platform=platform,
+                chat_id=chat_id,
+                user_id=user_id,
+                message_id=message_id,
+            ),
+            message=event_messages,
+        )
 
-    @property
-    def sign_function(self) -> bool:
+    @classmethod
+    def from_function(
+        cls,
+        llm_response: OpenAIResult,
+        task_sign: Sign,
+        receiver: Location,
+        message: List[EventMessage] = None,
+    ):
         """
-        判断是否有函数需要执行
+        从 Openai LLM Task中构建任务
         """
-        if self.function_call:
-            return True
-        if self.tool_calls:
-            for tol in self.tool_calls:
-                if tol.function:
-                    return True
-        return False
-
-    def request_final(self,
-                      *,
-                      schema_model: str,
-                      ) -> "Message":
-        return self
-
-
-class ToolMessage(Message):
-    role: str = Field(default="tool")
-    content: str
-    tool_call_id: str
-
-    def request_final(self,
-                      *,
-                      schema_model: str,
-                      ) -> "Message":
-        return self
+        # task_sign = task_sign.child("function") 发送到 function 的消息不需加点，因为此时 接收器算发送者
+        task_sign.llm_response = llm_response
+        return cls(
+            task_sign=task_sign, sender=receiver, receiver=receiver, message=message
+        )
 
+    @classmethod
+    def from_discord_hikari(
+        cls,
+        message: hikari.Message,
+        task_sign: Sign,
+        file: List[File] = None,
+        reply: bool = True,
+        hide_file_info: bool = False,
+        deliver_back_message: List[hikari.Message] = None,
+        trace_back_message: List[hikari.Message] = None,
+    ):
+        # none -> []
+        trace_back_message = [] if not trace_back_message else trace_back_message
+        file = [] if not file else file
+        deliver_back_message = [] if not deliver_back_message else deliver_back_message
+
+        def _convert(_message: hikari.Message) -> Optional[EventMessage]:
+            """
+            消息标准化
+            """
+            if not _message:
+                raise ValueError("Message is empty")
+            if isinstance(_message, hikari.Message):
+                user_id = message.author.id
+                chat_id = message.guild_id if message.guild_id else message.channel_id
+                thread_id = message.channel_id
+                text = _message.content
+                created_at = _message.created_at.timestamp()
+            else:
+                raise ValueError(f"Unknown message type {type(_message)}")
+            return EventMessage(
+                user_id=user_id,
+                chat_id=chat_id,
+                thread_id=thread_id,
+                text=text if text else "(empty message)",
+                created_at=str(created_at),
+            )
+
+        deliver_message_list: List[EventMessage] = [
+            _convert(msg) for msg in deliver_back_message
+        ]
+
+        # A
+        _file_name = []
+        for _file in file:
+            _file_name.append(_file.file_prompt)
+        # 转换为标准消息
+        head_message = _convert(message)
+        assert head_message, "HeadMessage is empty"
+        # 附加文件信息
+        head_message.file = file
+        # 追加元信息
+        if not hide_file_info:
+            head_message.text += "\n" + "\n".join(_file_name)
+
+        # 追加回溯消息
+        message_list = []
+        if trace_back_message:
+            for item in trace_back_message:
+                if item:
+                    message_list.append(_convert(item))
+        message_list.extend(deliver_message_list)
+        message_list.append(head_message)
 
-class FunctionMessage(Message):
-    role: str = Field(default="function")
-    content: str
-    name: str
+        # 去掉 None
+        message_list = [item for item in message_list if item]
 
-    @model_validator(mode="after")
-    def function_validator(self):
-        logger.warning("Function Message is deprecated by openai")
-        if self.role == "function" and not self.name:
-            raise ValidationError("sdk param validator:name must be specified when role is function")
-        return self
+        return cls(
+            task_sign=task_sign,
+            sender=cls.Location(
+                platform="discord_hikari",
+                thread_id=message.channel_id,
+                chat_id=message.guild_id if message.guild_id else message.channel_id,
+                user_id=message.author.id,
+                message_id=message.id if reply else None,
+            ),
+            receiver=cls.Location(
+                platform="discord_hikari",
+                thread_id=message.channel_id,
+                chat_id=message.guild_id if message.guild_id else message.channel_id,
+                user_id=message.author.id,
+                message_id=message.id if reply else None,
+            ),
+            message=message_list,
+        )
 
-    def request_final(self,
-                      *,
-                      schema_model: str,
-                      ) -> "Message":
-        """
-        Openai 请求标准格式最终转换根据 message_class 元信息锁定字段
-        :param schema_model: 适配的模型
-        """
-        return self
+    @classmethod
+    def from_kook(
+        cls,
+        message: khl.Message,
+        deliver_back_message: List[khl.Message],
+        trace_back_message: List[khl.Message],
+        task_sign: Sign,
+        hide_file_info: bool = False,
+        file: List[File] = None,
+        reply: bool = True,
+    ):
+        # none -> []
+        trace_back_message = [] if not trace_back_message else trace_back_message
+        file = [] if not file else file
+        deliver_back_message = [] if not deliver_back_message else deliver_back_message
+
+        def _convert(_message: khl.Message) -> Optional[EventMessage]:
+            """
+            消息标准化
+            """
+            if not _message:
+                raise ValueError("Message is empty")
+            if isinstance(_message, khl.Message):
+                user_id = message.author_id
+                chat_id = (
+                    message.ctx.guild.id
+                    if message.ctx.guild
+                    else message.ctx.channel.id
+                )
+                thread_id = message.ctx.channel.id
+                text = _message.content
+                created_at = _message.msg_timestamp
+            else:
+                raise ValueError(f"Unknown message type {type(_message)}")
+            return EventMessage(
+                user_id=user_id,
+                chat_id=chat_id,
+                thread_id=thread_id,
+                text=text if text else "(empty message)",
+                created_at=str(created_at),
+            )
+
+        deliver_message_list: List[EventMessage] = [
+            _convert(msg) for msg in deliver_back_message
+        ]
+
+        # A
+        _file_name = []
+        for _file in file:
+            _file_name.append(_file.file_prompt)
+        # 转换为标准消息
+        head_message = _convert(message)
+        assert head_message, "HeadMessage is empty"
+        # 附加文件信息
+        head_message.file = file
+        # 追加元信息
+        if not hide_file_info:
+            head_message.text += "\n" + "\n".join(_file_name)
+
+        # 追加回溯消息
+        message_list = []
+        if trace_back_message:
+            for item in trace_back_message:
+                if item:
+                    message_list.append(_convert(item))
+        message_list.extend(deliver_message_list)
+        message_list.append(head_message)
 
+        # 去掉 None
+        message_list = [item for item in message_list if item]
 
-def create_short_task(task_desc, refer, role: str = None):
-    """
-    创建单任务模板
-    """
-    if not role:
-        role = (
-            "[RULE]"
-            "Please complete the order according to the task description refer to given information, "
-            "if can't complete, please reply 'give up'"
-        )
-    return [
-        SystemMessage(
-            role="system",
-            content=role,
-        ),
-        UserMessage(
-            role="user",
-            content=f"{refer} <hint>{task_desc}<hint>",
-            name="task"
+        return cls(
+            task_sign=task_sign,
+            sender=cls.Location(
+                platform="kook",
+                thread_id=message.ctx.channel.id,
+                chat_id=message.ctx.guild.id
+                if message.ctx.guild
+                else message.ctx.channel.id,
+                user_id=message.author_id,
+                message_id=message.id if reply else None,
+            ),
+            receiver=cls.Location(
+                platform="kook",
+                thread_id=message.ctx.channel.id,
+                chat_id=message.ctx.guild.id
+                if message.ctx.guild
+                else message.ctx.channel.id,
+                user_id=message.author_id,
+                message_id=message.id if reply else None,
+            ),
+            message=message_list,
         )
-    ]
 
 
-def parse_message_dict(item: dict):
+class Snapshot(BaseModel):
     """
-    将 dict 实例化，用错误hook覆盖
+    快照
     """
-    role = item.get("role", None)
-    if not role:
-        return None
-    try:
-        if role == "assistant":
-            _message = AssistantMessage.model_validate(item)
-        elif role == "user":
-            _message = UserMessage.model_validate(item)
-        elif role == "system":
-            _message = SystemMessage.model_validate(item)
-        elif role == "tool":
-            _message = ToolMessage.model_validate(item)
-        elif role == "function":
-            _message = FunctionMessage.model_validate(item)
-        else:
-            raise CheckError(f"unknown message type {role}")
-    except Exception as e:
-        logger.exception(f"[ParseError]\nparse_message_dict:Unknown message type in redis data:\n{e}")
-        return None
-    else:
-        return _message
 
+    snap_uuid: str = Field(
+        default_factory=lambda: str(shortuuid.uuid()).upper()[:5],
+        description="快照UUID",
+    )
+    snapshot_credential: Optional[str] = None
+    snapshot_data: TaskHeader
+    creator: str
+    channel: str
+    expire_at: int
+    created_at: int = Field(default_factory=lambda: int(time.time()))
+    processed_at: Optional[int] = None
 
-def standardise_for_request(
-        *,
-        message: "Message",
-        schema_model: str
-) -> "Message":
-    """
-    标准化转换，供请求使用
-    """
-    if isinstance(message, dict):
-        message = Message.model_validate(message)
-    if hasattr(message, "message"):
-        return message.request_final(schema_model=schema_model)
-    else:
-        return message
-
-
-def generate_short_md5(data: Union[bytes, str, BytesIO],
-                       *,
-                       length: int = 8,
-                       upper: bool = True,
-                       ):
-    assert 0 < length <= 32, "length must be less than 32"
-    # 计算 MD5 哈希值
-    md5_hash = hashlib.md5()
-    if isinstance(data, bytes) or isinstance(data, BytesIO):
-        if isinstance(data, BytesIO):
-            data = data.getvalue()
-        with BytesIO(data) as file:
-            for chunk in iter(lambda: file.read(4096), b""):
-                md5_hash.update(chunk)
-    if isinstance(data, str):
-        md5_hash.update(data.encode("utf-8"))
-    # 获取哈希值的 16 进制表示
-    hex_digest = md5_hash.hexdigest()
-    # 生成唯一的短ID
-    short_id = str(hex_digest[:length])
-    if upper:
-        short_id = short_id.upper()
-    return short_id
+    @property
+    def processed(self) -> bool:
+        return self.processed_at is not None
```

### Comparing `llmkira-0.27.3/llmkira/sdk/utils.py` & `llmkira-1.0.0/llmkira/sdk/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,41 +5,41 @@
 
 同步执行异步函数
 """
 import asyncio
 import hashlib
 import tempfile
 from bisect import bisect_left
-from typing import Coroutine, Dict, List, Optional
+from typing import Coroutine, Optional
+from urllib.parse import urlparse
 
 import aiohttp
 import ffmpeg
 import nest_asyncio
 import shortuuid
 from loguru import logger
-from telebot import formatting
-from telebot.formatting import escape_markdown
 
 nest_asyncio.apply()
 
 
+def is_valid_url(url):
+    try:
+        result = urlparse(url)
+        return all([result.scheme, result.netloc])
+    except ValueError:
+        return False
+
+
 def __ensure_event_loop():
     try:
         asyncio.get_event_loop()
-    except Exception:
+    except Exception as e:  # noqa
         asyncio.set_event_loop(asyncio.new_event_loop())
 
 
-def dict2message(data: Dict[str, str]) -> List[str]:
-    _res = []
-    for key, value in data.items():
-        _res.append("".join([formatting.mitalic(key), escape_markdown("="), f"`{escape_markdown(value)}`"]))
-    return _res
-
-
 def sync(coroutine: Coroutine):
     """
     同步执行异步函数，使用可参考 [同步执行异步代码](https://nemo2011.github.io/bilibili-api/#/sync-executor)
 
     Args:
         coroutine (Coroutine): 异步函数
 
@@ -52,91 +52,99 @@
 
 
 def sha1_encrypt(string):
     """
     sha1加密算法
     """
 
-    sha = hashlib.sha1(string.encode('utf-8'))
+    sha = hashlib.sha1(string.encode("utf-8"))
     encrypts = sha.hexdigest()
     return encrypts[:8]
 
 
 def generate_uid():
     return shortuuid.uuid()[0:8].upper()
 
 
-async def aiohttp_download_file(url,
-                                session: aiohttp.ClientSession = None,
-                                timeout=None,
-                                size_limit=None,
-                                headers=None,
-                                **kwargs):
+async def aiohttp_download_file(
+    url,
+    session: aiohttp.ClientSession = None,
+    timeout=None,
+    size_limit=None,
+    headers=None,
+    **kwargs,
+):
     if not session:
         session = aiohttp.ClientSession()
     async with session as session:
-        async with session.get(url,
-                               timeout=timeout,
-                               headers=headers, **kwargs
-                               ) as response:
+        async with session.get(
+            url, timeout=timeout, headers=headers, **kwargs
+        ) as response:
             if response.status != 200:
                 raise Exception("无法下载文件")
 
             content_length = response.content_length
             if size_limit and content_length and content_length > size_limit:
                 raise Exception("文件大小超过限制")
 
             contents = await response.read()
             return contents
 
 
 class Ffmpeg(object):
     @staticmethod
-    def convert(*,
-                input_c: str = "mp3",
-                output_c: str = "ogg",
-                stream_data: bytes = None,
-                quiet=False
-                ) -> Optional[bytes]:
+    def convert(
+        *,
+        input_c: str = "mp3",
+        output_c: str = "ogg",
+        stream_data: bytes = None,
+        quiet=False,
+    ) -> Optional[bytes]:
         """
         使用ffmpeg转换音频格式
         :param input_c: 输入音频格式
         :param output_c: 输出音频格式
         :param stream_data: 输入音频流
         :param quiet: 是否静默
         """
         if not input_c.startswith("."):
             input_c = "." + input_c
         if not output_c.startswith("."):
             output_c = "." + output_c
-        in_fd, temp_filename = tempfile.mkstemp(suffix=input_c, prefix=None, dir=None, text=False)
-        out_fd, out_temp_filename = tempfile.mkstemp(suffix=output_c, prefix=None, dir=None, text=False)
+        in_fd, temp_filename = tempfile.mkstemp(
+            suffix=input_c, prefix=None, dir=None, text=False
+        )
+        out_fd, out_temp_filename = tempfile.mkstemp(
+            suffix=output_c, prefix=None, dir=None, text=False
+        )
         _bytes = None
         try:
             # 写入文件
             with open(temp_filename, "wb") as f:
                 f.write(stream_data)
             stream = ffmpeg.input(filename=temp_filename)
             if output_c == ".ogg":
-                stream = ffmpeg.output(stream, filename=out_temp_filename, acodec="libopus")
+                stream = ffmpeg.output(
+                    stream, filename=out_temp_filename, acodec="libopus"
+                )
             else:
                 stream = ffmpeg.output(stream, filename=out_temp_filename)
             stream = ffmpeg.overwrite_output(stream)
-            _ = ffmpeg.run(stream_spec=stream,
-                           quiet=quiet
-                           )
+            _ = ffmpeg.run(stream_spec=stream, quiet=quiet)
             # 读取文件
             import os
+
             _bytes = os.read(out_fd, os.path.getsize(out_temp_filename))
             assert _bytes, "ffmpeg convert failed"
         except Exception as e:
             logger.error(f"ffmpeg convert failed {e}")
             raise e
         finally:
             import os
+
             os.close(in_fd)
             os.close(out_fd)
             os.remove(out_temp_filename)
             os.remove(temp_filename)
         return _bytes
```

### Comparing `llmkira-0.27.3/llmkira/task/__init__.py` & `llmkira-1.0.0/llmkira/task/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,39 +7,36 @@
 
 import aio_pika
 from aio_pika import Message, DeliveryMode
 from aiormq import DeliveryError
 from loguru import logger
 from pamqp.commands import Basic
 
+from app.setting.database import RabbitMQSetting
 from .schema import TaskHeader
 
 EXPIRATION_SECOND = 60 * 5  # 5min
 QUEUE_MAX_LENGTH = 120
 X_OVERFLOW = "reject-publish"  # 拒绝
-CONSUMER_PREFETCH_COUNT = 12  # 消息流控
+CONSUMER_PREFETCH_COUNT = 20  # 消息流控
 QUEUE_ARGUMENTS = {
     "x-max-length": QUEUE_MAX_LENGTH,  # 上限
     # "message-ttl": EXPIRATION_SECOND * 1000,
-    "x-overflow": X_OVERFLOW  # 拒绝
+    "x-overflow": X_OVERFLOW,  # 拒绝
 }
 
 
 class Task(object):
-    def __init__(self, *,
-                 queue: str,
-                 amqp_dsn: str = None
-                 ):
+    def __init__(self, *, queue: str, amqp_dsn: str = None):
         """
-        :param queue: 队列名字
-        :param amqp_dsn: 队列数据库
+        :param queue: The name of the queue started by the task
+        :param amqp_dsn: Address of the RabbitMQ server
         """
         self.queue_name = queue
         if amqp_dsn is None:
-            from ..setting.rabbitmq import RabbitMQSetting
             amqp_dsn = RabbitMQSetting.amqp_dsn
         self._amqp_url = amqp_dsn
 
     async def send_task(self, task: TaskHeader):
         connection = await aio_pika.connect_robust(self._amqp_url)
         async with connection:
             channel = await connection.channel(
@@ -47,50 +44,56 @@
             )
             # 通道超时 2s
             # await channel.initialize(timeout=2000)
             # Creating a message
             message = Message(
                 body=task.model_dump_json().encode("utf-8"),
                 delivery_mode=DeliveryMode.PERSISTENT,
-                expiration=EXPIRATION_SECOND
+                expiration=EXPIRATION_SECOND,
             )
             # Declaring queue
             try:
                 await channel.declare_queue(
                     self.queue_name,
                     arguments=QUEUE_ARGUMENTS,
-                    durable=True  # 持续化
+                    durable=True,  # 持续化
                 )
             except Exception as e:
                 logger.error(
                     f"[5941163]Rabbitmq Queue param validation error, try deleting the abnormal "
                     f"queue manually and retrying. "
                     f"\n--error {e}"
                     f"\n--help |web: <database_ip>:15672/#/ |shell: `rabbitmqctl delete_queue {self.queue_name}`"
                 )
                 raise e
             # Sending the message
             try:
                 confirmation = await channel.default_exchange.publish(
-                    message,
-                    routing_key=self.queue_name,
-                    timeout=10
+                    message, routing_key=self.queue_name, timeout=10
                 )
             except DeliveryError as e:
-                logger.error(f"[502231]Task Delivery failed with exception: {e.reason}")
-                return False, "🔭 Sorry,failure to reach the control centre, possibly i reach design limit 🧯"
+                logger.error(
+                    f"[502231] Task Delivery failed with exception: {e.reason}"
+                )
+                return (
+                    False,
+                    "🔭 Sorry,failure to reach the control centre, possibly i reach design limit 🧯",
+                )
             except TimeoutError:
-                logger.error(f"[528532]Task Delivery timeout")
+                logger.error("[528532] Task Delivery timeout")
                 return False, "🔭 Sorry, failure to reach the control centre, ⏱ timeout"
             else:
                 if not isinstance(confirmation, Basic.Ack):
-                    logger.error(f"[552123]Task Delivery failed with confirmation")
-                    return False, "🔭 Sorry, failure to reach the control centre, sender error"
+                    logger.error("[552123]Task Delivery failed with confirmation")
+                    return (
+                        False,
+                        "🔭 Sorry, failure to reach the control centre, sender error",
+                    )
                 else:
-                    logger.info("[621132]Task sent success")
+                    logger.info("[621132] Task sent success")
                     return True, "Task sent success"
 
     async def consuming_task(self, func: callable):
         connection = await aio_pika.connect_robust(self._amqp_url)
         async with connection:
             # Creating a channel
             channel = await connection.channel()
@@ -99,29 +102,25 @@
             await channel.set_qos(prefetch_count=CONSUMER_PREFETCH_COUNT)  # 消息流控
 
             # Declaring queue
             try:
                 queue = await channel.declare_queue(
                     self.queue_name,
                     arguments=QUEUE_ARGUMENTS,
-                    durable=True  # 持续化
+                    durable=True,  # 持续化
                 )
             except Exception as e:
                 logger.error(
                     f"[502231]Rabbitmq Queue parameter validation failed, try deleting the abnormal queue manually "
                     f"and retrying."
                     f"\n--error {e}"
                     f"\n--help |web: <database_ip>:15672/#/ |shell: `rabbitmqctl delete_queue {self.queue_name}`"
                 )
                 raise e
             await queue.consume(func)
             await asyncio.Future()  # run forever
 
     @classmethod
-    async def create_and_send(cls,
-                              *,
-                              queue_name: str,
-                              task: TaskHeader
-                              ):
+    async def create_and_send(cls, *, queue_name: str, task: TaskHeader):
         sender = cls(queue=queue_name)
         await sender.send_task(task=task)
         return sender
```

### Comparing `llmkira-0.27.3/pyproject.toml` & `llmkira-1.0.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmkira"
-version = "0.27.3"
+version = "1.0.0"
 description = "A chain message bot based on OpenAI"
 authors = [
     { name = "sudoskys", email = "me@dianas.cyou" },
     { name = "llmkira", email = "me@dianas.cyou" },
 ]
 dependencies = [
     "pathlib>=1.0.1",
@@ -25,42 +25,49 @@
     "fasttext-wheel<1.0.0,>=0.9.2",
     "tenacity<9.0.0,>=8.2.3",
     "pysocks<2.0.0,>=1.7.1",
     "flask-sqlalchemy<4.0.0,>=3.1.1",
     "emoji<3.0.0,>=2.8.0",
     "websocket<1.0.0,>=0.2.1",
     "wrapt<2.0.0,>=1.11.0",
-    "motor<4.0.0,>=3.3.1",
     "dynaconf<4.0.0,>=3.2.3",
     "rich<14.0.0,>=13.6.0",
     "importlib-metadata<7.0.0,>=6.8.0",
     "sentry-sdk<2.0.0,>=1.34.0",
     "boltons<24.0.0,>=23.1.1",
     "orjson<4.0.0,>=3.9.10",
     "pydantic-settings<3.0.0,>=2.0.3",
     "docstring-parser<1.0,>=0.15",
     "polling<1.0.0,>=0.3.2",
     "elara<1.0.0,>=0.5.5",
-    "apscheduler<4.0.0,>=3.10.4",
     "tzlocal<6.0,>=5.2",
     "nltk<4.0.0,>=3.8.1",
     "jieba<1.0.0,>=0.42.1",
     "scikit-learn<2.0.0,>=1.3.2",
     "cjieba<1.0.0,>=0.4.4",
     "requests[socks]<3.0.0,>=2.31.0",
     "feedparser<7.0.0,>=6.0.10",
     "pillow<11.0.0,>=10.1.0",
     "inscriptis<3.0.0,>=2.3.2",
     "aiohttp<4.0.0,>=3.8.6",
     "pytelegrambotapi<5.0.0,>=4.14.0",
     "ffmpeg-python<1.0.0,>=0.2.0",
     "duckduckgo-search<4.0.0,>=3.9.5",
     "flask<4.0.0,>=3.0.0",
+    "telegramify-markdown>=0.1.2",
+    "json-repair>=0.13.0",
+    "curl-cffi>=0.6.2",
+    "deprecated>=1.2.14",
+    "aiofile>=3.8.8",
+    "file-read-backwards>=3.0.0",
+    "apscheduler>=3.10.4",
+    "montydb[lmdb]>=2.5.2",
+    "pymongo>=4.6.3",
 ]
-requires-python = ">=3.8,<3.12"
+requires-python = ">=3.9,<3.12"
 readme = "README.md"
 keywords = [
     "llmbot",
     "llmkira",
     "openai",
     "chatgpt",
     "telegram",
```

### Comparing `llmkira-0.27.3/PKG-INFO` & `llmkira-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: llmkira
-Version: 0.27.3
+Version: 1.0.0
 Summary: A chain message bot based on OpenAI
-Keywords: llmbot llmkira openai chatgpt telegram bot
+Keywords: llmbot,llmkira,openai,chatgpt,telegram,bot
 Home-page: https://llmkira.github.io/Docs/
 Author-Email: sudoskys <me@dianas.cyou>, llmkira <me@dianas.cyou>
 License: GPL3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Project-URL: Homepage, https://llmkira.github.io/Docs/
 Project-URL: Repository, https://github.com/LlmKira/Openaibot
-Requires-Python: <3.12,>=3.8
+Requires-Python: <3.12,>=3.9
 Requires-Dist: pathlib>=1.0.1
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: httpx>=0.24.1
 Requires-Dist: socksio<2.0.0,>=1.0.0
 Requires-Dist: python-dotenv<2.0.0,>=1.0.0
 Requires-Dist: redis>=4.5.4
@@ -29,40 +29,47 @@
 Requires-Dist: fasttext-wheel<1.0.0,>=0.9.2
 Requires-Dist: tenacity<9.0.0,>=8.2.3
 Requires-Dist: pysocks<2.0.0,>=1.7.1
 Requires-Dist: flask-sqlalchemy<4.0.0,>=3.1.1
 Requires-Dist: emoji<3.0.0,>=2.8.0
 Requires-Dist: websocket<1.0.0,>=0.2.1
 Requires-Dist: wrapt<2.0.0,>=1.11.0
-Requires-Dist: motor<4.0.0,>=3.3.1
 Requires-Dist: dynaconf<4.0.0,>=3.2.3
 Requires-Dist: rich<14.0.0,>=13.6.0
 Requires-Dist: importlib-metadata<7.0.0,>=6.8.0
 Requires-Dist: sentry-sdk<2.0.0,>=1.34.0
 Requires-Dist: boltons<24.0.0,>=23.1.1
 Requires-Dist: orjson<4.0.0,>=3.9.10
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.3
 Requires-Dist: docstring-parser<1.0,>=0.15
 Requires-Dist: polling<1.0.0,>=0.3.2
 Requires-Dist: elara<1.0.0,>=0.5.5
-Requires-Dist: apscheduler<4.0.0,>=3.10.4
 Requires-Dist: tzlocal<6.0,>=5.2
 Requires-Dist: nltk<4.0.0,>=3.8.1
 Requires-Dist: jieba<1.0.0,>=0.42.1
 Requires-Dist: scikit-learn<2.0.0,>=1.3.2
 Requires-Dist: cjieba<1.0.0,>=0.4.4
 Requires-Dist: requests[socks]<3.0.0,>=2.31.0
 Requires-Dist: feedparser<7.0.0,>=6.0.10
 Requires-Dist: pillow<11.0.0,>=10.1.0
 Requires-Dist: inscriptis<3.0.0,>=2.3.2
 Requires-Dist: aiohttp<4.0.0,>=3.8.6
 Requires-Dist: pytelegrambotapi<5.0.0,>=4.14.0
 Requires-Dist: ffmpeg-python<1.0.0,>=0.2.0
 Requires-Dist: duckduckgo-search<4.0.0,>=3.9.5
 Requires-Dist: flask<4.0.0,>=3.0.0
+Requires-Dist: telegramify-markdown>=0.1.2
+Requires-Dist: json-repair>=0.13.0
+Requires-Dist: curl-cffi>=0.6.2
+Requires-Dist: deprecated>=1.2.14
+Requires-Dist: aiofile>=3.8.8
+Requires-Dist: file-read-backwards>=3.0.0
+Requires-Dist: apscheduler>=3.10.4
+Requires-Dist: montydb[lmdb]>=2.5.2
+Requires-Dist: pymongo>=4.6.3
 Requires-Dist: hikari==2.0.0.dev121; extra == "bot"
 Requires-Dist: hikari-crescent<1.0.0,>=0.6.4; extra == "bot"
 Requires-Dist: khl-py<1.0.0,>=0.3.17; extra == "bot"
 Requires-Dist: slack-bolt<2.0.0,>=1.18.0; extra == "bot"
 Requires-Dist: hikari==2.0.0.dev121; extra == "testing"
 Requires-Dist: hikari-crescent<1.0.0,>=0.6.4; extra == "testing"
 Requires-Dist: khl-py<1.0.0,>=0.3.17; extra == "testing"
@@ -96,192 +103,160 @@
 </a>
 <a href="https://hub.docker.com/repository/docker/sudoskys/llmbot/builds">
     <img src="https://img.shields.io/docker/v/sudoskys/llmbot" alt="docker build">
 </a>
 </p>
 
 <p align="center">
-  <a href="https://llmkira.github.io/Docs/">🍩 部署文档</a> 
+  <a href="https://llmkira.github.io/Docs/">🍩 Deploy Docs</a>
   &
-  <a href="https://llmkira.github.io/Docs/dev/basic">🧀 开发文档</a>
+  <a href="https://llmkira.github.io/Docs/dev/basic">🧀 Dev Docs</a>
   &
-  <a href="README_EN.md">📝 English Readme</a>
-  &
-  <a href="CONTRIBUTING.md">🤝 贡献必看</a>
+  <a href=".github/CONTRIBUTING.md">🤝 Contribute</a>
 </p>
 
+> Don't hesitate to Star ⭐️, Issue 📝, and PR 🛠️
 
-> **Look for English README? Click [here](README_EN.md). We also have English
-documentation [here](https://llmkira.github.io/Docs/en).**
-
-> 部署遇到问题？提交 Issue 帮助我们提升可用性
+> Python>=3.9
 
-此项目为自部署，实用可扩展的机器人核心，以 `FunctionCall` `ToolCall` 为核心，支持多种消息平台。
+This project uses the ToolCall feature.
 
-采用消息队列，很好处理函数请求，支持繁杂的插件和功能设计。良好支持文件系统。
+It integrates a message queuing and snapshot system, offering plugin mechanisms and authentication prior to plugin
+execution.
 
-支持多种模型源，支持跨平台消息转发。
+The model adheres to the Openai Schema, other models are not supported. Please adapt using gateways independently.
 
 | Demo                              |
-|-----------------------------------| 
-| ![sticker](./docs/chain_chat.gif) | 
-
-与之前的项目不同的是，此项目尝试基于消息平台复刻 ChatGpt 的插件系统，实现部分或更进一步的功能。
+|-----------------------------------|
+| ![sticker](./docs/chain_chat.gif) |
 
-> 因为 func call 为 feature,所以只支持 Openai 类型的 api, 不打算支持没有 func call 的 LLM
+## 🍔 Roadmap
 
-## 📦 Feature
+- [x] Removal of legacy code
+- [x] Deletion of metric system
+- [x] Deletion of model selection system, unified to OpenAI Schema
+- [x] Implementation of a more robust plugin system
+- [x] Project structure simplification
+- [x] Elimination of the Provider system
+
+## 📦 Features
+
+- 🍪 A comprehensive plugin development ecosystem, adopting a classic design, and seamless integration with plugins
+  through `pip` installation
+- 📝 Message system with no time or sender constraints, offering fully decoupled logics
+- 📬 Offers Login via a URL mechanism, providing a flexible and expandable authentication development solution
+- 🍰 Empowers users to authorize plugin execution. Users can configure plugin environment variables at their discretion
+- 📦 Support for plugins to access files
+- 🍟 Multi-platform support – extend new platforms by inheriting the base class
+- 🍔 Plugins can determine their appearance in new sessions dynamically, preventing performance degradation despite large
+  amounts of plugins
+
+### 🍔 Login Modes
+
+- `Login via url`: Use `/login token#https://provider.com` to Login. The program posts the token to the interface to
+  retrieve configuration information
+- `Login`: Use `/login https://api.com/v1#key#model` to login
 
-- 🍪 完善的插件开发生态，采用经典设计，通过 `pip` 安装即可使用
-- 📝 消息系统，不限时间，不限发送端，定义发送接收者，逻辑完全解耦
-- 📎 路由消息，自定义消息路由，以路由决定运作方式
-- 📬 公共开放限额/私人自配置后端/代理Token认证，提供灵活可扩展的鉴权开发方案
-- 🍾 支持中间件拦截开发，开发扩展即可操作流程前后数据
-- 🎵 细化的统计系统，轻松统计使用情况
-- 🍰 支持插件人在回路验证，可鉴权，可设置插件黑名单
-- 📦 完善标准的文件交互支持，上传/下载文件
-- 🍖 支持个人单独配置环境密钥，为插件提供个人的私有环境变量
-- 🍟 支持大语言模型增量支持，支持多平台扩展，继承标准类即可适配
-- 🍔 同时支持 `FunctionCall` `ToolCall` 特性，根据模型动态构建需要的函数类
+### 🧀 Plugin Previews
 
-### 🧀 部分插件预览
-
-| Sticker Converter                   | Timer Func                      | Translate Func                               |
+| Sticker Converter                   | Timer Function                  | Translate Function                           |
 |-------------------------------------|---------------------------------|----------------------------------------------|
 | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/timer_func.gif) | ![translate](./docs/translate_file_func.gif) |
 
-### 🧀 认证系统介绍
-
-我们采用的认证系统称为 `Service Provider`，即服务提供商，它的作用是为每个发送者分配 Endpoint/Key/Model ，用于鉴权。
-拥有一个 `token` 作为绑定的 OpenKey。程序会调用设定的 `Service Provider` 读取私有 Key/配置 Token 来获取鉴权信息。
-
-![auth](./docs/SeriveProvider.svg)
-
-认证组件和后端均需要自行实现。
-
-### 🎬 平台支持
-
-| 平台       | 支持情况 | 文件系统 | 备注          |
-|----------|------|------|-------------|
-| Telegram | ✅    | ✅    |             |
-| Discord  | ✅    | ✅    |             |
-| Kook     | ✅    | ✅    | 不支持 `被回复启动` |
-| Slack    | ✅    | ✅    | 不支持 `被回复启动` |
-| QQ       | ❌    |      |             |
-| Wechat   | ❌    |      |             |
-| Twitter  | ❌    |      |             |
-| Matrix   | ❌    |      |             |
-| IRC      | ❌    |      |             |
-| ...      |      |      | 创建Issue/PR  |
-
-## 📦 快速开始
+### 🎬 Platform Support
 
-阅读 [🧀 部署文档](https://llmkira.github.io/Docs/) 获得更多信息。
+| Platform | Support | File System | Remarks                                |
+|----------|---------|-------------|----------------------------------------|
+| Telegram | ✅       | ✅           |                                        |
+| Discord  | ✅       | ✅           |                                        |
+| Kook     | ✅       | ✅           | Does not support `triggering by reply` |
+| Slack    | ✅       | ✅           | Does not support `triggering by reply` |
+| QQ       | ❌       |             |                                        |
+| Wechat   | ❌       |             |                                        |
+| Twitter  | ❌       |             |                                        |
+| Matrix   | ❌       |             |                                        |
+| IRC      | ❌       |             |                                        |
+| ...      |         |             | Create Issue/PR                        |
 
-请提前用 `pdm run python3 start_sender.py`  `pdm run python3 start_receiver.py` 测试是否能正常运行。
+## 📦 Quick Start
 
-#### 性能指标测试(Until 2023/11/1)
+Refer to the [🧀 Deployment Document](https://llmkira.github.io/Docs/) for more information.
 
-注意，不包括pm2，redis，rabbitmq，mongodb，docker等服务的内存占用。
-
-| 进程         | 内存均值      | 测算命令                                             | client   |
-|------------|-----------|--------------------------------------------------|----------|
-| `receiver` | 120.202MB | `python3 -m memray run --live start_receiver.py` | telegram |
-| `sender`   | 83.375MB  | `python3 -m memray run --live start_sender.py`   | telegram |
+```shell
+# Install RabbitMQ
+docker pull rabbitmq:3.10-management
+docker run -d -p 5672:5672 -p 15672:15672 \
+  -e RABBITMQ_DEFAULT_USER=admin \
+  -e RABBITMQ_DEFAULT_PASS=8a8a8a \
+  --hostname myRabbit \
+  --name rabbitmq \
+  rabbitmq:3.10-management
+docker ps -l
+# Install Project
+pip install pdm
+pdm install -G bot
+cp .env.exp .env && nano .env
+# Test
+pdm run python3 start_sender.py
+pdm run python3 start_receiver.py
+# Host
+pdm start pm2.json
+```
 
 ### 🥣 Docker
 
 Build Hub: [sudoskys/llmbot](https://hub.docker.com/repository/docker/sudoskys/llmbot/general)
 
-#### 自动 Docker/Docker-compose安装
-
-如果你在使用一台崭新的服务器，你可以使用下面的Shell来尝试自动安装本项目。
+#### Automatic Docker/Docker-compose Installation
 
-此脚本会自动使用 Docker 方法安装所需服务并映射端口，如果您已经部署了 `redis` ，`rabbitmq` ，`mongodb` 。
+If you are using a brand new server, you can use the following shell to automatically install this project.
 
-请自行修改 `docker-compose.yml` 文件。
+This script automatically installs the required services and maps ports using Docker methods. If you have
+deployed `redis`, `rabbitmq`, `mongodb`, please modify the `docker-compose.yml` file accordingly.
 
 ```shell
-
 curl -sSL https://raw.githubusercontent.com/LLMKira/Openaibot/main/deploy.sh | bash
 ```
 
-#### 手动 Docker-compose安装
+#### Manual Docker-compose Installation
 
 ```shell
 git clone https://github.com/LlmKira/Openaibot.git
 cd Openaibot
 cp .env.exp .env&&nano .env
 docker-compose -f docker-compose.yml up -d
-
 ```
 
-更新镜像使用 `docker-compose pull`。
+Update image using `docker-compose pull`.
 
-在 docker 中查看 Shell，使用 `docker exec -it llmbot /bin/bash`，输入 `exit` 退出。
+Use `docker exec -it llmbot /bin/bash` to view Shell in Docker, enter `exit` to exit.
 
-### 🍔 Shell
-
-人工使用Pm2启动，需要自行安装 `redis` ，`rabbitmq` ，`mongodb` 。
-
-```shell
-git clone https://github.com/LlmKira/Openaibot.git
-pip install pdm
-cd Openaibot
-pdm install -G bot
-cp .env.exp .env && nano .env
-apt install npm -y && npm install pm2 && pm2 start pm2.json
-pm2 monit
-
-```
-
-重启程序使用 `pm2 restart pm2.json` 。
-
-> 推荐使用 `pdm` 进行依赖管理，因为我们使用了 `pydantic^1.9.0`，为了防止出现版本冲突，我们使用了 `pdm` 进行依赖管理。
-
-## 🍪 Slash Command
+## 🍪 Slash Commands
 
 ```shell
-clear - 删除聊天记录
-help - 显示文档
-chat - 对话
-task - 启用函数以对话
-ask - 禁止函数以对话
-tool - 列出所有函数
-set_endpoint - 设置私有 key 和 endpoint
-clear_endpoint - 清除私有 key 和 endpoint
-auth - 授权一个函数
-env - 函数环境变量
-token - 绑定令牌
-token_clear - 清除令牌绑定
-func_ban - 禁用一个函数
-func_unban - 解禁一个函数
-bind - 绑定消息源
-unbind - 解绑消息源
+clear - Deletes chat records
+help - Displays documentation
+chat - Conversation
+task - Use a function to converse
+ask - Disable function-based conversations
+tool - Lists all functions
+login - Login
+auth - Authorize a function
+env - Environment variables of the function
 ```
 
-## 💻 如何开发插件？
-
-插件开发文档请参考 `plugins` 目录下的示例插件和 [🧀 插件开发文档](https://llmkira.github.io/Docs/dev/basic)
-
-## 🤝 We need your help!
-
-This is a long term project and we started the development of the LLM APP very early!
-
-We applied a plugin-like system and search online before GPT3 OpenaiApi was released(davinci-003)
-
-After many iterations, we have worked hard to make this project more standardized, generic, and open.
+## 💻 How to Develop Plugins?
 
-We can't do it on our own at the moment:
+Refer to the example plugins in the `plugins` directory and
+the [🧀 Plugin Development Document](https://llmkira.github.io/Docs/dev/basic) for plugin development documentation.
 
-- [ ] We need help with the documentation
-- [ ] Web UI
+## 🧀 Sponsor
 
-Feel free to submit a Pull Request or discuss, we'd love to receive your contribution!
+[![sponsor](./.github/sponsor_ohmygpt.png)](https://www.ohmygpt.com)
 
-## 📜 告知
+## 📜 Notice
 
-> 此项目与 Openai 官方无关，全称为 OpenAiBot，表示开放人工智能机器人，并不表示为 Openai 所属机器人。
+> This project, named OpenAiBot, signifying "Open Artificial Intelligence Robot", is not officially affiliated with
+> OpenAI.
 
-> 如果您所在辖区禁止使用 Openai 服务，请勿使用此项目。
 
-[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot.svg?type=small)](https://app.fossa.com/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot?ref=badge_small)
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot.svg?type=small)](https://app.fossa.com/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot?ref=badge_small)
```

#### html2text {}

```diff
@@ -1,140 +1,114 @@
-Metadata-Version: 2.1 Name: llmkira Version: 0.27.3 Summary: A chain message
-bot based on OpenAI Keywords: llmbot llmkira openai chatgpt telegram bot Home-
-page: https://llmkira.github.io/Docs/ Author-Email: sudoskys
+Metadata-Version: 2.1 Name: llmkira Version: 1.0.0 Summary: A chain message bot
+based on OpenAI Keywords: llmbot,llmkira,openai,chatgpt,telegram,bot Home-page:
+https://llmkira.github.io/Docs/ Author-Email: sudoskys
 dianas.cyou>, llmkira
 dianas.cyou> License: GPL3 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Project-URL: Homepage, https:
 //llmkira.github.io/Docs/ Project-URL: Repository, https://github.com/LlmKira/
-Openaibot Requires-Python: <3.12,>=3.8 Requires-Dist: pathlib>=1.0.1 Requires-
+Openaibot Requires-Python: <3.12,>=3.9 Requires-Dist: pathlib>=1.0.1 Requires-
 Dist: pydantic>=2.0.0 Requires-Dist: loguru>=0.5.3 Requires-Dist: httpx>=0.24.1
 Requires-Dist: socksio<2.0.0,>=1.0.0 Requires-Dist: python-dotenv<2.0.0,>=1.0.0
 Requires-Dist: redis>=4.5.4 Requires-Dist: aio-pika<10.0.0,>=9.3.0 Requires-
 Dist: arclet-alconna<2.0.0,>=1.7.26 Requires-Dist: shortuuid<2.0.0,>=1.0.11
 Requires-Dist: tiktoken<1.0.0,>=0.5.1 Requires-Dist: nest-asyncio<2.0.0,>=1.5.8
 Requires-Dist: contextvars<3.0,>=2.4 Requires-Dist:
 pytz<2024.0.0,>=2023.3.post1 Requires-Dist: numpy<2.0.0,>=1.24.0 Requires-Dist:
 fasttext-wheel<1.0.0,>=0.9.2 Requires-Dist: tenacity<9.0.0,>=8.2.3 Requires-
 Dist: pysocks<2.0.0,>=1.7.1 Requires-Dist: flask-sqlalchemy<4.0.0,>=3.1.1
 Requires-Dist: emoji<3.0.0,>=2.8.0 Requires-Dist: websocket<1.0.0,>=0.2.1
-Requires-Dist: wrapt<2.0.0,>=1.11.0 Requires-Dist: motor<4.0.0,>=3.3.1
-Requires-Dist: dynaconf<4.0.0,>=3.2.3 Requires-Dist: rich<14.0.0,>=13.6.0
-Requires-Dist: importlib-metadata<7.0.0,>=6.8.0 Requires-Dist: sentry-
-sdk<2.0.0,>=1.34.0 Requires-Dist: boltons<24.0.0,>=23.1.1 Requires-Dist:
-orjson<4.0.0,>=3.9.10 Requires-Dist: pydantic-settings<3.0.0,>=2.0.3 Requires-
-Dist: docstring-parser<1.0,>=0.15 Requires-Dist: polling<1.0.0,>=0.3.2
-Requires-Dist: elara<1.0.0,>=0.5.5 Requires-Dist: apscheduler<4.0.0,>=3.10.4
+Requires-Dist: wrapt<2.0.0,>=1.11.0 Requires-Dist: dynaconf<4.0.0,>=3.2.3
+Requires-Dist: rich<14.0.0,>=13.6.0 Requires-Dist: importlib-
+metadata<7.0.0,>=6.8.0 Requires-Dist: sentry-sdk<2.0.0,>=1.34.0 Requires-Dist:
+boltons<24.0.0,>=23.1.1 Requires-Dist: orjson<4.0.0,>=3.9.10 Requires-Dist:
+pydantic-settings<3.0.0,>=2.0.3 Requires-Dist: docstring-parser<1.0,>=0.15
+Requires-Dist: polling<1.0.0,>=0.3.2 Requires-Dist: elara<1.0.0,>=0.5.5
 Requires-Dist: tzlocal<6.0,>=5.2 Requires-Dist: nltk<4.0.0,>=3.8.1 Requires-
 Dist: jieba<1.0.0,>=0.42.1 Requires-Dist: scikit-learn<2.0.0,>=1.3.2 Requires-
 Dist: cjieba<1.0.0,>=0.4.4 Requires-Dist: requests[socks]<3.0.0,>=2.31.0
 Requires-Dist: feedparser<7.0.0,>=6.0.10 Requires-Dist: pillow<11.0.0,>=10.1.0
 Requires-Dist: inscriptis<3.0.0,>=2.3.2 Requires-Dist: aiohttp<4.0.0,>=3.8.6
 Requires-Dist: pytelegrambotapi<5.0.0,>=4.14.0 Requires-Dist: ffmpeg-
 python<1.0.0,>=0.2.0 Requires-Dist: duckduckgo-search<4.0.0,>=3.9.5 Requires-
-Dist: flask<4.0.0,>=3.0.0 Requires-Dist: hikari==2.0.0.dev121; extra == "bot"
-Requires-Dist: hikari-crescent<1.0.0,>=0.6.4; extra == "bot" Requires-Dist:
-khl-py<1.0.0,>=0.3.17; extra == "bot" Requires-Dist: slack-bolt<2.0.0,>=1.18.0;
-extra == "bot" Requires-Dist: hikari==2.0.0.dev121; extra == "testing"
-Requires-Dist: hikari-crescent<1.0.0,>=0.6.4; extra == "testing" Requires-Dist:
-khl-py<1.0.0,>=0.3.17; extra == "testing" Requires-Dist: slack-
-bolt<2.0.0,>=1.18.0; extra == "testing" Requires-Dist: pre-
-commit<3.5.0,>=2.15.0; extra == "testing" Provides-Extra: bot Provides-Extra:
-testing Description-Content-Type: text/markdown ![cover](https://
-raw.githubusercontent.com/LlmKira/.github/main/llmbot/project_cover.png) ------
-------------
+Dist: flask<4.0.0,>=3.0.0 Requires-Dist: telegramify-markdown>=0.1.2 Requires-
+Dist: json-repair>=0.13.0 Requires-Dist: curl-cffi>=0.6.2 Requires-Dist:
+deprecated>=1.2.14 Requires-Dist: aiofile>=3.8.8 Requires-Dist: file-read-
+backwards>=3.0.0 Requires-Dist: apscheduler>=3.10.4 Requires-Dist: montydb
+[lmdb]>=2.5.2 Requires-Dist: pymongo>=4.6.3 Requires-Dist:
+hikari==2.0.0.dev121; extra == "bot" Requires-Dist: hikari-
+crescent<1.0.0,>=0.6.4; extra == "bot" Requires-Dist: khl-py<1.0.0,>=0.3.17;
+extra == "bot" Requires-Dist: slack-bolt<2.0.0,>=1.18.0; extra == "bot"
+Requires-Dist: hikari==2.0.0.dev121; extra == "testing" Requires-Dist: hikari-
+crescent<1.0.0,>=0.6.4; extra == "testing" Requires-Dist: khl-
+py<1.0.0,>=0.3.17; extra == "testing" Requires-Dist: slack-bolt<2.0.0,>=1.18.0;
+extra == "testing" Requires-Dist: pre-commit<3.5.0,>=2.15.0; extra == "testing"
+Provides-Extra: bot Provides-Extra: testing Description-Content-Type: text/
+markdown ![cover](https://raw.githubusercontent.com/LlmKira/.github/main/
+llmbot/project_cover.png) ------------------
                            _[_d_o_c_k_e_r_]_[_d_o_c_k_e_r_ _w_o_r_k_f_l_o_w_]
                               _[_t_e_l_e_g_r_a_m_]_[_d_i_s_c_o_r_d_]
                             _[_l_i_c_e_n_s_e_]_[_d_o_c_k_e_r_ _b_u_i_l_d_]
-_ð___©_ _é__¨_ç_½_²_æ___æ_¡_£ & _ð__§__ _å_¼__å___æ___æ_¡_£ & _ð____ _E_n_g_l_i_s_h_ _R_e_a_d_m_e & _ð__¤__ _è_´_¡_ç__®_å_¿__ç__
-> **Look for English README? Click [here](README_EN.md). We also have English
-documentation [here](https://llmkira.github.io/Docs/en).** >
-é¨ç½²éå°é®é¢ï¼æäº¤ Issue å¸®å©æä»¬æåå¯ç¨æ§
-æ­¤é¡¹ç®ä¸ºèªé¨ç½²ï¼å®ç¨å¯æ©å±çæºå¨äººæ ¸å¿ï¼ä»¥ `FunctionCall`
-`ToolCall` ä¸ºæ ¸å¿ï¼æ¯æå¤ç§æ¶æ¯å¹³å°ã
-éç¨æ¶æ¯éåï¼å¾å¥½å¤çå½æ°è¯·æ±ï¼æ¯æç¹æçæä»¶ååè½è®¾è®¡ãè¯å¥½æ¯ææä»¶ç³»ç»ã
-æ¯æå¤ç§æ¨¡åæºï¼æ¯æè·¨å¹³å°æ¶æ¯è½¬åã | Demo | |--------------
----------------------| | ![sticker](./docs/chain_chat.gif) |
-ä¸ä¹åçé¡¹ç®ä¸åçæ¯ï¼æ­¤é¡¹ç®å°è¯åºäºæ¶æ¯å¹³å°å¤å»
-ChatGpt çæä»¶ç³»ç»ï¼å®ç°é¨åææ´è¿ä¸æ­¥çåè½ã > å ä¸º func
-call ä¸º feature,æä»¥åªæ¯æ Openai ç±»åç api, ä¸æç®æ¯ææ²¡æ
-func call ç LLM ## ð¦ Feature - ðª
-å®åçæä»¶å¼åçæï¼éç¨ç»å¸è®¾è®¡ï¼éè¿ `pip`
-å®è£å³å¯ä½¿ç¨ - ð
-æ¶æ¯ç³»ç»ï¼ä¸éæ¶é´ï¼ä¸éåéç«¯ï¼å®ä¹åéæ¥æ¶èï¼é»è¾å®å¨è§£è¦
-- ð è·¯ç±æ¶æ¯ï¼èªå®ä¹æ¶æ¯è·¯ç±ï¼ä»¥è·¯ç±å³å®è¿ä½æ¹å¼ -
-ð¬ å¬å±å¼æ¾éé¢/ç§äººèªéç½®åç«¯/
-ä»£çTokenè®¤è¯ï¼æä¾çµæ´»å¯æ©å±çé´æå¼åæ¹æ¡ - ð¾
-æ¯æä¸­é´ä»¶æ¦æªå¼åï¼å¼åæ©å±å³å¯æä½æµç¨ååæ°æ® - ðµ
-ç»åçç»è®¡ç³»ç»ï¼è½»æ¾ç»è®¡ä½¿ç¨æåµ - ð°
-æ¯ææä»¶äººå¨åè·¯éªè¯ï¼å¯é´æï¼å¯è®¾ç½®æä»¶é»åå - ð¦
-å®åæ åçæä»¶äº¤äºæ¯æï¼ä¸ä¼ /ä¸è½½æä»¶ - ð
-æ¯æä¸ªäººåç¬éç½®ç¯å¢å¯é¥ï¼ä¸ºæä»¶æä¾ä¸ªäººçç§æç¯å¢åé
-- ð
-æ¯æå¤§è¯­è¨æ¨¡åå¢éæ¯æï¼æ¯æå¤å¹³å°æ©å±ï¼ç»§æ¿æ åç±»å³å¯éé
-- ð åæ¶æ¯æ `FunctionCall` `ToolCall`
-ç¹æ§ï¼æ ¹æ®æ¨¡åå¨ææå»ºéè¦çå½æ°ç±» ### ð§ é¨åæä»¶é¢è§
-| Sticker Converter | Timer Func | Translate Func | |--------------------------
------------|---------------------------------|---------------------------------
--------------| | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/
-timer_func.gif) | ![translate](./docs/translate_file_func.gif) | ### ð§
-è®¤è¯ç³»ç»ä»ç» æä»¬éç¨çè®¤è¯ç³»ç»ç§°ä¸º `Service
-Provider`ï¼å³æå¡æä¾åï¼å®çä½ç¨æ¯ä¸ºæ¯ä¸ªåéèåé
-Endpoint/Key/Model ï¼ç¨äºé´æã æ¥æä¸ä¸ª `token` ä½ä¸ºç»å®ç
-OpenKeyãç¨åºä¼è°ç¨è®¾å®ç `Service Provider` è¯»åç§æ Key/éç½®
-Token æ¥è·åé´æä¿¡æ¯ã ![auth](./docs/SeriveProvider.svg)
-è®¤è¯ç»ä»¶ååç«¯åéè¦èªè¡å®ç°ã ### ð¬ å¹³å°æ¯æ | å¹³å° |
-æ¯ææåµ | æä»¶ç³»ç» | å¤æ³¨ | |----------|------|------|-------------
-| | Telegram | â | â | | | Discord | â | â | | | Kook | â | â |
-ä¸æ¯æ `è¢«åå¤å¯å¨` | | Slack | â | â | ä¸æ¯æ `è¢«åå¤å¯å¨`
-| | QQ | â | | | | Wechat | â | | | | Twitter | â | | | | Matrix | â |
-| | | IRC | â | | | | ... | | | åå»ºIssue/PR | ## ð¦ å¿«éå¼å§ éè¯»
-[ð§ é¨ç½²ææ¡£](https://llmkira.github.io/Docs/) è·å¾æ´å¤ä¿¡æ¯ã
-è¯·æåç¨ `pdm run python3 start_sender.py` `pdm run python3
-start_receiver.py` æµè¯æ¯å¦è½æ­£å¸¸è¿è¡ã #### æ§è½ææ æµè¯(Until
-2023/11/1)
-æ³¨æï¼ä¸åæ¬pm2ï¼redisï¼rabbitmqï¼mongodbï¼dockerç­æå¡çåå­å ç¨ã
-| è¿ç¨ | åå­åå¼ | æµç®å½ä»¤ | client | |------------|-----------|---
------------------------------------------------|----------| | `receiver` |
-120.202MB | `python3 -m memray run --live start_receiver.py` | telegram | |
-`sender` | 83.375MB | `python3 -m memray run --live start_sender.py` | telegram
-| ### ð¥£ Docker Build Hub: [sudoskys/llmbot](https://hub.docker.com/
-repository/docker/sudoskys/llmbot/general) #### èªå¨ Docker/Docker-
-composeå®è£
-å¦æä½ å¨ä½¿ç¨ä¸å°å´­æ°çæå¡å¨ï¼ä½ å¯ä»¥ä½¿ç¨ä¸é¢çShellæ¥å°è¯èªå¨å®è£æ¬é¡¹ç®ã
-æ­¤èæ¬ä¼èªå¨ä½¿ç¨ Docker
-æ¹æ³å®è£æéæå¡å¹¶æ å°ç«¯å£ï¼å¦ææ¨å·²ç»é¨ç½²äº `redis`
-ï¼`rabbitmq` ï¼`mongodb` ã è¯·èªè¡ä¿®æ¹ `docker-compose.yml` æä»¶ã
-```shell curl -sSL https://raw.githubusercontent.com/LLMKira/Openaibot/main/
-deploy.sh | bash ``` #### æå¨ Docker-composeå®è£ ```shell git clone https:
-//github.com/LlmKira/Openaibot.git cd Openaibot cp .env.exp .env&&nano .env
-docker-compose -f docker-compose.yml up -d ``` æ´æ°éåä½¿ç¨ `docker-
-compose pull`ã å¨ docker ä¸­æ¥ç Shellï¼ä½¿ç¨ `docker exec -it llmbot /
-bin/bash`ï¼è¾å¥ `exit` éåºã ### ð Shell
-äººå·¥ä½¿ç¨Pm2å¯å¨ï¼éè¦èªè¡å®è£ `redis` ï¼`rabbitmq` ï¼`mongodb`
-ã ```shell git clone https://github.com/LlmKira/Openaibot.git pip install pdm
-cd Openaibot pdm install -G bot cp .env.exp .env && nano .env apt install npm -
-y && npm install pm2 && pm2 start pm2.json pm2 monit ``` éå¯ç¨åºä½¿ç¨
-`pm2 restart pm2.json` ã > æ¨èä½¿ç¨ `pdm`
-è¿è¡ä¾èµç®¡çï¼å ä¸ºæä»¬ä½¿ç¨äº
-`pydantic^1.9.0`ï¼ä¸ºäºé²æ­¢åºç°çæ¬å²çªï¼æä»¬ä½¿ç¨äº `pdm`
-è¿è¡ä¾èµç®¡çã ## ðª Slash Command ```shell clear - å é¤èå¤©è®°å½
-help - æ¾ç¤ºææ¡£ chat - å¯¹è¯ task - å¯ç¨å½æ°ä»¥å¯¹è¯ ask -
-ç¦æ­¢å½æ°ä»¥å¯¹è¯ tool - ååºææå½æ° set_endpoint - è®¾ç½®ç§æ key
-å endpoint clear_endpoint - æ¸é¤ç§æ key å endpoint auth -
-ææä¸ä¸ªå½æ° env - å½æ°ç¯å¢åé token - ç»å®ä»¤ç token_clear -
-æ¸é¤ä»¤çç»å® func_ban - ç¦ç¨ä¸ä¸ªå½æ° func_unban -
-è§£ç¦ä¸ä¸ªå½æ° bind - ç»å®æ¶æ¯æº unbind - è§£ç»æ¶æ¯æº ``` ## ð»
-å¦ä½å¼åæä»¶ï¼ æä»¶å¼åææ¡£è¯·åè `plugins`
-ç®å½ä¸çç¤ºä¾æä»¶å [ð§ æä»¶å¼åææ¡£](https://
-llmkira.github.io/Docs/dev/basic) ## ð¤ We need your help! This is a long
-term project and we started the development of the LLM APP very early! We
-applied a plugin-like system and search online before GPT3 OpenaiApi was
-released(davinci-003) After many iterations, we have worked hard to make this
-project more standardized, generic, and open. We can't do it on our own at the
-moment: - [ ] We need help with the documentation - [ ] Web UI Feel free to
-submit a Pull Request or discuss, we'd love to receive your contribution! ##
-ð åç¥ > æ­¤é¡¹ç®ä¸ Openai å®æ¹æ å³ï¼å¨ç§°ä¸º
-OpenAiBotï¼è¡¨ç¤ºå¼æ¾äººå·¥æºè½æºå¨äººï¼å¹¶ä¸è¡¨ç¤ºä¸º Openai
-æå±æºå¨äººã > å¦ææ¨æå¨è¾åºç¦æ­¢ä½¿ç¨ Openai
-æå¡ï¼è¯·å¿ä½¿ç¨æ­¤é¡¹ç®ã [![FOSSA Status](https://app.fossa.com/api/
-projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot.svg?type=small)](https://
+              _ð___©_ _D_e_p_l_o_y_ _D_o_c_s & _ð__§__ _D_e_v_ _D_o_c_s & _ð__¤__ _C_o_n_t_r_i_b_u_t_e
+> Don't hesitate to Star â­ï¸, Issue ð, and PR ð ï¸ > Python>=3.9 This
+project uses the ToolCall feature. It integrates a message queuing and snapshot
+system, offering plugin mechanisms and authentication prior to plugin
+execution. The model adheres to the Openai Schema, other models are not
+supported. Please adapt using gateways independently. | Demo | |---------------
+--------------------| | ![sticker](./docs/chain_chat.gif) | ## ð Roadmap -
+[x] Removal of legacy code - [x] Deletion of metric system - [x] Deletion of
+model selection system, unified to OpenAI Schema - [x] Implementation of a more
+robust plugin system - [x] Project structure simplification - [x] Elimination
+of the Provider system ## ð¦ Features - ðª A comprehensive plugin
+development ecosystem, adopting a classic design, and seamless integration with
+plugins through `pip` installation - ð Message system with no time or sender
+constraints, offering fully decoupled logics - ð¬ Offers Login via a URL
+mechanism, providing a flexible and expandable authentication development
+solution - ð° Empowers users to authorize plugin execution. Users can
+configure plugin environment variables at their discretion - ð¦ Support for
+plugins to access files - ð Multi-platform support â extend new platforms
+by inheriting the base class - ð Plugins can determine their appearance in
+new sessions dynamically, preventing performance degradation despite large
+amounts of plugins ### ð Login Modes - `Login via url`: Use `/login
+token#https://provider.com` to Login. The program posts the token to the
+interface to retrieve configuration information - `Login`: Use `/login https://
+api.com/v1#key#model` to login ### ð§ Plugin Previews | Sticker Converter |
+Timer Function | Translate Function | |-------------------------------------|--
+-------------------------------|----------------------------------------------
+| | ![sticker](./docs/sticker_func.gif) | ![timer](./docs/timer_func.gif) | !
+[translate](./docs/translate_file_func.gif) | ### ð¬ Platform Support |
+Platform | Support | File System | Remarks | |----------|---------|------------
+-|----------------------------------------| | Telegram | â | â | | |
+Discord | â | â | | | Kook | â | â | Does not support `triggering by
+reply` | | Slack | â | â | Does not support `triggering by reply` | | QQ |
+â | | | | Wechat | â | | | | Twitter | â | | | | Matrix | â | | | | IRC
+| â | | | | ... | | | Create Issue/PR | ## ð¦ Quick Start Refer to the
+[ð§ Deployment Document](https://llmkira.github.io/Docs/) for more
+information. ```shell # Install RabbitMQ docker pull rabbitmq:3.10-management
+docker run -d -p 5672:5672 -p 15672:15672 \ -e RABBITMQ_DEFAULT_USER=admin \ -
+e RABBITMQ_DEFAULT_PASS=8a8a8a \ --hostname myRabbit \ --name rabbitmq \
+rabbitmq:3.10-management docker ps -l # Install Project pip install pdm pdm
+install -G bot cp .env.exp .env && nano .env # Test pdm run python3
+start_sender.py pdm run python3 start_receiver.py # Host pdm start pm2.json ```
+### ð¥£ Docker Build Hub: [sudoskys/llmbot](https://hub.docker.com/repository/
+docker/sudoskys/llmbot/general) #### Automatic Docker/Docker-compose
+Installation If you are using a brand new server, you can use the following
+shell to automatically install this project. This script automatically installs
+the required services and maps ports using Docker methods. If you have deployed
+`redis`, `rabbitmq`, `mongodb`, please modify the `docker-compose.yml` file
+accordingly. ```shell curl -sSL https://raw.githubusercontent.com/LLMKira/
+Openaibot/main/deploy.sh | bash ``` #### Manual Docker-compose Installation
+```shell git clone https://github.com/LlmKira/Openaibot.git cd Openaibot cp
+.env.exp .env&&nano .env docker-compose -f docker-compose.yml up -d ``` Update
+image using `docker-compose pull`. Use `docker exec -it llmbot /bin/bash` to
+view Shell in Docker, enter `exit` to exit. ## ðª Slash Commands ```shell
+clear - Deletes chat records help - Displays documentation chat - Conversation
+task - Use a function to converse ask - Disable function-based conversations
+tool - Lists all functions login - Login auth - Authorize a function env -
+Environment variables of the function ``` ## ð» How to Develop Plugins? Refer
+to the example plugins in the `plugins` directory and the [ð§ Plugin
+Development Document](https://llmkira.github.io/Docs/dev/basic) for plugin
+development documentation. ## ð§ Sponsor [![sponsor](./.github/
+sponsor_ohmygpt.png)](https://www.ohmygpt.com) ## ð Notice > This project,
+named OpenAiBot, signifying "Open Artificial Intelligence Robot", is not
+officially affiliated with > OpenAI. [![FOSSA Status](https://app.fossa.com/
+api/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot.svg?type=small)](https://
 app.fossa.com/projects/git%2Bgithub.com%2Fsudoskys%2FOpenaibot?ref=badge_small)
```

