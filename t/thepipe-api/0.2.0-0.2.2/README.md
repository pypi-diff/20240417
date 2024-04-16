# Comparing `tmp/thepipe_api-0.2.0.tar.gz` & `tmp/thepipe_api-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepipe_api-0.2.0.tar", last modified: Tue Apr 16 00:12:54 2024, max compression
+gzip compressed data, was "thepipe_api-0.2.2.tar", last modified: Tue Apr 16 18:08:40 2024, max compression
```

## Comparing `thepipe_api-0.2.0.tar` & `thepipe_api-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 00:12:54.856780 thepipe_api-0.2.0/
--rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     9672 2024-04-16 00:12:54.854779 thepipe_api-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     8944 2024-04-16 00:09:20.000000 thepipe_api-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-16 00:12:54.856780 thepipe_api-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-04-16 00:10:02.000000 thepipe_api-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 00:12:54.826780 thepipe_api-0.2.0/tests/
--rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0     9523 2024-04-13 23:06:00.000000 thepipe_api-0.2.0/tests/test_thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-16 00:12:54.831779 thepipe_api-0.2.0/thepipe_api/
--rw-rw-rw-   0        0        0       86 2024-04-15 22:46:19.000000 thepipe_api-0.2.0/thepipe_api/__init__.py
--rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.2.0/thepipe_api/compressor.py
--rw-rw-rw-   0        0        0     2789 2024-04-15 23:00:33.000000 thepipe_api-0.2.0/thepipe_api/core.py
--rw-rw-rw-   0        0        0    19781 2024-04-16 00:09:41.000000 thepipe_api-0.2.0/thepipe_api/extractor.py
--rw-rw-rw-   0        0        0     3628 2024-04-16 00:06:35.000000 thepipe_api-0.2.0/thepipe_api/thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-16 00:12:54.853779 thepipe_api-0.2.0/thepipe_api.egg-info/
--rw-rw-rw-   0        0        0     9672 2024-04-16 00:12:54.000000 thepipe_api-0.2.0/thepipe_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-04-16 00:12:54.000000 thepipe_api-0.2.0/thepipe_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 00:12:54.000000 thepipe_api-0.2.0/thepipe_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-16 00:12:54.000000 thepipe_api-0.2.0/thepipe_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      105 2024-04-16 00:12:54.000000 thepipe_api-0.2.0/thepipe_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-16 00:12:54.000000 thepipe_api-0.2.0/thepipe_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 18:08:40.765298 thepipe_api-0.2.2/
+-rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     9795 2024-04-16 18:08:40.764298 thepipe_api-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9068 2024-04-16 05:29:43.000000 thepipe_api-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 18:08:40.766298 thepipe_api-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-04-16 18:08:14.000000 thepipe_api-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:08:40.733785 thepipe_api-0.2.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.2.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     9265 2024-04-16 16:00:52.000000 thepipe_api-0.2.2/tests/test_thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:08:40.737785 thepipe_api-0.2.2/thepipe_api/
+-rw-rw-rw-   0        0        0       86 2024-04-15 22:46:19.000000 thepipe_api-0.2.2/thepipe_api/__init__.py
+-rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.2.2/thepipe_api/compressor.py
+-rw-rw-rw-   0        0        0     2778 2024-04-16 05:18:22.000000 thepipe_api-0.2.2/thepipe_api/core.py
+-rw-rw-rw-   0        0        0    19869 2024-04-16 18:07:02.000000 thepipe_api-0.2.2/thepipe_api/extractor.py
+-rw-rw-rw-   0        0        0     3649 2024-04-16 05:20:42.000000 thepipe_api-0.2.2/thepipe_api/thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:08:40.764298 thepipe_api-0.2.2/thepipe_api.egg-info/
+-rw-rw-rw-   0        0        0     9795 2024-04-16 18:08:40.000000 thepipe_api-0.2.2/thepipe_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-16 18:08:40.000000 thepipe_api-0.2.2/thepipe_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 18:08:40.000000 thepipe_api-0.2.2/thepipe_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-16 18:08:40.000000 thepipe_api-0.2.2/thepipe_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      104 2024-04-16 18:08:40.000000 thepipe_api-0.2.2/thepipe_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-16 18:08:40.000000 thepipe_api-0.2.2/thepipe_api.egg-info/top_level.txt
```

### Comparing `thepipe_api-0.2.0/LICENSE` & `thepipe_api-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.0/PKG-INFO` & `thepipe_api-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.2.0
+Version: 0.2.2
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 Requires-Dist: Pyarrow
 Requires-Dist: python-magic
 Requires-Dist: colorama
 Requires-Dist: requests
 Requires-Dist: pillow
 Requires-Dist: cssutils
 Requires-Dist: beautifulsoup4
-Requires-Dist: PyMuPDF
+Requires-Dist: magika
 
 
 # <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
 <p>
   <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
 </p>
 
@@ -32,22 +32,32 @@
 
 ### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
 
 The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally.
 
 ![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
 
+## Features 🌟
+
+- Extracts text and visuals from files or web pages 📚
+- Outputs chunks optimized for multimodal LLMs 🖼️
+- Interpret complex PDFs, web pages, slides, CSVs, and more 🧠
+- Auto-compress prompts exceeding your chosen token limit 📦
+- Works even with missing file extensions, in-memory data streams 💾
+- Works with codebases, git repos, and custom integrations 🌐
+- Multi-threaded ⚡️
+
 ## Getting Started  🚀
 
 First, install The Pipe. 
 ```
 pip install thepipe_api
 ```
 
-Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key yet? [Get one here](https://thepi.pe). Looking to operate it yourself locally instead? See the local installation section.
+Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key yet? [Get one here](https://thepi.pe). Alternatively, see the local installation section for the more advanced local setup.
 
 Now you can extract comprehensive text and visuals from any file:
 ```python
 from thepipe_api import thepipe
 chunks = thepipe.extract("example.pdf")
 ```
 Or any website:
@@ -64,37 +74,27 @@
 The Pipe's output is a list of sensible "chunks", and thus can be used either for storage in a vector database or for direct use as a prompt. Extra features such as data table extraction, bar chart extraction, custom web authentications and more are available in the [API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider.
 
 You can also use The Pipe from the command line. Here's how to recursively extract from a directory:
 ```
 thepipe path/to/folder
 ```
 
-## Features 🌟
-
-- Extracts text and visuals from any file or web page 📚
-- Outputs RAG-ready chunks, optimized for multimodal LLMs 🖼️ + 💬
-- Can interpret complex PDFs, web apps, markdown, etc 🧠
-- Auto-compress prompts exceeding your chosen token limit 📦
-- Works with missing file extensions, in-memory data streams 💾
-- Works with codebases, URL, git repos, and more 🌐
-- Multi-threaded ⚡️
-
 ##  How it works 🛠️
 
-The pipe is accessible from the command line or from [Python](https://www.python.org/downloads/). The input source is either a file path, a URL, or a directory (or zip file) path. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based (or multimodal) representation of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
+The pipe is accessible from the command line or from [Python](https://www.python.org/downloads/). The input source is either a file path, a URL, or a directory. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based (or multimodal) representation of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
 
 ## Supported File Types 📚
 
 | Source Type                           | Input types        | Token Compression 🗜️ | Image Extraction 👁️ | Notes 📌                                                  |
 |---------------------------------------|------------------------------------------|-------------------|------------------|---------------------------------------------------------|
 | Directory                             | Any `/path/to/directory`                 | ✔️               | ✔️               | Extracts from all files in directory, supports match and ignore patterns |
 | Code                                  | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | ✔️ (varies)   | ❌               | Combines all code files. `.c`, `.cpp`, `.py` are compressible with ctags, others are not |
 | Plaintext                             | `.txt`, `.md`, `.rtf`, etc               | ✔️               | ❌               | Regular text files                                                      |
 | PDF                                   | `.pdf`                                  | ✔️               | ✔️    | Extracts text and images of each page; can use AI for extraction of table data and  images within pages |
-| Image                                 | `.jpg`, `.jpeg`, `.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
+| Image                                 | `.jpg`, `.jpeg`, `.png` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
 | Data Table                           | `.csv`, `.xls`, `.xlsx`             | ✔️                | ❌               | Extracts data from spreadsheets; converts to text representation. For very large datasets, will only extract column names and types         |
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
 | Website                               | URLs (inputs containing `http`, `https`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
@@ -104,22 +104,27 @@
 To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements. You will also need to use the local version of the requirements file:
 
 ```bash
 git clone https://github.com/emcf/thepipe
 pip install -r requirements_local.txt
 ```
 
-Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`.
+Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`. You may also need to ensure the tesseract-ocr binaries and the ctags binaries are in your PATH.
 
-Now you can use The Pipe:
+Now you can use The Pipe with Python:
 ```bash
 from thepipe_api import thepipe
 chunks = thepipe.extract("example.pdf", local=True)
 ```
 
+or from the command line:
+```bash
+thepipe path/to/folder --local
+```
+
 Arguments are:
 - `source` (required): can be a file path, a URL, or a directory path.
 - `local` (optional): Use the local version of The Pipe instead of the hosted API.
 - `match` (optional): Regex pattern to match files in the directory.
 - `ignore` (optional): Regex pattern to ignore files in the directory.
 - `limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed.
 - `ai_extraction` (optional): Extract tables, figures, and math from PDFs using our extractor. Incurs extra costs.
```

#### html2text {}

```diff
@@ -1,107 +1,108 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.0 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.2 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
 pillow Requires-Dist: cssutils Requires-Dist: beautifulsoup4 Requires-Dist:
-PyMuPDF # _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
+magika # _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
 _E_n_g_l_i_s_h | _ä_¸_­_æ__
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/
 badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-
 action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/
 badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
 _A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
 docs, slides, web pages and more into Vision-LLMs with one line of code â¡ The
 Pipe is a multimodal-first tool for feeding files and web pages into vision-
 language models such as GPT-4V. It is best for LLM and RAG applications that
 require a deep understanding of tricky data sources. The Pipe is available as a
 hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. !
 [Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/
-assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Getting Started ð First,
-install The Pipe. ``` pip install thepipe_api ``` Ensure the `THEPIPE_API_KEY`
-environment variable is set. Don't have an API key yet? [Get one here](https://
-thepi.pe). Looking to operate it yourself locally instead? See the local
-installation section. Now you can extract comprehensive text and visuals from
-any file: ```python from thepipe_api import thepipe chunks = thepipe.extract
-("example.pdf") ``` Or any website: ```python chunks = thepipe.extract("https:/
-/example.com") ``` Then feed it into GPT-4-Vision: ```python response =
-client.chat.completions.create( model="gpt-4-vision-preview", messages =
-chunks, ) ``` The Pipe's output is a list of sensible "chunks", and thus can be
-used either for storage in a vector database or for direct use as a prompt.
-Extra features such as data table extraction, bar chart extraction, custom web
-authentications and more are available in the [API documentation](https://
-thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to
-easily integrate The Pipe with any LLM provider. You can also use The Pipe from
-the command line. Here's how to recursively extract from a directory: ```
-thepipe path/to/folder ``` ## Features ð - Extracts text and visuals from
-any file or web page ð - Outputs RAG-ready chunks, optimized for multimodal
-LLMs ð¼ï¸ + ð¬ - Can interpret complex PDFs, web apps, markdown, etc ð§ 
-- Auto-compress prompts exceeding your chosen token limit ð¦ - Works with
-missing file extensions, in-memory data streams ð¾ - Works with codebases,
-URL, git repos, and more ð - Multi-threaded â¡ï¸ ## How it works ð ï¸
-The pipe is accessible from the command line or from [Python](https://
-www.python.org/downloads/). The input source is either a file path, a URL, or a
-directory (or zip file) path. The pipe will extract information from the source
-and process it for downstream use with [language models](https://
-en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://
-en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://
-arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based
-(or multimodal) representation of the extracted information, carefully crafted
-to fit within context windows for any models from [gemma-7b](https://
-huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a
-variety of heuristics for optimal performance with vision-language models,
-including AI filetype detection with [filetype detection](https://
-opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-
-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token
-compression](https://arxiv.org/abs/2403.12968), automatic [image encoding]
-(https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/
-2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects,
-and more, all pre-built to work out-of-the-box. ## Supported File Types ð |
-Source Type | Input types | Token Compression ðï¸ | Image Extraction
-ðï¸ | Notes ð | |---------------------------------------|---------------
----------------------------|-------------------|------------------|------------
----------------------------------------------| | Directory | Any `/path/to/
-directory` | âï¸ | âï¸ | Extracts from all files in directory, supports
-match and ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`,
-`.cpp`, etc | âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`,
-`.py` are compressible with ctags, others are not | | Plaintext | `.txt`,
-`.md`, `.rtf`, etc | âï¸ | â | Regular text files | | PDF | `.pdf` |
-âï¸ | âï¸ | Extracts text and images of each page; can use AI for
-extraction of table data and images within pages | | Image | `.jpg`, `.jpeg`,
-`.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | â | âï¸ | Extracts
-images, uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx` | âï¸
-| â | Extracts data from spreadsheets; converts to text representation. For
-very large datasets, will only extract column names and types | | Jupyter
-Notebook | `.ipynb` | â | âï¸ | Extracts code, markdown, and images from
-Jupyter notebooks | | Microsoft Word Document | `.docx` | âï¸ | âï¸ |
-Extracts text and images from Word documents | | Microsoft PowerPoint
-Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images from
-PowerPoint presentations | | Website | URLs (inputs containing `http`, `https`,
-`ftp`) | âï¸ | âï¸ | Extracts text from web page along with image (or
-images if scrollable); text-only extraction available | | GitHub Repository |
-GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub repositories;
-supports branch specification | | ZIP File | `.zip` | âï¸ | âï¸ |
-Extracts contents of ZIP files; supports nested directory extraction | ## Local
-Installation ð ï¸ To use The Pipe locally, you will need [playwright](https:
-//github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/
-), [pytesseract](https://github.com/h/pytesseract), and the local python
+assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Features ð - Extracts
+text and visuals from files or web pages ð - Outputs chunks optimized for
+multimodal LLMs ð¼ï¸ - Interpret complex PDFs, web pages, slides, CSVs, and
+more ð§  - Auto-compress prompts exceeding your chosen token limit ð¦ -
+Works even with missing file extensions, in-memory data streams ð¾ - Works
+with codebases, git repos, and custom integrations ð - Multi-threaded â¡ï¸
+## Getting Started ð First, install The Pipe. ``` pip install thepipe_api
+``` Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API
+key yet? [Get one here](https://thepi.pe). Alternatively, see the local
+installation section for the more advanced local setup. Now you can extract
+comprehensive text and visuals from any file: ```python from thepipe_api import
+thepipe chunks = thepipe.extract("example.pdf") ``` Or any website: ```python
+chunks = thepipe.extract("https://example.com") ``` Then feed it into GPT-4-
+Vision: ```python response = client.chat.completions.create( model="gpt-4-
+vision-preview", messages = chunks, ) ``` The Pipe's output is a list of
+sensible "chunks", and thus can be used either for storage in a vector database
+or for direct use as a prompt. Extra features such as data table extraction,
+bar chart extraction, custom web authentications and more are available in the
+[API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/
+BerriAI/litellm) can be used to easily integrate The Pipe with any LLM
+provider. You can also use The Pipe from the command line. Here's how to
+recursively extract from a directory: ``` thepipe path/to/folder ``` ## How it
+works ð ï¸ The pipe is accessible from the command line or from [Python]
+(https://www.python.org/downloads/). The input source is either a file path, a
+URL, or a directory. The pipe will extract information from the source and
+process it for downstream use with [language models](https://en.wikipedia.org/
+wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/
+wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/
+2304.00685). The output from the pipe is a sensible text-based (or multimodal)
+representation of the extracted information, carefully crafted to fit within
+context windows for any models from [gemma-7b](https://huggingface.co/google/
+gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a variety of heuristics
+for optimal performance with vision-language models, including AI filetype
+detection with [filetype detection](https://opensource.googleblog.com/2024/02/
+magika-ai-powered-fast-and-efficient-file-type-identification.html), AI [PDF
+extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/
+abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/
+Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle]
+(https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work
+out-of-the-box. ## Supported File Types ð | Source Type | Input types |
+Token Compression ðï¸ | Image Extraction ðï¸ | Notes ð | |----------
+-----------------------------|------------------------------------------|------
+-------------|------------------|----------------------------------------------
+-----------| | Directory | Any `/path/to/directory` | âï¸ | âï¸ |
+Extracts from all files in directory, supports match and ignore patterns | |
+Code | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | âï¸ (varies) |
+â | Combines all code files. `.c`, `.cpp`, `.py` are compressible with ctags,
+others are not | | Plaintext | `.txt`, `.md`, `.rtf`, etc | âï¸ | â |
+Regular text files | | PDF | `.pdf` | âï¸ | âï¸ | Extracts text and
+images of each page; can use AI for extraction of table data and images within
+pages | | Image | `.jpg`, `.jpeg`, `.png` | â | âï¸ | Extracts images,
+uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx` | âï¸ | â |
+Extracts data from spreadsheets; converts to text representation. For very
+large datasets, will only extract column names and types | | Jupyter Notebook |
+`.ipynb` | â | âï¸ | Extracts code, markdown, and images from Jupyter
+notebooks | | Microsoft Word Document | `.docx` | âï¸ | âï¸ | Extracts
+text and images from Word documents | | Microsoft PowerPoint Presentation |
+`.pptx` | âï¸ | âï¸ | Extracts text and images from PowerPoint
+presentations | | Website | URLs (inputs containing `http`, `https`, `ftp`) |
+âï¸ | âï¸ | Extracts text from web page along with image (or images if
+scrollable); text-only extraction available | | GitHub Repository | GitHub repo
+URLs | âï¸ | âï¸ | Extracts from GitHub repositories; supports branch
+specification | | ZIP File | `.zip` | âï¸ | âï¸ | Extracts contents of
+ZIP files; supports nested directory extraction | ## Local Installation ð ï¸
+To use The Pipe locally, you will need [playwright](https://github.com/
+microsoft/playwright), [ctags](https://github.com/universal-ctags/),
+[pytesseract](https://github.com/h/pytesseract), and the local python
 requirements, which differ from the more lightweight API requirements. You will
 also need to use the local version of the requirements file: ```bash git clone
 https://github.com/emcf/thepipe pip install -r requirements_local.txt ``` Tip
 for windows users: you may need to install the python-libmagic binaries with
-`pip install python-magic-bin`. Now you can use The Pipe: ```bash from
-thepipe_api import thepipe chunks = thepipe.extract("example.pdf", local=True)
-``` Arguments are: - `source` (required): can be a file path, a URL, or a
-directory path. - `local` (optional): Use the local version of The Pipe instead
-of the hosted API. - `match` (optional): Regex pattern to match files in the
-directory. - `ignore` (optional): Regex pattern to ignore files in the
-directory. - `limit` (optional): The token limit for the output prompt,
+`pip install python-magic-bin`. You may also need to ensure the tesseract-ocr
+binaries and the ctags binaries are in your PATH. Now you can use The Pipe with
+Python: ```bash from thepipe_api import thepipe chunks = thepipe.extract
+("example.pdf", local=True) ``` or from the command line: ```bash thepipe path/
+to/folder --local ``` Arguments are: - `source` (required): can be a file path,
+a URL, or a directory path. - `local` (optional): Use the local version of The
+Pipe instead of the hosted API. - `match` (optional): Regex pattern to match
+files in the directory. - `ignore` (optional): Regex pattern to ignore files in
+the directory. - `limit` (optional): The token limit for the output prompt,
 defaults to 100K. Prompts exceeding the limit will be compressed. -
 `ai_extraction` (optional): Extract tables, figures, and math from PDFs using
 our extractor. Incurs extra costs. - `text_only` (optional): Do not extract
 images from documents or websites. Additionally, image files will be
 represented with OCR instead of as images.
```

### Comparing `thepipe_api-0.2.0/README.md` & `thepipe_api-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,32 @@
 
 ### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
 
 The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally.
 
 ![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
 
+## Features 🌟
+
+- Extracts text and visuals from files or web pages 📚
+- Outputs chunks optimized for multimodal LLMs 🖼️
+- Interpret complex PDFs, web pages, slides, CSVs, and more 🧠
+- Auto-compress prompts exceeding your chosen token limit 📦
+- Works even with missing file extensions, in-memory data streams 💾
+- Works with codebases, git repos, and custom integrations 🌐
+- Multi-threaded ⚡️
+
 ## Getting Started  🚀
 
 First, install The Pipe. 
 ```
 pip install thepipe_api
 ```
 
-Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key yet? [Get one here](https://thepi.pe). Looking to operate it yourself locally instead? See the local installation section.
+Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key yet? [Get one here](https://thepi.pe). Alternatively, see the local installation section for the more advanced local setup.
 
 Now you can extract comprehensive text and visuals from any file:
 ```python
 from thepipe_api import thepipe
 chunks = thepipe.extract("example.pdf")
 ```
 Or any website:
@@ -40,37 +50,27 @@
 The Pipe's output is a list of sensible "chunks", and thus can be used either for storage in a vector database or for direct use as a prompt. Extra features such as data table extraction, bar chart extraction, custom web authentications and more are available in the [API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider.
 
 You can also use The Pipe from the command line. Here's how to recursively extract from a directory:
 ```
 thepipe path/to/folder
 ```
 
-## Features 🌟
-
-- Extracts text and visuals from any file or web page 📚
-- Outputs RAG-ready chunks, optimized for multimodal LLMs 🖼️ + 💬
-- Can interpret complex PDFs, web apps, markdown, etc 🧠
-- Auto-compress prompts exceeding your chosen token limit 📦
-- Works with missing file extensions, in-memory data streams 💾
-- Works with codebases, URL, git repos, and more 🌐
-- Multi-threaded ⚡️
-
 ##  How it works 🛠️
 
-The pipe is accessible from the command line or from [Python](https://www.python.org/downloads/). The input source is either a file path, a URL, or a directory (or zip file) path. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based (or multimodal) representation of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
+The pipe is accessible from the command line or from [Python](https://www.python.org/downloads/). The input source is either a file path, a URL, or a directory. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based (or multimodal) representation of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
 
 ## Supported File Types 📚
 
 | Source Type                           | Input types        | Token Compression 🗜️ | Image Extraction 👁️ | Notes 📌                                                  |
 |---------------------------------------|------------------------------------------|-------------------|------------------|---------------------------------------------------------|
 | Directory                             | Any `/path/to/directory`                 | ✔️               | ✔️               | Extracts from all files in directory, supports match and ignore patterns |
 | Code                                  | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | ✔️ (varies)   | ❌               | Combines all code files. `.c`, `.cpp`, `.py` are compressible with ctags, others are not |
 | Plaintext                             | `.txt`, `.md`, `.rtf`, etc               | ✔️               | ❌               | Regular text files                                                      |
 | PDF                                   | `.pdf`                                  | ✔️               | ✔️    | Extracts text and images of each page; can use AI for extraction of table data and  images within pages |
-| Image                                 | `.jpg`, `.jpeg`, `.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
+| Image                                 | `.jpg`, `.jpeg`, `.png` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
 | Data Table                           | `.csv`, `.xls`, `.xlsx`             | ✔️                | ❌               | Extracts data from spreadsheets; converts to text representation. For very large datasets, will only extract column names and types         |
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
 | Website                               | URLs (inputs containing `http`, `https`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
@@ -80,22 +80,27 @@
 To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements. You will also need to use the local version of the requirements file:
 
 ```bash
 git clone https://github.com/emcf/thepipe
 pip install -r requirements_local.txt
 ```
 
-Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`.
+Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`. You may also need to ensure the tesseract-ocr binaries and the ctags binaries are in your PATH.
 
-Now you can use The Pipe:
+Now you can use The Pipe with Python:
 ```bash
 from thepipe_api import thepipe
 chunks = thepipe.extract("example.pdf", local=True)
 ```
 
+or from the command line:
+```bash
+thepipe path/to/folder --local
+```
+
 Arguments are:
 - `source` (required): can be a file path, a URL, or a directory path.
 - `local` (optional): Use the local version of The Pipe instead of the hosted API.
 - `match` (optional): Regex pattern to match files in the directory.
 - `ignore` (optional): Regex pattern to ignore files in the directory.
 - `limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed.
 - `ai_extraction` (optional): Extract tables, figures, and math from PDFs using our extractor. Incurs extra costs.
```

#### html2text {}

```diff
@@ -8,91 +8,92 @@
 _A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
 docs, slides, web pages and more into Vision-LLMs with one line of code â¡ The
 Pipe is a multimodal-first tool for feeding files and web pages into vision-
 language models such as GPT-4V. It is best for LLM and RAG applications that
 require a deep understanding of tricky data sources. The Pipe is available as a
 hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. !
 [Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/
-assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Getting Started ð First,
-install The Pipe. ``` pip install thepipe_api ``` Ensure the `THEPIPE_API_KEY`
-environment variable is set. Don't have an API key yet? [Get one here](https://
-thepi.pe). Looking to operate it yourself locally instead? See the local
-installation section. Now you can extract comprehensive text and visuals from
-any file: ```python from thepipe_api import thepipe chunks = thepipe.extract
-("example.pdf") ``` Or any website: ```python chunks = thepipe.extract("https:/
-/example.com") ``` Then feed it into GPT-4-Vision: ```python response =
-client.chat.completions.create( model="gpt-4-vision-preview", messages =
-chunks, ) ``` The Pipe's output is a list of sensible "chunks", and thus can be
-used either for storage in a vector database or for direct use as a prompt.
-Extra features such as data table extraction, bar chart extraction, custom web
-authentications and more are available in the [API documentation](https://
-thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to
-easily integrate The Pipe with any LLM provider. You can also use The Pipe from
-the command line. Here's how to recursively extract from a directory: ```
-thepipe path/to/folder ``` ## Features ð - Extracts text and visuals from
-any file or web page ð - Outputs RAG-ready chunks, optimized for multimodal
-LLMs ð¼ï¸ + ð¬ - Can interpret complex PDFs, web apps, markdown, etc ð§ 
-- Auto-compress prompts exceeding your chosen token limit ð¦ - Works with
-missing file extensions, in-memory data streams ð¾ - Works with codebases,
-URL, git repos, and more ð - Multi-threaded â¡ï¸ ## How it works ð ï¸
-The pipe is accessible from the command line or from [Python](https://
-www.python.org/downloads/). The input source is either a file path, a URL, or a
-directory (or zip file) path. The pipe will extract information from the source
-and process it for downstream use with [language models](https://
-en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://
-en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://
-arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based
-(or multimodal) representation of the extracted information, carefully crafted
-to fit within context windows for any models from [gemma-7b](https://
-huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a
-variety of heuristics for optimal performance with vision-language models,
-including AI filetype detection with [filetype detection](https://
-opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-
-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token
-compression](https://arxiv.org/abs/2403.12968), automatic [image encoding]
-(https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/
-2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects,
-and more, all pre-built to work out-of-the-box. ## Supported File Types ð |
-Source Type | Input types | Token Compression ðï¸ | Image Extraction
-ðï¸ | Notes ð | |---------------------------------------|---------------
----------------------------|-------------------|------------------|------------
----------------------------------------------| | Directory | Any `/path/to/
-directory` | âï¸ | âï¸ | Extracts from all files in directory, supports
-match and ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`,
-`.cpp`, etc | âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`,
-`.py` are compressible with ctags, others are not | | Plaintext | `.txt`,
-`.md`, `.rtf`, etc | âï¸ | â | Regular text files | | PDF | `.pdf` |
-âï¸ | âï¸ | Extracts text and images of each page; can use AI for
-extraction of table data and images within pages | | Image | `.jpg`, `.jpeg`,
-`.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | â | âï¸ | Extracts
-images, uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx` | âï¸
-| â | Extracts data from spreadsheets; converts to text representation. For
-very large datasets, will only extract column names and types | | Jupyter
-Notebook | `.ipynb` | â | âï¸ | Extracts code, markdown, and images from
-Jupyter notebooks | | Microsoft Word Document | `.docx` | âï¸ | âï¸ |
-Extracts text and images from Word documents | | Microsoft PowerPoint
-Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images from
-PowerPoint presentations | | Website | URLs (inputs containing `http`, `https`,
-`ftp`) | âï¸ | âï¸ | Extracts text from web page along with image (or
-images if scrollable); text-only extraction available | | GitHub Repository |
-GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub repositories;
-supports branch specification | | ZIP File | `.zip` | âï¸ | âï¸ |
-Extracts contents of ZIP files; supports nested directory extraction | ## Local
-Installation ð ï¸ To use The Pipe locally, you will need [playwright](https:
-//github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/
-), [pytesseract](https://github.com/h/pytesseract), and the local python
+assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Features ð - Extracts
+text and visuals from files or web pages ð - Outputs chunks optimized for
+multimodal LLMs ð¼ï¸ - Interpret complex PDFs, web pages, slides, CSVs, and
+more ð§  - Auto-compress prompts exceeding your chosen token limit ð¦ -
+Works even with missing file extensions, in-memory data streams ð¾ - Works
+with codebases, git repos, and custom integrations ð - Multi-threaded â¡ï¸
+## Getting Started ð First, install The Pipe. ``` pip install thepipe_api
+``` Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API
+key yet? [Get one here](https://thepi.pe). Alternatively, see the local
+installation section for the more advanced local setup. Now you can extract
+comprehensive text and visuals from any file: ```python from thepipe_api import
+thepipe chunks = thepipe.extract("example.pdf") ``` Or any website: ```python
+chunks = thepipe.extract("https://example.com") ``` Then feed it into GPT-4-
+Vision: ```python response = client.chat.completions.create( model="gpt-4-
+vision-preview", messages = chunks, ) ``` The Pipe's output is a list of
+sensible "chunks", and thus can be used either for storage in a vector database
+or for direct use as a prompt. Extra features such as data table extraction,
+bar chart extraction, custom web authentications and more are available in the
+[API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/
+BerriAI/litellm) can be used to easily integrate The Pipe with any LLM
+provider. You can also use The Pipe from the command line. Here's how to
+recursively extract from a directory: ``` thepipe path/to/folder ``` ## How it
+works ð ï¸ The pipe is accessible from the command line or from [Python]
+(https://www.python.org/downloads/). The input source is either a file path, a
+URL, or a directory. The pipe will extract information from the source and
+process it for downstream use with [language models](https://en.wikipedia.org/
+wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/
+wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/
+2304.00685). The output from the pipe is a sensible text-based (or multimodal)
+representation of the extracted information, carefully crafted to fit within
+context windows for any models from [gemma-7b](https://huggingface.co/google/
+gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a variety of heuristics
+for optimal performance with vision-language models, including AI filetype
+detection with [filetype detection](https://opensource.googleblog.com/2024/02/
+magika-ai-powered-fast-and-efficient-file-type-identification.html), AI [PDF
+extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/
+abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/
+Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle]
+(https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work
+out-of-the-box. ## Supported File Types ð | Source Type | Input types |
+Token Compression ðï¸ | Image Extraction ðï¸ | Notes ð | |----------
+-----------------------------|------------------------------------------|------
+-------------|------------------|----------------------------------------------
+-----------| | Directory | Any `/path/to/directory` | âï¸ | âï¸ |
+Extracts from all files in directory, supports match and ignore patterns | |
+Code | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | âï¸ (varies) |
+â | Combines all code files. `.c`, `.cpp`, `.py` are compressible with ctags,
+others are not | | Plaintext | `.txt`, `.md`, `.rtf`, etc | âï¸ | â |
+Regular text files | | PDF | `.pdf` | âï¸ | âï¸ | Extracts text and
+images of each page; can use AI for extraction of table data and images within
+pages | | Image | `.jpg`, `.jpeg`, `.png` | â | âï¸ | Extracts images,
+uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx` | âï¸ | â |
+Extracts data from spreadsheets; converts to text representation. For very
+large datasets, will only extract column names and types | | Jupyter Notebook |
+`.ipynb` | â | âï¸ | Extracts code, markdown, and images from Jupyter
+notebooks | | Microsoft Word Document | `.docx` | âï¸ | âï¸ | Extracts
+text and images from Word documents | | Microsoft PowerPoint Presentation |
+`.pptx` | âï¸ | âï¸ | Extracts text and images from PowerPoint
+presentations | | Website | URLs (inputs containing `http`, `https`, `ftp`) |
+âï¸ | âï¸ | Extracts text from web page along with image (or images if
+scrollable); text-only extraction available | | GitHub Repository | GitHub repo
+URLs | âï¸ | âï¸ | Extracts from GitHub repositories; supports branch
+specification | | ZIP File | `.zip` | âï¸ | âï¸ | Extracts contents of
+ZIP files; supports nested directory extraction | ## Local Installation ð ï¸
+To use The Pipe locally, you will need [playwright](https://github.com/
+microsoft/playwright), [ctags](https://github.com/universal-ctags/),
+[pytesseract](https://github.com/h/pytesseract), and the local python
 requirements, which differ from the more lightweight API requirements. You will
 also need to use the local version of the requirements file: ```bash git clone
 https://github.com/emcf/thepipe pip install -r requirements_local.txt ``` Tip
 for windows users: you may need to install the python-libmagic binaries with
-`pip install python-magic-bin`. Now you can use The Pipe: ```bash from
-thepipe_api import thepipe chunks = thepipe.extract("example.pdf", local=True)
-``` Arguments are: - `source` (required): can be a file path, a URL, or a
-directory path. - `local` (optional): Use the local version of The Pipe instead
-of the hosted API. - `match` (optional): Regex pattern to match files in the
-directory. - `ignore` (optional): Regex pattern to ignore files in the
-directory. - `limit` (optional): The token limit for the output prompt,
+`pip install python-magic-bin`. You may also need to ensure the tesseract-ocr
+binaries and the ctags binaries are in your PATH. Now you can use The Pipe with
+Python: ```bash from thepipe_api import thepipe chunks = thepipe.extract
+("example.pdf", local=True) ``` or from the command line: ```bash thepipe path/
+to/folder --local ``` Arguments are: - `source` (required): can be a file path,
+a URL, or a directory path. - `local` (optional): Use the local version of The
+Pipe instead of the hosted API. - `match` (optional): Regex pattern to match
+files in the directory. - `ignore` (optional): Regex pattern to ignore files in
+the directory. - `limit` (optional): The token limit for the output prompt,
 defaults to 100K. Prompts exceeding the limit will be compressed. -
 `ai_extraction` (optional): Extract tables, figures, and math from PDFs using
 our extractor. Incurs extra costs. - `text_only` (optional): Do not extract
 images from documents or websites. Additionally, image files will be
 represented with OCR instead of as images.
```

### Comparing `thepipe_api-0.2.0/setup.py` & `thepipe_api-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='thepipe_api',
-    version='0.2.0',
+    version='0.2.2',
     author='Emmett McFarlane',
     author_email='emmett@thepi.pe',
     description='Automate information extraction for multimodal LLMs.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/emcf/thepipe',
     packages=find_packages(),
```

### Comparing `thepipe_api-0.2.0/tests/test_thepipe.py` & `thepipe_api-0.2.2/tests/test_thepipe.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,32 +40,27 @@
         for message in messages:
             self.assertEqual(type(message), dict)
             self.assertIn('role', message)
             self.assertIn('content', message)
     
     def test_extract_from_source(self):
         # test extracting examples for all supported file type
-        chunks = extractor.extract_from_source(source=self.files_directory)
+        chunks = extractor.extract_from_source(source=self.files_directory, ignore="unknown")
         self.assertEqual(type(chunks), list)
         for chunk in chunks:
             self.assertEqual(type(chunk), core.Chunk)
             self.assertIsNotNone(chunk.path)
             self.assertIsNotNone(chunk.text or chunk.image)
-        # ensure unknown sources still acknowledges the existence of the source
-        chunks = extractor.extract_from_source(source='none')
-        self.assertEqual(type(chunks), list)
-        self.assertEqual(len(chunks), 1)
-        # ensure a chunk is still created to acknowledge the existence of an unknown source
-        chunks = extractor.extract_from_source(source=self.files_directory+"/example.unknown")
-        self.assertEqual(type(chunks), list)
-        self.assertEqual(len(chunks), 1)
+        # ensure unknown sources fail (test has "unknown in filename)
+        with self.assertRaises(Exception):
+            chunks = extractor.extract_from_source(source=self.files_directory+"/example.unknown")
 
     def test_extract_from_source_text_only(self):
         # test extracting examples for all supported file type
-        chunks = extractor.extract_from_source(source=self.files_directory, text_only=True)
+        chunks = extractor.extract_from_source(source=self.files_directory, text_only=True, ignore="unknown")
         self.assertEqual(type(chunks), list)
         # ensure no images are extracted
         for chunk in chunks:
             self.assertEqual(type(chunk), core.Chunk)
             self.assertIsNone(chunk.image)
 
     def test_should_ignore(self):
```

### Comparing `thepipe_api-0.2.0/thepipe_api/compressor.py` & `thepipe_api-0.2.2/thepipe_api/compressor.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.2.0/thepipe_api/core.py` & `thepipe_api-0.2.2/thepipe_api/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,19 +27,19 @@
         self.path = path
         self.text = text
         self.image = image
         self.source_type = source_type
 
 def print_status(text: str, status: str) -> None:
     if status == 'success':
-        message = Fore.GREEN + f"{text} ✔️"
+        message = Fore.GREEN + f"{text}"
     elif status == 'info':
         message = Fore.YELLOW + f"{text}..."
     elif status == 'error':
-        message = Fore.RED + f"{text} ❌"
+        message = Fore.RED + f"{text}"
     print(Style.RESET_ALL + message + Style.RESET_ALL)
 
 def count_tokens(chunks: List[Chunk]) -> int:
     return sum([((len(chunk.path) if chunk.path else 0) + (len(chunk.text) if chunk.text else 0))/4 for chunk in chunks])
 
 def image_to_base64(image: Image.Image) -> str:
     buffered = BytesIO()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `thepipe_api-0.2.0/thepipe_api/extractor.py` & `thepipe_api-0.2.2/thepipe_api/extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import os
 import tempfile
 from urllib.parse import urlparse
 import zipfile
 from PIL import Image
 import requests
 import json
-import fitz
 from .core import Chunk, print_status, SourceTypes, create_chunks_from_messages, API_URL
 import tempfile
 import mimetypes
 
 FILES_TO_IGNORE = {'package-lock.json', '.gitignore', '.bin', '.pyc', '.pyo', '.exe', '.bat', '.dll', '.obj', '.o', '.a', '.lib', '.so', '.dylib', '.ncb', '.sdf', '.suo', '.pdb', '.idb', '.pyd', '.ipynb_checkpoints', '.npy', '.pth'} # Files to ignore, please feel free to customize!
 CODE_EXTENSIONS = {'.h', '.json', '.js', '.jsx', '.ts', '.tsx',  '.cs', '.java', '.html', '.css', '.ini', '.xml', '.yaml', '.xaml', '.sh'} # Plaintext files that should not be compressed with LLMLingua
 CTAGS_CODE_EXTENSIONS = {'.c', '.cpp', '.py'} # code files that work with ctags
@@ -24,23 +23,23 @@
 SPREADSHEET_EXTENSIONS = {'.csv', '.xls', '.xlsx'}
 DOCUMENT_EXTENSIONS = {'.pdf', '.docx', '.pptx'}
 OTHER_EXTENSIONS = {'.zip', '.ipynb'}
 KNOWN_EXTENSIONS = IMAGE_EXTENSIONS.union(CODE_EXTENSIONS).union(CTAGS_CODE_EXTENSIONS).union(PLAINTEXT_EXTENSIONS).union(IMAGE_EXTENSIONS).union(SPREADSHEET_EXTENSIONS).union(DOCUMENT_EXTENSIONS).union(OTHER_EXTENSIONS)
 GITHUB_TOKEN: str = os.getenv("GITHUB_TOKEN")
 THEPIPE_API_KEY: str = os.getenv("THEPIPE_API_KEY")
 
-def extract_from_source(source: str, match: Optional[str] = None, ignore: Optional[str] = None, limit: int = 64000, verbose: bool = False, ai_extraction: bool = False, text_only: bool = False, local: bool = True) -> List[Chunk]:
+def extract_from_source(source: str, match: Optional[str] = None, ignore: Optional[str] = None, limit: int = None, verbose: bool = False, ai_extraction: bool = False, text_only: bool = False, local: bool = True) -> List[Chunk]:
     source_type = detect_type(source)
     if source_type is None:
-        return [Chunk(path=source)]
+        raise ValueError(f"Could not detect source type for {source}.")
     if verbose: print_status(f"Extracting from {source_type.value}", status='info')
     if source_type == SourceTypes.DIR or source == '.' or source == './':
         if source == '.' or source == './':
             source = os.getcwd()
-        return extract_from_directory(dir_path=source, match=match, ignore=ignore, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only)
+        return extract_from_directory(dir_path=source, match=match, ignore=ignore, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only, limit=limit)
     elif source_type == SourceTypes.GITHUB:
         return extract_github(github_url=source, file_path='', match=match, ignore=ignore, text_only=text_only, verbose=verbose, ai_extraction=ai_extraction, branch='master')
     elif source_type == SourceTypes.URL:
         return extract_url(url=source, text_only=text_only, local=local)
     elif source_type == SourceTypes.ZIP:
         return extract_zip(file_path=source, match=match, ignore=ignore, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only)
     return extract_from_file(file_path=source, source_type=source_type, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only, local=local)
@@ -145,21 +144,21 @@
         return True
     if any(x in file_path for x in ['node_modules', 'venv', '.git', '.vscode', '__pycache__']):
         return True
     if not os.path.isfile(file_path):
         return True
     return False
 
-def extract_from_directory(dir_path: str, match: Optional[str] = None, ignore: Optional[str] = None, verbose: bool = False, ai_extraction: bool = False, text_only: bool = False) -> List[Chunk]:
+def extract_from_directory(dir_path: str, match: Optional[str] = None, ignore: Optional[str] = None, verbose: bool = False, ai_extraction: bool = False, text_only: bool = False, limit: int = None) -> List[Chunk]:
     all_files = glob.glob(dir_path + "/**/*", recursive=True)
     matched_files = [file for file in all_files if re.search(match, file, re.IGNORECASE)] if match else all_files
     file_paths = [file for file in matched_files if not should_ignore(file, ignore)]
     contents = []
     with ThreadPoolExecutor() as executor:
-        results = executor.map(lambda file_path: extract_from_source(source=file_path, match=match, ignore=ignore, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only), file_paths)
+        results = executor.map(lambda file_path: extract_from_source(source=file_path, match=match, ignore=ignore, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only, limit=limit), file_paths)
         for result in results:
             contents += result
     return contents
 
 def extract_zip(file_path: str, match: Optional[str] = None, ignore: Optional[str] = None, verbose: bool = False, ai_extraction: bool = False, text_only: bool = False) -> List[Chunk]:
     extracted_files = []
     with tempfile.TemporaryDirectory() as temp_dir:
@@ -179,14 +178,15 @@
             )
             response_json = response.json()
             if 'error' in response_json:
                 raise ValueError(f"{response_json['error']}")
             messages = response_json['messages']
             chunks = create_chunks_from_messages(messages)
     else:
+        import fitz
         # extract text and images of each page from the PDF
         with open(file_path, 'rb') as file:
             doc = fitz.open(file_path)
             for page in doc:
                 text = page.get_text()
                 if text_only:
                     chunks.append(Chunk(path=file_path, text=text, image=None, source_type=SourceTypes.PDF))
```

### Comparing `thepipe_api-0.2.0/thepipe_api/thepipe.py` & `thepipe_api-0.2.2/thepipe_api/thepipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     text = ""
     n_images = 0
     for i, chunk in enumerate(chunks):
         if chunk is None:
             continue
         if chunk.text is not None:
             text += f"""{chunk.path}:\n```\n{chunk.text}\n```\n\n"""
-        if chunk.image is not None:
+        if (chunk.image is not None) and (not text_only):
             if chunk.path is None:
                 clean_path = f"image"
             else:
                 clean_path = chunk.path.replace('/', '_').replace('\\', '_')
                 clean_path = re.sub(r"[^a-zA-Z0-9 _]", "", clean_path)
             chunk.image.convert('RGB').save(f'outputs/{clean_path}_{i}.jpg')
             n_images += 1
@@ -39,15 +39,15 @@
     return final_prompt
 
 def parse_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(description='Compress project files into a context prompt.')
     parser.add_argument('source', type=str, help='The source file or directory to compress.')
     parser.add_argument('--match', type=str, default=None, help='The glob filename pattern to match in the directory. Glob notation, not regex. Only matches filenames, not paths.')
     parser.add_argument('--ignore', type=str, default=None, help='The regex filepath pattern to ignore in the directory. Regex notation, not glob. Matches filenames and paths.')
-    parser.add_argument('--limit', type=float, default=1e5, help='The token limit for the compressed project context.')
+    parser.add_argument('--limit', type=int, default=None, help='The token limit for the compressed project context.')
     parser.add_argument('--ai_extraction', action='store_true', help='Use ai_extraction to extract text from images.')
     parser.add_argument('--text_only', action='store_true', help='Extract only text from the source.')
     parser.add_argument('--quiet', action='store_true', help='Do not print status messages.')
     parser.add_argument('--local', action='store_true', help='Use local machine to extract data. Not recommended for systems with limited resources.')
     args = parser.parse_args()
     verbose = not args.quiet
     args.verbose = verbose
```

### Comparing `thepipe_api-0.2.0/thepipe_api.egg-info/PKG-INFO` & `thepipe_api-0.2.2/thepipe_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.2.0
+Version: 0.2.2
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 Requires-Dist: Pyarrow
 Requires-Dist: python-magic
 Requires-Dist: colorama
 Requires-Dist: requests
 Requires-Dist: pillow
 Requires-Dist: cssutils
 Requires-Dist: beautifulsoup4
-Requires-Dist: PyMuPDF
+Requires-Dist: magika
 
 
 # <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
 <p>
   <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
 </p>
 
@@ -32,22 +32,32 @@
 
 ### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
 
 The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally.
 
 ![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
 
+## Features 🌟
+
+- Extracts text and visuals from files or web pages 📚
+- Outputs chunks optimized for multimodal LLMs 🖼️
+- Interpret complex PDFs, web pages, slides, CSVs, and more 🧠
+- Auto-compress prompts exceeding your chosen token limit 📦
+- Works even with missing file extensions, in-memory data streams 💾
+- Works with codebases, git repos, and custom integrations 🌐
+- Multi-threaded ⚡️
+
 ## Getting Started  🚀
 
 First, install The Pipe. 
 ```
 pip install thepipe_api
 ```
 
-Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key yet? [Get one here](https://thepi.pe). Looking to operate it yourself locally instead? See the local installation section.
+Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key yet? [Get one here](https://thepi.pe). Alternatively, see the local installation section for the more advanced local setup.
 
 Now you can extract comprehensive text and visuals from any file:
 ```python
 from thepipe_api import thepipe
 chunks = thepipe.extract("example.pdf")
 ```
 Or any website:
@@ -64,37 +74,27 @@
 The Pipe's output is a list of sensible "chunks", and thus can be used either for storage in a vector database or for direct use as a prompt. Extra features such as data table extraction, bar chart extraction, custom web authentications and more are available in the [API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to easily integrate The Pipe with any LLM provider.
 
 You can also use The Pipe from the command line. Here's how to recursively extract from a directory:
 ```
 thepipe path/to/folder
 ```
 
-## Features 🌟
-
-- Extracts text and visuals from any file or web page 📚
-- Outputs RAG-ready chunks, optimized for multimodal LLMs 🖼️ + 💬
-- Can interpret complex PDFs, web apps, markdown, etc 🧠
-- Auto-compress prompts exceeding your chosen token limit 📦
-- Works with missing file extensions, in-memory data streams 💾
-- Works with codebases, URL, git repos, and more 🌐
-- Multi-threaded ⚡️
-
 ##  How it works 🛠️
 
-The pipe is accessible from the command line or from [Python](https://www.python.org/downloads/). The input source is either a file path, a URL, or a directory (or zip file) path. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based (or multimodal) representation of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
+The pipe is accessible from the command line or from [Python](https://www.python.org/downloads/). The input source is either a file path, a URL, or a directory. The pipe will extract information from the source and process it for downstream use with [language models](https://en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based (or multimodal) representation of the extracted information, carefully crafted to fit within context windows for any models from [gemma-7b](https://huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a variety of heuristics for optimal performance with vision-language models, including AI filetype detection with [filetype detection](https://opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work out-of-the-box.
 
 ## Supported File Types 📚
 
 | Source Type                           | Input types        | Token Compression 🗜️ | Image Extraction 👁️ | Notes 📌                                                  |
 |---------------------------------------|------------------------------------------|-------------------|------------------|---------------------------------------------------------|
 | Directory                             | Any `/path/to/directory`                 | ✔️               | ✔️               | Extracts from all files in directory, supports match and ignore patterns |
 | Code                                  | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | ✔️ (varies)   | ❌               | Combines all code files. `.c`, `.cpp`, `.py` are compressible with ctags, others are not |
 | Plaintext                             | `.txt`, `.md`, `.rtf`, etc               | ✔️               | ❌               | Regular text files                                                      |
 | PDF                                   | `.pdf`                                  | ✔️               | ✔️    | Extracts text and images of each page; can use AI for extraction of table data and  images within pages |
-| Image                                 | `.jpg`, `.jpeg`, `.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
+| Image                                 | `.jpg`, `.jpeg`, `.png` | ❌                | ✔️              | Extracts images, uses OCR if text_only                        |
 | Data Table                           | `.csv`, `.xls`, `.xlsx`             | ✔️                | ❌               | Extracts data from spreadsheets; converts to text representation. For very large datasets, will only extract column names and types         |
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
 | Website                               | URLs (inputs containing `http`, `https`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
@@ -104,22 +104,27 @@
 To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements. You will also need to use the local version of the requirements file:
 
 ```bash
 git clone https://github.com/emcf/thepipe
 pip install -r requirements_local.txt
 ```
 
-Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`.
+Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`. You may also need to ensure the tesseract-ocr binaries and the ctags binaries are in your PATH.
 
-Now you can use The Pipe:
+Now you can use The Pipe with Python:
 ```bash
 from thepipe_api import thepipe
 chunks = thepipe.extract("example.pdf", local=True)
 ```
 
+or from the command line:
+```bash
+thepipe path/to/folder --local
+```
+
 Arguments are:
 - `source` (required): can be a file path, a URL, or a directory path.
 - `local` (optional): Use the local version of The Pipe instead of the hosted API.
 - `match` (optional): Regex pattern to match files in the directory.
 - `ignore` (optional): Regex pattern to ignore files in the directory.
 - `limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed.
 - `ai_extraction` (optional): Extract tables, figures, and math from PDFs using our extractor. Incurs extra costs.
```

#### html2text {}

```diff
@@ -1,107 +1,108 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.0 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.2.2 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
 pillow Requires-Dist: cssutils Requires-Dist: beautifulsoup4 Requires-Dist:
-PyMuPDF # _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
+magika # _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
 _E_n_g_l_i_s_h | _ä_¸_­_æ__
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/
 badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-
 action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/
 badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
 _A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
 docs, slides, web pages and more into Vision-LLMs with one line of code â¡ The
 Pipe is a multimodal-first tool for feeding files and web pages into vision-
 language models such as GPT-4V. It is best for LLM and RAG applications that
 require a deep understanding of tricky data sources. The Pipe is available as a
 hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. !
 [Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/
-assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Getting Started ð First,
-install The Pipe. ``` pip install thepipe_api ``` Ensure the `THEPIPE_API_KEY`
-environment variable is set. Don't have an API key yet? [Get one here](https://
-thepi.pe). Looking to operate it yourself locally instead? See the local
-installation section. Now you can extract comprehensive text and visuals from
-any file: ```python from thepipe_api import thepipe chunks = thepipe.extract
-("example.pdf") ``` Or any website: ```python chunks = thepipe.extract("https:/
-/example.com") ``` Then feed it into GPT-4-Vision: ```python response =
-client.chat.completions.create( model="gpt-4-vision-preview", messages =
-chunks, ) ``` The Pipe's output is a list of sensible "chunks", and thus can be
-used either for storage in a vector database or for direct use as a prompt.
-Extra features such as data table extraction, bar chart extraction, custom web
-authentications and more are available in the [API documentation](https://
-thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/litellm) can be used to
-easily integrate The Pipe with any LLM provider. You can also use The Pipe from
-the command line. Here's how to recursively extract from a directory: ```
-thepipe path/to/folder ``` ## Features ð - Extracts text and visuals from
-any file or web page ð - Outputs RAG-ready chunks, optimized for multimodal
-LLMs ð¼ï¸ + ð¬ - Can interpret complex PDFs, web apps, markdown, etc ð§ 
-- Auto-compress prompts exceeding your chosen token limit ð¦ - Works with
-missing file extensions, in-memory data streams ð¾ - Works with codebases,
-URL, git repos, and more ð - Multi-threaded â¡ï¸ ## How it works ð ï¸
-The pipe is accessible from the command line or from [Python](https://
-www.python.org/downloads/). The input source is either a file path, a URL, or a
-directory (or zip file) path. The pipe will extract information from the source
-and process it for downstream use with [language models](https://
-en.wikipedia.org/wiki/Large_language_model), [vision transformers](https://
-en.wikipedia.org/wiki/Vision_transformer), or [vision-language models](https://
-arxiv.org/abs/2304.00685). The output from the pipe is a sensible text-based
-(or multimodal) representation of the extracted information, carefully crafted
-to fit within context windows for any models from [gemma-7b](https://
-huggingface.co/google/gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a
-variety of heuristics for optimal performance with vision-language models,
-including AI filetype detection with [filetype detection](https://
-opensource.googleblog.com/2024/02/magika-ai-powered-fast-and-efficient-file-
-type-identification.html), AI [PDF extraction](thepi.pe/docs), efficient [token
-compression](https://arxiv.org/abs/2403.12968), automatic [image encoding]
-(https://en.wikipedia.org/wiki/Base64), [reranking](https://arxiv.org/abs/
-2310.06839) for [lost-in-the-middle](https://arxiv.org/abs/2307.03172) effects,
-and more, all pre-built to work out-of-the-box. ## Supported File Types ð |
-Source Type | Input types | Token Compression ðï¸ | Image Extraction
-ðï¸ | Notes ð | |---------------------------------------|---------------
----------------------------|-------------------|------------------|------------
----------------------------------------------| | Directory | Any `/path/to/
-directory` | âï¸ | âï¸ | Extracts from all files in directory, supports
-match and ignore patterns | | Code | `.py`, `.tsx`, `.js`, `.html`, `.css`,
-`.cpp`, etc | âï¸ (varies) | â | Combines all code files. `.c`, `.cpp`,
-`.py` are compressible with ctags, others are not | | Plaintext | `.txt`,
-`.md`, `.rtf`, etc | âï¸ | â | Regular text files | | PDF | `.pdf` |
-âï¸ | âï¸ | Extracts text and images of each page; can use AI for
-extraction of table data and images within pages | | Image | `.jpg`, `.jpeg`,
-`.png`, `.gif`, `.bmp`, `.tiff`, `.webp`, `.svg` | â | âï¸ | Extracts
-images, uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx` | âï¸
-| â | Extracts data from spreadsheets; converts to text representation. For
-very large datasets, will only extract column names and types | | Jupyter
-Notebook | `.ipynb` | â | âï¸ | Extracts code, markdown, and images from
-Jupyter notebooks | | Microsoft Word Document | `.docx` | âï¸ | âï¸ |
-Extracts text and images from Word documents | | Microsoft PowerPoint
-Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images from
-PowerPoint presentations | | Website | URLs (inputs containing `http`, `https`,
-`ftp`) | âï¸ | âï¸ | Extracts text from web page along with image (or
-images if scrollable); text-only extraction available | | GitHub Repository |
-GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub repositories;
-supports branch specification | | ZIP File | `.zip` | âï¸ | âï¸ |
-Extracts contents of ZIP files; supports nested directory extraction | ## Local
-Installation ð ï¸ To use The Pipe locally, you will need [playwright](https:
-//github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/
-), [pytesseract](https://github.com/h/pytesseract), and the local python
+assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z) ## Features ð - Extracts
+text and visuals from files or web pages ð - Outputs chunks optimized for
+multimodal LLMs ð¼ï¸ - Interpret complex PDFs, web pages, slides, CSVs, and
+more ð§  - Auto-compress prompts exceeding your chosen token limit ð¦ -
+Works even with missing file extensions, in-memory data streams ð¾ - Works
+with codebases, git repos, and custom integrations ð - Multi-threaded â¡ï¸
+## Getting Started ð First, install The Pipe. ``` pip install thepipe_api
+``` Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API
+key yet? [Get one here](https://thepi.pe). Alternatively, see the local
+installation section for the more advanced local setup. Now you can extract
+comprehensive text and visuals from any file: ```python from thepipe_api import
+thepipe chunks = thepipe.extract("example.pdf") ``` Or any website: ```python
+chunks = thepipe.extract("https://example.com") ``` Then feed it into GPT-4-
+Vision: ```python response = client.chat.completions.create( model="gpt-4-
+vision-preview", messages = chunks, ) ``` The Pipe's output is a list of
+sensible "chunks", and thus can be used either for storage in a vector database
+or for direct use as a prompt. Extra features such as data table extraction,
+bar chart extraction, custom web authentications and more are available in the
+[API documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/
+BerriAI/litellm) can be used to easily integrate The Pipe with any LLM
+provider. You can also use The Pipe from the command line. Here's how to
+recursively extract from a directory: ``` thepipe path/to/folder ``` ## How it
+works ð ï¸ The pipe is accessible from the command line or from [Python]
+(https://www.python.org/downloads/). The input source is either a file path, a
+URL, or a directory. The pipe will extract information from the source and
+process it for downstream use with [language models](https://en.wikipedia.org/
+wiki/Large_language_model), [vision transformers](https://en.wikipedia.org/
+wiki/Vision_transformer), or [vision-language models](https://arxiv.org/abs/
+2304.00685). The output from the pipe is a sensible text-based (or multimodal)
+representation of the extracted information, carefully crafted to fit within
+context windows for any models from [gemma-7b](https://huggingface.co/google/
+gemma-7b) to [GPT-4](https://openai.com/gpt-4). It uses a variety of heuristics
+for optimal performance with vision-language models, including AI filetype
+detection with [filetype detection](https://opensource.googleblog.com/2024/02/
+magika-ai-powered-fast-and-efficient-file-type-identification.html), AI [PDF
+extraction](thepi.pe/docs), efficient [token compression](https://arxiv.org/
+abs/2403.12968), automatic [image encoding](https://en.wikipedia.org/wiki/
+Base64), [reranking](https://arxiv.org/abs/2310.06839) for [lost-in-the-middle]
+(https://arxiv.org/abs/2307.03172) effects, and more, all pre-built to work
+out-of-the-box. ## Supported File Types ð | Source Type | Input types |
+Token Compression ðï¸ | Image Extraction ðï¸ | Notes ð | |----------
+-----------------------------|------------------------------------------|------
+-------------|------------------|----------------------------------------------
+-----------| | Directory | Any `/path/to/directory` | âï¸ | âï¸ |
+Extracts from all files in directory, supports match and ignore patterns | |
+Code | `.py`, `.tsx`, `.js`, `.html`, `.css`, `.cpp`, etc | âï¸ (varies) |
+â | Combines all code files. `.c`, `.cpp`, `.py` are compressible with ctags,
+others are not | | Plaintext | `.txt`, `.md`, `.rtf`, etc | âï¸ | â |
+Regular text files | | PDF | `.pdf` | âï¸ | âï¸ | Extracts text and
+images of each page; can use AI for extraction of table data and images within
+pages | | Image | `.jpg`, `.jpeg`, `.png` | â | âï¸ | Extracts images,
+uses OCR if text_only | | Data Table | `.csv`, `.xls`, `.xlsx` | âï¸ | â |
+Extracts data from spreadsheets; converts to text representation. For very
+large datasets, will only extract column names and types | | Jupyter Notebook |
+`.ipynb` | â | âï¸ | Extracts code, markdown, and images from Jupyter
+notebooks | | Microsoft Word Document | `.docx` | âï¸ | âï¸ | Extracts
+text and images from Word documents | | Microsoft PowerPoint Presentation |
+`.pptx` | âï¸ | âï¸ | Extracts text and images from PowerPoint
+presentations | | Website | URLs (inputs containing `http`, `https`, `ftp`) |
+âï¸ | âï¸ | Extracts text from web page along with image (or images if
+scrollable); text-only extraction available | | GitHub Repository | GitHub repo
+URLs | âï¸ | âï¸ | Extracts from GitHub repositories; supports branch
+specification | | ZIP File | `.zip` | âï¸ | âï¸ | Extracts contents of
+ZIP files; supports nested directory extraction | ## Local Installation ð ï¸
+To use The Pipe locally, you will need [playwright](https://github.com/
+microsoft/playwright), [ctags](https://github.com/universal-ctags/),
+[pytesseract](https://github.com/h/pytesseract), and the local python
 requirements, which differ from the more lightweight API requirements. You will
 also need to use the local version of the requirements file: ```bash git clone
 https://github.com/emcf/thepipe pip install -r requirements_local.txt ``` Tip
 for windows users: you may need to install the python-libmagic binaries with
-`pip install python-magic-bin`. Now you can use The Pipe: ```bash from
-thepipe_api import thepipe chunks = thepipe.extract("example.pdf", local=True)
-``` Arguments are: - `source` (required): can be a file path, a URL, or a
-directory path. - `local` (optional): Use the local version of The Pipe instead
-of the hosted API. - `match` (optional): Regex pattern to match files in the
-directory. - `ignore` (optional): Regex pattern to ignore files in the
-directory. - `limit` (optional): The token limit for the output prompt,
+`pip install python-magic-bin`. You may also need to ensure the tesseract-ocr
+binaries and the ctags binaries are in your PATH. Now you can use The Pipe with
+Python: ```bash from thepipe_api import thepipe chunks = thepipe.extract
+("example.pdf", local=True) ``` or from the command line: ```bash thepipe path/
+to/folder --local ``` Arguments are: - `source` (required): can be a file path,
+a URL, or a directory path. - `local` (optional): Use the local version of The
+Pipe instead of the hosted API. - `match` (optional): Regex pattern to match
+files in the directory. - `ignore` (optional): Regex pattern to ignore files in
+the directory. - `limit` (optional): The token limit for the output prompt,
 defaults to 100K. Prompts exceeding the limit will be compressed. -
 `ai_extraction` (optional): Extract tables, figures, and math from PDFs using
 our extractor. Incurs extra costs. - `text_only` (optional): Do not extract
 images from documents or websites. Additionally, image files will be
 represented with OCR instead of as images.
```

