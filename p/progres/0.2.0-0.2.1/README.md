# Comparing `tmp/progres-0.2.0.tar.gz` & `tmp/progres-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progres-0.2.0.tar", last modified: Wed Mar 29 16:19:18 2023, max compression
+gzip compressed data, was "progres-0.2.1.tar", last modified: Wed Apr 17 18:16:41 2024, max compression
```

## Comparing `progres-0.2.0.tar` & `progres-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2023-03-29 16:19:18.795895 progres-0.2.0/
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)     2231 2022-11-15 17:59:33.000000 progres-0.2.0/LICENSE
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)    10820 2023-03-29 16:19:18.795895 progres-0.2.0/PKG-INFO
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)    10246 2023-03-29 16:15:52.000000 progres-0.2.0/README.md
-drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2023-03-29 16:19:18.791895 progres-0.2.0/bin/
--rwxrwxr-x   0 jgreener  (1000) jgreener  (1000)     3870 2023-03-28 15:15:10.000000 progres-0.2.0/bin/progres
-drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2023-03-29 16:19:18.795895 progres-0.2.0/progres/
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       23 2022-11-16 16:19:38.000000 progres-0.2.0/progres/__init__.py
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)    21478 2023-03-29 15:37:25.000000 progres-0.2.0/progres/progres.py
-drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2023-03-29 16:19:18.795895 progres-0.2.0/progres.egg-info/
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)    10820 2023-03-29 16:19:18.000000 progres-0.2.0/progres.egg-info/PKG-INFO
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)      231 2023-03-29 16:19:18.000000 progres-0.2.0/progres.egg-info/SOURCES.txt
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)        1 2023-03-29 16:19:18.000000 progres-0.2.0/progres.egg-info/dependency_links.txt
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       29 2023-03-29 16:19:18.000000 progres-0.2.0/progres.egg-info/requires.txt
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)        8 2023-03-29 16:19:18.000000 progres-0.2.0/progres.egg-info/top_level.txt
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       38 2023-03-29 16:19:18.795895 progres-0.2.0/setup.cfg
--rw-rw-r--   0 jgreener  (1000) jgreener  (1000)      914 2023-03-24 16:05:36.000000 progres-0.2.0/setup.py
+drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-04-17 18:16:41.381106 progres-0.2.1/
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)     3635 2024-04-15 18:40:30.000000 progres-0.2.1/LICENSE
+-rw-r--r--   0 jgreener  (1000) jgreener  (1000)    12718 2024-04-17 18:16:41.381106 progres-0.2.1/PKG-INFO
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)    12067 2024-04-17 17:35:48.000000 progres-0.2.1/README.md
+drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-04-17 18:16:41.377106 progres-0.2.1/bin/
+-rwxrwxr-x   0 jgreener  (1000) jgreener  (1000)     3876 2024-04-17 17:04:22.000000 progres-0.2.1/bin/progres
+drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-04-17 18:16:41.377106 progres-0.2.1/progres/
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       23 2022-11-16 16:19:38.000000 progres-0.2.1/progres/__init__.py
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)    23732 2024-04-17 17:30:15.000000 progres-0.2.1/progres/progres.py
+drwxrwxr-x   0 jgreener  (1000) jgreener  (1000)        0 2024-04-17 18:16:41.381106 progres-0.2.1/progres.egg-info/
+-rw-r--r--   0 jgreener  (1000) jgreener  (1000)    12718 2024-04-17 18:16:41.000000 progres-0.2.1/progres.egg-info/PKG-INFO
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)      231 2024-04-17 18:16:41.000000 progres-0.2.1/progres.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)        1 2024-04-17 18:16:41.000000 progres-0.2.1/progres.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       29 2024-04-17 18:16:41.000000 progres-0.2.1/progres.egg-info/requires.txt
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)        8 2024-04-17 18:16:41.000000 progres-0.2.1/progres.egg-info/top_level.txt
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)       38 2024-04-17 18:16:41.381106 progres-0.2.1/setup.cfg
+-rw-rw-r--   0 jgreener  (1000) jgreener  (1000)      917 2024-04-17 09:53:40.000000 progres-0.2.1/setup.py
```

### Comparing `progres-0.2.0/PKG-INFO` & `progres-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,33 @@
-Metadata-Version: 2.1
-Name: progres
-Version: 0.2.0
-Summary: Fast protein structure searching using structure graph embeddings
-Home-page: https://github.com/jgreener64/progres
-Author: Joe G Greener
-Author-email: jgreener@mrc-lmb.cam.ac.uk
-License: MIT
-Keywords: protein structure search graph embedding
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Progres - Protein Graph Embedding Search
 
-[![Build status](https://github.com/jgreener64/progres/workflows/CI/badge.svg)](https://github.com/jgreener64/progres/actions)
+[![Build status](https://github.com/greener-group/progres/workflows/CI/badge.svg)](https://github.com/greener-group/progres/actions)
 
 This repository contains the method from the pre-print:
 
-Greener JG and Jamali K. Fast protein structure searching using structure graph embeddings. bioRxiv (2022) - [link](https://www.biorxiv.org/content/10.1101/2022.11.28.518224v1)
-
-It provides the `progres` Python package that lets you search structures against pre-embedded structural databases and pre-embed datasets for searching against. Searching typically takes 1-2 s and is faster for multiple queries. Currently [SCOPe](https://scop.berkeley.edu), [CATH](http://cathdb.info), [ECOD](http://prodata.swmed.edu/ecod) and the [AlphaFold structures for 21 model organisms](https://doi.org/10.1093/nar/gkab1061) are provided for searching against. We may add others such as the whole [AlphaFold database](https://alphafold.ebi.ac.uk) and the [ESM Metagenomic Atlas](https://esmatlas.com) in future.
+- Greener JG and Jamali K. Fast protein structure searching using structure graph embeddings. bioRxiv (2022) - [link](https://www.biorxiv.org/content/10.1101/2022.11.28.518224)
 
-This is work in progress software - the implementation, API and results may change.
-Appropriate version numbers will distinguish versions.
-Since the pre-print the model has been updated and the AlphaFold structures have been made available to search against.
-Please open issues or [contact me](http://jgreener64.github.io) with any feedback.
-Training scripts and datasets will be made available on publication.
+It provides the `progres` Python package that lets you search structures against pre-embedded structural databases and pre-embed datasets for searching against.
+Searching typically takes 1-2 s and is much faster for multiple queries.
+For the AlphaFold database, initial data loading takes around a minute but subsequent searching takes a tenth of a second per query.
+Currently [SCOPe](https://scop.berkeley.edu), [CATH](http://cathdb.info), [ECOD](http://prodata.swmed.edu/ecod), the [AlphaFold structures for 21 model organisms](https://doi.org/10.1093/nar/gkab1061) and the [AlphaFold database TED domains](https://www.biorxiv.org/content/10.1101/2024.03.18.585509) are provided for searching against.
 
 ## Installation
 
-1. Python 3.6 or later is required. The software is OS-independent.
-2. Install [PyTorch](https://pytorch.org) 1.11 or later, [PyTorch Scatter](https://github.com/rusty1s/pytorch_scatter) and [PyTorch Geometric](https://github.com/pyg-team/pytorch_geometric) as appropriate for your system. A GPU is not required and will only provide speedup in certain situations since multiple workers can be used on CPU. Example commands:
+1. Python 3.8 or later is required. The software is OS-independent.
+2. Install [PyTorch](https://pytorch.org) 1.11 or later, [PyTorch Scatter](https://github.com/rusty1s/pytorch_scatter), [PyTorch Geometric](https://github.com/pyg-team/pytorch_geometric) and [FAISS](https://github.com/facebookresearch/faiss) as appropriate for your system. A GPU is not required and will only provide speedup in certain situations since multiple workers can be used on CPU. Example commands:
 ```bash
-conda install pytorch==1.12.0 -c pytorch
+conda create -n prog python=3.9
+conda activate prog
+conda install pytorch=1.11 faiss-cpu -c pytorch
 conda install pytorch-scatter pyg -c pyg
 ```
-
 3. Run `pip install progres`, which will also install [Biopython](https://biopython.org), [mmtf-python](https://github.com/rcsb/mmtf-python) and [einops](https://github.com/arogozhnikov/einops) if they are not already present.
-4. The first time you run the software the trained model and pre-embedded databases (~340 MB) will be downloaded to the package directory from [Zenodo](https://zenodo.org/record/7782088), which requires an internet connection. This can take a few minutes.
+4. The first time you search with the software the trained model and pre-embedded databases (~220 MB) will be downloaded to the package directory from [Zenodo](https://zenodo.org/record/7782088), which requires an internet connection. This can take a few minutes.
+5. The first time you search against the AlphaFold database TED domains the pre-embedded database (~33 GB) will be downloaded in a similar way. This can take a while. Make sure you have enough disk space!
 
 ## Usage
 
 On Unix systems the executable `progres` will be added to the path during installation.
 On Windows you can call the `bin/progres` script with python if you can't access the executable.
 
 Run `progres -h` to see the help text and `progres {mode} -h` to see the help text for each mode.
@@ -58,59 +41,65 @@
 progres search -q query.pdb -t scope95
 ```
 ```
 # QUERY_NUM: 1
 # QUERY: query.pdb
 # QUERY_SIZE: 150 residues
 # DATABASE: scope95
-# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.0
+# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.1
 # HIT_N  DOMAIN   HIT_NRES  SIMILARITY  NOTES
       1  d1a6ja_       150      1.0000  d.112.1.1 - Nitrogen regulatory bacterial protein IIa-ntr {Escherichia coli [TaxId: 562]}
       2  d2a0ja_       146      0.9988  d.112.1.0 - automated matches {Neisseria meningitidis [TaxId: 122586]}
       3  d3urra1       151      0.9983  d.112.1.0 - automated matches {Burkholderia thailandensis [TaxId: 271848]}
       4  d3lf6a_       154      0.9971  d.112.1.1 - automated matches {Artificial gene [TaxId: 32630]}
       5  d3oxpa1       147      0.9968  d.112.1.0 - automated matches {Yersinia pestis [TaxId: 214092]}
 ...
 ```
 - `-q` is the path to the query structure file. Alternatively, `-l` is a text file with one query file path per line and each result will be printed in turn. This is considerably faster for multiple queries since setup only occurs once and multiple workers can be used.
 - `-t` is the pre-embedded database to search against. Currently this must be either one of the databases listed below or the file path to a pre-embedded dataset generated with `progres embed`.
 - `-f` determines the file format of the query structure (`guess`, `pdb`, `mmcif`, `mmtf` or `coords`). By default this is guessed from the file extension, with `pdb` chosen if a guess can't be made. `coords` refers to a text file with the coordinates of a Cα atom separated by white space on each line.
-- `-s` is the minimum similarity threshold above which to return hits, default 0.8.
+- `-s` is the minimum similarity threshold above which to return hits, default 0.8. As discussed in the paper, 0.8 indicates the same fold.
 - `-m` is the maximum number of hits to return, default 100.
 
 Query structures should be a single protein domain, though it can be discontinuous (chain IDs are ignored).
-You can slice out domains manually using software such as the `pdb_selres` command from [pdb-tools](http://www.bonvinlab.org/pdb-tools).
+Tools such as [Merizo](https://github.com/psipred/Merizo), [SWORD2](https://www.dsimb.inserm.fr/SWORD2) and [Chainsaw](https://github.com/JudeWells/chainsaw) can be used to predict domains from a larger structure.
+You can also slice out domains manually using software such as the `pdb_selres` command from [pdb-tools](http://www.bonvinlab.org/pdb-tools).
 
 Interpreting the hit descriptions depends on the database being searched.
 The domain name often includes a reference to the corresponding PDB file, for example d1a6ja_ refers to PDB ID 1A6J chain A, and this can be opened in the [RCSB PDB structure view](https://www.rcsb.org/3d-view/1A6J/1) to get a quick look.
+For the AlphaFold database TED domains, files can be downloaded from [links such as this](https://alphafold.ebi.ac.uk/files/AF-A0A6J8EXE6-F1-model_v4.pdb) where `AF-A0A6J8EXE6-F1` is the first part of the hit notes and is followed by the residue range of the domain.
 
 The available pre-embedded databases are:
 
-| Name      | Description                                                                                                                                                | Number of domains | Search time (1 query) | Search time (100 queries) |
-| --------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------- | --------------------- | ------------------------- |
-| `scope95` | ASTRAL set of [SCOPe](https://scop.berkeley.edu) 2.08 domains clustered at 95% seq ID                                                                      | 35,371            | 1.43 s                | 2.47 s                    |
-| `scope40` | ASTRAL set of [SCOPe](https://scop.berkeley.edu) 2.08 domains clustered at 40% seq ID                                                                      | 15,127            | 1.36 s                | 2.25 s                    |
-| `cath40`  | S40 non-redundant domains from [CATH](http://cathdb.info) 23/11/22                                                                                         | 31,884            | 1.44 s                | 2.42 s                    |
-| `ecod70`  | F70 representative domains from [ECOD](http://prodata.swmed.edu/ecod) develop287                                                                           | 71,635            | 1.48 s                | 3.36 s                    |
-| `af21org` | [AlphaFold](https://alphafold.ebi.ac.uk) structures for 21 model organisms split into domains by [CATH-Assign](https://doi.org/10.1038/s42003-023-04488-9) | 338,258           | 2.15 s                | 7.88 s                    |
+| Name      | Description                                                                                                                                                                                | Number of domains | Search time (1 query)      | Search time (100 queries)  |
+| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------- | -------------------------- | -------------------------- |
+| `scope95` | ASTRAL set of [SCOPe](https://scop.berkeley.edu) 2.08 domains clustered at 95% seq ID                                                                                                      | 35,371            | 1.35 s                     | 2.81 s                     |
+| `scope40` | ASTRAL set of [SCOPe](https://scop.berkeley.edu) 2.08 domains clustered at 40% seq ID                                                                                                      | 15,127            | 1.32 s                     | 2.36 s                     |
+| `cath40`  | S40 non-redundant domains from [CATH](http://cathdb.info) 23/11/22                                                                                                                         | 31,884            | 1.38 s                     | 2.79 s                     |
+| `ecod70`  | F70 representative domains from [ECOD](http://prodata.swmed.edu/ecod) develop287                                                                                                           | 71,635            | 1.46 s                     | 3.82 s                     |
+| `af21org` | [AlphaFold](https://alphafold.ebi.ac.uk) structures for 21 model organisms split into domains by [CATH-Assign](https://doi.org/10.1038/s42003-023-04488-9)                                 | 338,258           | 2.21 s                     | 11.0 s                     |
+| `afted`   | [AlphaFold database](https://alphafold.ebi.ac.uk) structures split into domains by [TED](https://www.biorxiv.org/content/10.1101/2024.03.18.585509) and clustered at 50% sequence identity | 53,344,209        | 67.7 s                     | 73.1 s                     |
 
 Search time is for a 150 residue protein (d1a6ja_ in PDB format) on an Intel i9-10980XE CPU with 256 GB RAM and PyTorch 1.11.
 Times are given for 1 or 100 queries.
+Note that `afted` uses exhaustive FAISS searching.
+This doesn't change the hits that are found, but the similarity score will differ by a small amount - see the paper.
 
 ## Pre-embed a dataset to search against
 
 To embed a dataset of structures, allowing it to be searched against:
 ```bash
 progres embed -l filepaths.txt -o searchdb.pt
 ```
 - `-l` is a text file with information on one structure per line, each of which will be one entry in the output. White space should separate the file path to the structure and the domain name, with optionally any additional text being treated as a note for the notes column of the results.
 - `-o` is the output file path for the PyTorch file containing a dictionary with the embeddings and associated data. It can be read in with `torch.load`.
 - `-f` determines the file format of each structure as above (`guess`, `pdb`, `mmcif`, `mmtf` or `coords`).
 
 Again, the structures should correspond to single protein domains.
+The embeddings are stored as Float16, which has no noticeable effect on search performance.
 
 ## Python library
 
 `progres` can also be used in Python, allowing it to be integrated into other methods:
 ```python
 import progres as pg
 
@@ -129,29 +118,40 @@
 graph = pg.read_graph("query.pdb")
 graph # Data(x=[150, 67], edge_index=[2, 2758], coords=[150, 3])
 
 # Embed a single structure
 embedding = pg.embed_structure("query.pdb")
 embedding.shape # torch.Size([128])
 
+# Load and reuse the model for speed
+model = pg.load_trained_model()
+embedding = pg.embed_structure("query.pdb", model=model)
+
 # Embed Cα coordinates and search with the embedding
 # This is useful for using progres in existing pipelines that give out Cα coordinates
 # queryembeddings should have shape (128) or (n, 128)
 #   and should be normalised across the 128 dimension
 coords = pg.read_coords("query.pdb")
 embedding = pg.embed_coords(coords) # Can take a list of coords or a tensor of shape (nres, 3)
 results = pg.progres_search(queryembeddings=embedding, targetdb="scope95")
 
 # Get the similarity score (0 to 1) between two embeddings
 # The distance (1 - similarity) is also available as pg.embedding_distance
 score = pg.embedding_similarity(embedding, embedding)
 score # tensor(1.) in this case since they are the same embedding
 
 # Get all-v-all similarity scores between 1000 embeddings
-embs = torch.nn.functional.normalize(torch.rand(1000, 128), dim=1)
+embs = torch.nn.functional.normalize(torch.randn(1000, 128), dim=1)
 scores = pg.embedding_similarity(embs.unsqueeze(0), embs.unsqueeze(1))
 scores.shape # torch.Size([1000, 1000])
 ```
 
+## Scripts
+
+Datasets and scripts for benchmarking (including for other methods), FAISS index generation and training are in the `scripts` directory.
+The trained model and pre-embedded databases are available on [Zenodo](https://zenodo.org/record/7782088).
+
 ## Notes
 
 The implementation of the E(n)-equivariant GNN uses [EGNN PyTorch](https://github.com/lucidrains/egnn-pytorch).
+
+Please open issues or [get in touch](http://jgreener64.github.io) with any feedback.
```

### Comparing `progres-0.2.0/README.md` & `progres-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,52 @@
+Metadata-Version: 2.1
+Name: progres
+Version: 0.2.1
+Summary: Fast protein structure searching using structure graph embeddings
+Home-page: https://github.com/greener-group/progres
+Author: Joe G Greener
+Author-email: jgreener@mrc-lmb.cam.ac.uk
+License: MIT
+Keywords: protein structure search graph embedding
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: biopython
+Requires-Dist: mmtf-python
+Requires-Dist: einops
+
 # Progres - Protein Graph Embedding Search
 
-[![Build status](https://github.com/jgreener64/progres/workflows/CI/badge.svg)](https://github.com/jgreener64/progres/actions)
+[![Build status](https://github.com/greener-group/progres/workflows/CI/badge.svg)](https://github.com/greener-group/progres/actions)
 
 This repository contains the method from the pre-print:
 
-Greener JG and Jamali K. Fast protein structure searching using structure graph embeddings. bioRxiv (2022) - [link](https://www.biorxiv.org/content/10.1101/2022.11.28.518224v1)
-
-It provides the `progres` Python package that lets you search structures against pre-embedded structural databases and pre-embed datasets for searching against. Searching typically takes 1-2 s and is faster for multiple queries. Currently [SCOPe](https://scop.berkeley.edu), [CATH](http://cathdb.info), [ECOD](http://prodata.swmed.edu/ecod) and the [AlphaFold structures for 21 model organisms](https://doi.org/10.1093/nar/gkab1061) are provided for searching against. We may add others such as the whole [AlphaFold database](https://alphafold.ebi.ac.uk) and the [ESM Metagenomic Atlas](https://esmatlas.com) in future.
+- Greener JG and Jamali K. Fast protein structure searching using structure graph embeddings. bioRxiv (2022) - [link](https://www.biorxiv.org/content/10.1101/2022.11.28.518224)
 
-This is work in progress software - the implementation, API and results may change.
-Appropriate version numbers will distinguish versions.
-Since the pre-print the model has been updated and the AlphaFold structures have been made available to search against.
-Please open issues or [contact me](http://jgreener64.github.io) with any feedback.
-Training scripts and datasets will be made available on publication.
+It provides the `progres` Python package that lets you search structures against pre-embedded structural databases and pre-embed datasets for searching against.
+Searching typically takes 1-2 s and is much faster for multiple queries.
+For the AlphaFold database, initial data loading takes around a minute but subsequent searching takes a tenth of a second per query.
+Currently [SCOPe](https://scop.berkeley.edu), [CATH](http://cathdb.info), [ECOD](http://prodata.swmed.edu/ecod), the [AlphaFold structures for 21 model organisms](https://doi.org/10.1093/nar/gkab1061) and the [AlphaFold database TED domains](https://www.biorxiv.org/content/10.1101/2024.03.18.585509) are provided for searching against.
 
 ## Installation
 
-1. Python 3.6 or later is required. The software is OS-independent.
-2. Install [PyTorch](https://pytorch.org) 1.11 or later, [PyTorch Scatter](https://github.com/rusty1s/pytorch_scatter) and [PyTorch Geometric](https://github.com/pyg-team/pytorch_geometric) as appropriate for your system. A GPU is not required and will only provide speedup in certain situations since multiple workers can be used on CPU. Example commands:
+1. Python 3.8 or later is required. The software is OS-independent.
+2. Install [PyTorch](https://pytorch.org) 1.11 or later, [PyTorch Scatter](https://github.com/rusty1s/pytorch_scatter), [PyTorch Geometric](https://github.com/pyg-team/pytorch_geometric) and [FAISS](https://github.com/facebookresearch/faiss) as appropriate for your system. A GPU is not required and will only provide speedup in certain situations since multiple workers can be used on CPU. Example commands:
 ```bash
-conda install pytorch==1.12.0 -c pytorch
+conda create -n prog python=3.9
+conda activate prog
+conda install pytorch=1.11 faiss-cpu -c pytorch
 conda install pytorch-scatter pyg -c pyg
 ```
-
 3. Run `pip install progres`, which will also install [Biopython](https://biopython.org), [mmtf-python](https://github.com/rcsb/mmtf-python) and [einops](https://github.com/arogozhnikov/einops) if they are not already present.
-4. The first time you run the software the trained model and pre-embedded databases (~340 MB) will be downloaded to the package directory from [Zenodo](https://zenodo.org/record/7782088), which requires an internet connection. This can take a few minutes.
+4. The first time you search with the software the trained model and pre-embedded databases (~220 MB) will be downloaded to the package directory from [Zenodo](https://zenodo.org/record/7782088), which requires an internet connection. This can take a few minutes.
+5. The first time you search against the AlphaFold database TED domains the pre-embedded database (~33 GB) will be downloaded in a similar way. This can take a while. Make sure you have enough disk space!
 
 ## Usage
 
 On Unix systems the executable `progres` will be added to the path during installation.
 On Windows you can call the `bin/progres` script with python if you can't access the executable.
 
 Run `progres -h` to see the help text and `progres {mode} -h` to see the help text for each mode.
@@ -42,59 +60,65 @@
 progres search -q query.pdb -t scope95
 ```
 ```
 # QUERY_NUM: 1
 # QUERY: query.pdb
 # QUERY_SIZE: 150 residues
 # DATABASE: scope95
-# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.0
+# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.1
 # HIT_N  DOMAIN   HIT_NRES  SIMILARITY  NOTES
       1  d1a6ja_       150      1.0000  d.112.1.1 - Nitrogen regulatory bacterial protein IIa-ntr {Escherichia coli [TaxId: 562]}
       2  d2a0ja_       146      0.9988  d.112.1.0 - automated matches {Neisseria meningitidis [TaxId: 122586]}
       3  d3urra1       151      0.9983  d.112.1.0 - automated matches {Burkholderia thailandensis [TaxId: 271848]}
       4  d3lf6a_       154      0.9971  d.112.1.1 - automated matches {Artificial gene [TaxId: 32630]}
       5  d3oxpa1       147      0.9968  d.112.1.0 - automated matches {Yersinia pestis [TaxId: 214092]}
 ...
 ```
 - `-q` is the path to the query structure file. Alternatively, `-l` is a text file with one query file path per line and each result will be printed in turn. This is considerably faster for multiple queries since setup only occurs once and multiple workers can be used.
 - `-t` is the pre-embedded database to search against. Currently this must be either one of the databases listed below or the file path to a pre-embedded dataset generated with `progres embed`.
 - `-f` determines the file format of the query structure (`guess`, `pdb`, `mmcif`, `mmtf` or `coords`). By default this is guessed from the file extension, with `pdb` chosen if a guess can't be made. `coords` refers to a text file with the coordinates of a Cα atom separated by white space on each line.
-- `-s` is the minimum similarity threshold above which to return hits, default 0.8.
+- `-s` is the minimum similarity threshold above which to return hits, default 0.8. As discussed in the paper, 0.8 indicates the same fold.
 - `-m` is the maximum number of hits to return, default 100.
 
 Query structures should be a single protein domain, though it can be discontinuous (chain IDs are ignored).
-You can slice out domains manually using software such as the `pdb_selres` command from [pdb-tools](http://www.bonvinlab.org/pdb-tools).
+Tools such as [Merizo](https://github.com/psipred/Merizo), [SWORD2](https://www.dsimb.inserm.fr/SWORD2) and [Chainsaw](https://github.com/JudeWells/chainsaw) can be used to predict domains from a larger structure.
+You can also slice out domains manually using software such as the `pdb_selres` command from [pdb-tools](http://www.bonvinlab.org/pdb-tools).
 
 Interpreting the hit descriptions depends on the database being searched.
 The domain name often includes a reference to the corresponding PDB file, for example d1a6ja_ refers to PDB ID 1A6J chain A, and this can be opened in the [RCSB PDB structure view](https://www.rcsb.org/3d-view/1A6J/1) to get a quick look.
+For the AlphaFold database TED domains, files can be downloaded from [links such as this](https://alphafold.ebi.ac.uk/files/AF-A0A6J8EXE6-F1-model_v4.pdb) where `AF-A0A6J8EXE6-F1` is the first part of the hit notes and is followed by the residue range of the domain.
 
 The available pre-embedded databases are:
 
-| Name      | Description                                                                                                                                                | Number of domains | Search time (1 query) | Search time (100 queries) |
-| --------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------- | --------------------- | ------------------------- |
-| `scope95` | ASTRAL set of [SCOPe](https://scop.berkeley.edu) 2.08 domains clustered at 95% seq ID                                                                      | 35,371            | 1.43 s                | 2.47 s                    |
-| `scope40` | ASTRAL set of [SCOPe](https://scop.berkeley.edu) 2.08 domains clustered at 40% seq ID                                                                      | 15,127            | 1.36 s                | 2.25 s                    |
-| `cath40`  | S40 non-redundant domains from [CATH](http://cathdb.info) 23/11/22                                                                                         | 31,884            | 1.44 s                | 2.42 s                    |
-| `ecod70`  | F70 representative domains from [ECOD](http://prodata.swmed.edu/ecod) develop287                                                                           | 71,635            | 1.48 s                | 3.36 s                    |
-| `af21org` | [AlphaFold](https://alphafold.ebi.ac.uk) structures for 21 model organisms split into domains by [CATH-Assign](https://doi.org/10.1038/s42003-023-04488-9) | 338,258           | 2.15 s                | 7.88 s                    |
+| Name      | Description                                                                                                                                                                                | Number of domains | Search time (1 query)      | Search time (100 queries)  |
+| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------- | -------------------------- | -------------------------- |
+| `scope95` | ASTRAL set of [SCOPe](https://scop.berkeley.edu) 2.08 domains clustered at 95% seq ID                                                                                                      | 35,371            | 1.35 s                     | 2.81 s                     |
+| `scope40` | ASTRAL set of [SCOPe](https://scop.berkeley.edu) 2.08 domains clustered at 40% seq ID                                                                                                      | 15,127            | 1.32 s                     | 2.36 s                     |
+| `cath40`  | S40 non-redundant domains from [CATH](http://cathdb.info) 23/11/22                                                                                                                         | 31,884            | 1.38 s                     | 2.79 s                     |
+| `ecod70`  | F70 representative domains from [ECOD](http://prodata.swmed.edu/ecod) develop287                                                                                                           | 71,635            | 1.46 s                     | 3.82 s                     |
+| `af21org` | [AlphaFold](https://alphafold.ebi.ac.uk) structures for 21 model organisms split into domains by [CATH-Assign](https://doi.org/10.1038/s42003-023-04488-9)                                 | 338,258           | 2.21 s                     | 11.0 s                     |
+| `afted`   | [AlphaFold database](https://alphafold.ebi.ac.uk) structures split into domains by [TED](https://www.biorxiv.org/content/10.1101/2024.03.18.585509) and clustered at 50% sequence identity | 53,344,209        | 67.7 s                     | 73.1 s                     |
 
 Search time is for a 150 residue protein (d1a6ja_ in PDB format) on an Intel i9-10980XE CPU with 256 GB RAM and PyTorch 1.11.
 Times are given for 1 or 100 queries.
+Note that `afted` uses exhaustive FAISS searching.
+This doesn't change the hits that are found, but the similarity score will differ by a small amount - see the paper.
 
 ## Pre-embed a dataset to search against
 
 To embed a dataset of structures, allowing it to be searched against:
 ```bash
 progres embed -l filepaths.txt -o searchdb.pt
 ```
 - `-l` is a text file with information on one structure per line, each of which will be one entry in the output. White space should separate the file path to the structure and the domain name, with optionally any additional text being treated as a note for the notes column of the results.
 - `-o` is the output file path for the PyTorch file containing a dictionary with the embeddings and associated data. It can be read in with `torch.load`.
 - `-f` determines the file format of each structure as above (`guess`, `pdb`, `mmcif`, `mmtf` or `coords`).
 
 Again, the structures should correspond to single protein domains.
+The embeddings are stored as Float16, which has no noticeable effect on search performance.
 
 ## Python library
 
 `progres` can also be used in Python, allowing it to be integrated into other methods:
 ```python
 import progres as pg
 
@@ -113,29 +137,40 @@
 graph = pg.read_graph("query.pdb")
 graph # Data(x=[150, 67], edge_index=[2, 2758], coords=[150, 3])
 
 # Embed a single structure
 embedding = pg.embed_structure("query.pdb")
 embedding.shape # torch.Size([128])
 
+# Load and reuse the model for speed
+model = pg.load_trained_model()
+embedding = pg.embed_structure("query.pdb", model=model)
+
 # Embed Cα coordinates and search with the embedding
 # This is useful for using progres in existing pipelines that give out Cα coordinates
 # queryembeddings should have shape (128) or (n, 128)
 #   and should be normalised across the 128 dimension
 coords = pg.read_coords("query.pdb")
 embedding = pg.embed_coords(coords) # Can take a list of coords or a tensor of shape (nres, 3)
 results = pg.progres_search(queryembeddings=embedding, targetdb="scope95")
 
 # Get the similarity score (0 to 1) between two embeddings
 # The distance (1 - similarity) is also available as pg.embedding_distance
 score = pg.embedding_similarity(embedding, embedding)
 score # tensor(1.) in this case since they are the same embedding
 
 # Get all-v-all similarity scores between 1000 embeddings
-embs = torch.nn.functional.normalize(torch.rand(1000, 128), dim=1)
+embs = torch.nn.functional.normalize(torch.randn(1000, 128), dim=1)
 scores = pg.embedding_similarity(embs.unsqueeze(0), embs.unsqueeze(1))
 scores.shape # torch.Size([1000, 1000])
 ```
 
+## Scripts
+
+Datasets and scripts for benchmarking (including for other methods), FAISS index generation and training are in the `scripts` directory.
+The trained model and pre-embedded databases are available on [Zenodo](https://zenodo.org/record/7782088).
+
 ## Notes
 
 The implementation of the E(n)-equivariant GNN uses [EGNN PyTorch](https://github.com/lucidrains/egnn-pytorch).
+
+Please open issues or [get in touch](http://jgreener64.github.io) with any feedback.
```

### Comparing `progres-0.2.0/bin/progres` & `progres-0.2.1/bin/progres`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #!/usr/bin/env python
 
 # Argument handling
 
 import argparse
-import pkg_resources
+import importlib.metadata
 import sys
 
 parser = argparse.ArgumentParser(description=(
     "Fast protein structure searching using structure graph embeddings. "
-    "See https://github.com/jgreener64/progres for documentation and citation information. "
-    f"This is version {pkg_resources.get_distribution('progres').version} of the software."
+    "See https://github.com/greener-group/progres for documentation and citation information. "
+    f"This is version {importlib.metadata.version('progres')} of the software."
 ))
 subparsers = parser.add_subparsers(dest="mode",
     help="the mode to run progres in, run \"progres {mode} -h\" to see help for each")
 
 parser_search = subparsers.add_parser("search",
     description="Search one or more queries against a pre-embedded database.",
     help="search one or more queries against a pre-embedded database")
 parser_search.add_argument("-q", "--querystructure",
     help="query structure file in PDB/mmCIF/MMTF/coordinate format")
 parser_search.add_argument("-l", "--querylist",
     help="text file with one query file path per line")
 parser_search.add_argument("-t", "--targetdb", required=True,
     help=("pre-embedded database to search against, either "
-          "\"scope95\", \"scope40\", \"cath40\", \"ecod70\", \"af21org\" or a file path"))
+          "\"scope95\", \"scope40\", \"cath40\", \"ecod70\", \"af21org\", \"afted\" or a file path"))
 parser_search.add_argument("-f", "--fileformat",
     choices=["guess", "pdb", "mmcif", "mmtf", "coords"], default="guess",
     help="file format of the query structure(s), by default guessed from the file extension")
 parser_search.add_argument("-s", "--minsimilarity", type=float, default=0.8,
     help="similarity threshold above which to return hits, default 0.8")
 parser_search.add_argument("-m", "--maxhits", type=int, default=100,
     help="maximum number of hits to return, default 100")
@@ -60,14 +60,14 @@
                              fileformat=args.fileformat, minsimilarity=args.minsimilarity,
                              maxhits=args.maxhits, device=args.device)
     elif args.querylist:
         progres_search_print(querylist=args.querylist, targetdb=args.targetdb,
                              fileformat=args.fileformat, minsimilarity=args.minsimilarity,
                              maxhits=args.maxhits, device=args.device)
     else:
-        print("One of -q and -l must be given for structural searching", file=sys.stderr)
+        print("One of -q and -l must be given for structure searching", file=sys.stderr)
 elif args.mode == "embed":
     from progres import progres_embed
     progres_embed(structurelist=args.structurelist, outputfile=args.outputfile,
                   fileformat=args.fileformat, device=args.device)
 else:
     print("No mode selected, run \"progres -h\" to see help", file=sys.stderr)
```

### Comparing `progres-0.2.0/progres/progres.py` & `progres-0.2.1/progres/progres.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Fast protein structure searching using structure graph embeddings
 
-# biopython imported in a function
+# faiss and biopython imported in functions
 import torch
 from torch.nn import Dropout, Identity, Linear, Sequential, SiLU
 from torch.nn.functional import normalize
 from torch.utils.data import Dataset
 from torch_scatter import scatter
 from torch_geometric.data import Data
 from torch_geometric.loader import DataLoader
 from einops import rearrange
+import importlib.metadata
 from math import ceil
 import os
-import pkg_resources
 import sys
 from urllib import request
 
 n_layers = 6
 embedding_size = 128
 hidden_dim = 128
 hidden_egnn_dim = 64
@@ -25,17 +25,18 @@
 pos_embed_freq_inv = 2000
 contact_dist = 10.0 # Å
 dropout = 0.0
 dropout_final = 0.0
 default_minsimilarity = 0.8
 default_maxhits = 100
 pre_embedded_dbs = ["scope95", "scope40", "cath40", "ecod70", "af21org"]
-zenodo_record = "7782089" # This only needs to change when the trained model or databases change
+pre_embedded_dbs_faiss = ["afted"]
+zenodo_record = "10975201" # This only needs to change when the trained model or databases change
 trained_model_subdir = "v_0_2_0" # This only needs to change when the trained model changes
-database_subdir      = "v_0_2_0" # This only needs to change when the databases change
+database_subdir      = "v_0_2_1" # This only needs to change when the databases change
 progres_dir       = os.path.dirname(os.path.realpath(__file__))
 trained_model_dir = os.path.join(progres_dir, "trained_models", trained_model_subdir)
 database_dir      = os.path.join(progres_dir, "databases"     , database_subdir     )
 trained_model_fp  = os.path.join(trained_model_dir, "trained_model.pt")
 
 class SinusoidalPositionalEncoding(torch.nn.Module):
     def __init__(self, channels):
@@ -269,15 +270,16 @@
                 coords.append([float(v) for v in line.rstrip().split()])
     else:
         raise ValueError("fileformat must be \"guess\", \"pdb\", \"mmcif\", \"mmtf\" or \"coords\"")
     return coords
 
 def coords_to_graph(coords):
     n_res = len(coords)
-    coords = torch.tensor(coords)
+    if not isinstance(coords, torch.Tensor):
+        coords = torch.tensor(coords)
     if coords.size(1) != 3:
         raise ValueError("coords must be, or must be convertible to, a tensor of shape (nres, 3)")
     dmap = torch.cdist(coords.unsqueeze(0), coords.unsqueeze(0),
                        compute_mode="donot_use_mm_for_euclid_dist")
     contacts = (dmap <= contact_dist).squeeze(0)
     edge_index = contacts.to_sparse().indices()
 
@@ -315,77 +317,92 @@
     return coords_to_graph(coords)
 
 def embedding_distance(emb_1, emb_2):
     cosine_dist = (emb_1 * emb_2).sum(dim=-1) # Normalised in the model
     return (1 - cosine_dist) / 2 # Runs 0 (close) to 1 (far)
 
 def embedding_similarity(emb_1, emb_2):
-    return 1 - embedding_distance(emb_1, emb_2) # Runs 0 (far) to 1 (close)
+    cosine_dist = (emb_1 * emb_2).sum(dim=-1) # Normalised in the model
+    return (1 + cosine_dist) / 2 # Runs 0 (far) to 1 (close)
 
 def load_trained_model(device="cpu"):
     model = Model().to(device)
     loaded_model = torch.load(trained_model_fp, map_location=device)
     model.load_state_dict(loaded_model["model"])
     model.eval()
     return model
 
-def embed_graph(graph, device="cpu"):
+def embed_graph(graph, device="cpu", model=None):
     with torch.no_grad():
-        model = load_trained_model(device)
+        if model is None:
+            model = load_trained_model(device)
         data_loader = DataLoader([graph], batch_size=1)
         for batch in data_loader:
             emb = model(batch.to(device))
             break
         return emb.squeeze(0)
 
-def embed_coords(coords, device="cpu"):
+def embed_coords(coords, device="cpu", model=None):
     graph = coords_to_graph(coords)
-    return embed_graph(graph, device)
+    return embed_graph(graph, device, model)
 
-def embed_structure(querystructure, fileformat="guess", device="cpu"):
+def embed_structure(querystructure, fileformat="guess", device="cpu", model=None):
     graph = read_graph(querystructure, fileformat)
-    return embed_graph(graph, device)
+    return embed_graph(graph, device, model)
 
-def get_batch_size(device="cpu"):
-    return 8
+def get_batch_size(device="cpu", using_faiss=False):
+    if using_faiss:
+        return 64
+    else:
+        return 8
 
 def get_num_workers(device="cpu"):
     if device == "cpu":
         return torch.get_num_threads()
     else:
         return 0
 
-def download_data_if_required():
+def download_data_if_required(download_afted=False):
     url_base = f"https://zenodo.org/record/{zenodo_record}/files"
     fps = [trained_model_fp]
     urls = [f"{url_base}/trained_model.pt"]
     for targetdb in pre_embedded_dbs:
         fps.append(os.path.join(database_dir, targetdb + ".pt"))
         urls.append(f"{url_base}/{targetdb}.pt")
+    if download_afted:
+        for fn in ["afted.index", "afted_noembs.pt"]:
+            fps.append(os.path.join(database_dir, fn))
+            urls.append(f"{url_base}/{fn}")
 
     if not os.path.isdir(trained_model_dir):
         os.makedirs(trained_model_dir)
     if not os.path.isdir(database_dir):
         os.makedirs(database_dir)
 
     printed = False
     for fp, url in zip(fps, urls):
         if not os.path.isfile(fp):
+            if fp.endswith("afted.index"):
+                print("Downloading afted data as first time setup (~33 GB) to ", database_dir,
+                      ", internet connection required, this may take a while",
+                      sep="", file=sys.stderr)
+                printed = True
             if not printed:
-                print("Downloading data as first time setup (~340 MB) to ", progres_dir,
+                print("Downloading data as first time setup (~220 MB) to ", progres_dir,
                       ", internet connection required, this can take a few minutes",
                       sep="", file=sys.stderr)
                 printed = True
             try:
                 request.urlretrieve(url, fp)
-                d = torch.load(fp, map_location="cpu")
-                if fp == trained_model_fp:
-                    assert "model" in d
-                else:
-                    assert "embeddings" in d
+                if not fp.endswith("afted.index"):
+                    d = torch.load(fp, map_location="cpu")
+                    if fp == trained_model_fp:
+                        assert "model" in d
+                    else:
+                        assert "notes" in d
             except:
                 if os.path.isfile(fp):
                     os.remove(fp)
                 print("Failed to download from", url, "and save to", fp, file=sys.stderr)
                 print("Exiting", file=sys.stderr)
                 sys.exit(1)
 
@@ -396,21 +413,29 @@
                              targetdb=None, fileformat="guess", minsimilarity=default_minsimilarity,
                              maxhits=default_maxhits, device="cpu", batch_size=None):
     if querystructure is None and querylist is None and queryembeddings is None:
         raise ValueError("One of querystructure, querylist or queryembeddings must be given")
     if targetdb is None:
         raise ValueError("targetdb must be given")
 
-    download_data_if_required()
+    download_data_if_required(targetdb == "afted")
 
-    if targetdb in pre_embedded_dbs:
+    if targetdb in pre_embedded_dbs_faiss:
+        import faiss
+        print(f"Loading {targetdb} data, this can take a minute", file=sys.stderr)
+        target_index = faiss.read_index(os.path.join(database_dir, f"{targetdb}.index"))
+        target_data = torch.load(os.path.join(database_dir, f"{targetdb}_noembs.pt"), map_location=device)
+        search_type = "faiss"
+    elif targetdb in pre_embedded_dbs:
         target_fp = os.path.join(database_dir, targetdb + ".pt")
         target_data = torch.load(target_fp, map_location=device)
+        search_type = "torch"
     else:
         target_data = torch.load(targetdb, map_location=device)
+        search_type = "torch"
 
     model = load_trained_model(device)
     if querystructure is not None:
         query_fps = [querystructure]
         data_set = StructureDataset(query_fps, fileformat, model, device)
         num_workers = get_num_workers(device)
     elif querylist is not None:
@@ -422,35 +447,54 @@
         num_workers = get_num_workers(device)
     else:
         data_set = EmbeddingDataset(queryembeddings.to(device))
         query_fps = ["?"] * len(data_set)
         num_workers = 0
 
     if batch_size is None:
-        batch_size = get_batch_size(device)
-    data_loader = DataLoader(data_set, batch_size=batch_size, shuffle=False,
-                             num_workers=num_workers)
+        batch_size = get_batch_size(device, search_type == "faiss")
+    data_loader = DataLoader(
+        data_set,
+        batch_size=batch_size,
+        shuffle=False,
+        num_workers=num_workers,
+    )
 
     with torch.no_grad():
         qi = 0
         for embs, nress in data_loader:
+            if search_type == "faiss":
+                sims_ord_batch, inds_ord_batch = target_index.search(embs.cpu().numpy(), maxhits)
+
             for bi in range(embs.size(0)):
                 query_size = nress[bi].item() if type(nress) == torch.Tensor else "?"
-                dists = embedding_distance(embs[bi], target_data["embeddings"])
-                hits = dists.argsort()[:maxhits].to("cpu") # Move to CPU since we loop over
-
+                if search_type == "faiss":
+                    sims_ord = sims_ord_batch[bi]
+                    inds_ord = inds_ord_batch[bi]
+                else:
+                    dists = embedding_distance(embs[bi], target_data["embeddings"])
+                    inds_ord = dists.argsort()[:maxhits].to("cpu")
                 domids, hits_nres, similarities, notes = [], [], [], []
-                for i, di in enumerate(hits):
-                    similarity = (1 - dists[di]).item()
-                    if similarity < minsimilarity:
-                        break
-                    domids.append(target_data["ids"][di])
-                    hits_nres.append(target_data["nres"][di])
-                    similarities.append(similarity)
-                    notes.append(target_data["notes"][di])
+                if search_type == "faiss":
+                    for si, similarity in enumerate(sims_ord):
+                        if similarity < minsimilarity:
+                            break
+                        domids.append(target_data["ids"][inds_ord[si]])
+                        hits_nres.append(target_data["nres"][inds_ord[si]])
+                        similarities.append(similarity)
+                        notes.append(target_data["notes"][inds_ord[si]])
+                else:
+                    for i in inds_ord:
+                        similarity = (1 - dists[i]).item()
+                        if similarity < minsimilarity:
+                            break
+                        domids.append(target_data["ids"][i])
+                        hits_nres.append(target_data["nres"][i])
+                        similarities.append(similarity)
+                        notes.append(target_data["notes"][i])
 
                 result_dict = {
                     "query_num":     qi + 1,
                     "query":         query_fps[qi],
                     "query_size":    query_size,
                     "database":      targetdb,
                     "minsimilarity": minsimilarity,
@@ -472,29 +516,30 @@
     return list(generator)
 
 def progres_search_print(querystructure=None, querylist=None, queryembeddings=None, targetdb=None,
                          fileformat="guess", minsimilarity=default_minsimilarity,
                          maxhits=default_maxhits, device="cpu", batch_size=None):
     generator = progres_search_generator(querystructure, querylist, queryembeddings, targetdb,
                                          fileformat, minsimilarity, maxhits, device, batch_size)
-    version = pkg_resources.get_distribution("progres").version
+    version = importlib.metadata.version("progres")
 
     for rd in generator:
         n_hits = len(rd["domains"])
         inds_str = [str(i + 1) for i in range(n_hits)]
         hits_nres_str = [str(n) for n in rd["hits_nres"]]
         padding_inds      = max(len(s) for s in inds_str        + ["# HIT_N" ])
         padding_domids    = max(len(s) for s in rd["domains"]   + ["DOMAIN"  ])
         padding_hits_nres = max(len(s) for s in hits_nres_str   + ["HIT_NRES"])
+        faiss_str = ", FAISS search" if targetdb in pre_embedded_dbs_faiss else ""
 
         print("# QUERY_NUM:" , rd["query_num"])
         print("# QUERY:"     , rd["query"])
         print("# QUERY_SIZE:", rd["query_size"], "residues")
         print("# DATABASE:", targetdb)
-        print(f"# PARAMETERS: minsimilarity {minsimilarity}, maxhits {maxhits}, progres v{version}")
+        print(f"# PARAMETERS: minsimilarity {minsimilarity}, maxhits {maxhits}, progres v{version}{faiss_str}")
         print("  ".join([
             "#" + " HIT_N".rjust(padding_inds - 1),
             "DOMAIN".ljust(padding_domids),
             "HIT_NRES".rjust(padding_hits_nres),
             "SIMILARITY",
             "NOTES",
         ]))
@@ -519,26 +564,30 @@
             domids.append(cols[1])
             notes.append(cols[2] if len(cols) > 2 else "-")
 
     model = load_trained_model(device)
     data_set = StructureDataset(fps, fileformat, model, device)
     if batch_size is None:
         batch_size = get_batch_size(device)
-    data_loader = DataLoader(data_set, batch_size=batch_size, shuffle=False,
-                             num_workers=get_num_workers(device))
+    data_loader = DataLoader(
+        data_set,
+        batch_size=batch_size,
+        shuffle=False,
+        num_workers=get_num_workers(device),
+    )
 
     with torch.no_grad():
         embeddings = torch.zeros(len(data_set), embedding_size, device=device)
         n_residues = torch.zeros(len(data_set), dtype=torch.int, device=device)
         for bi, (embs, nress) in enumerate(data_loader):
             embeddings[(bi * batch_size):(bi * batch_size + embs.size(0))] = embs
             n_residues[(bi * batch_size):(bi * batch_size + embs.size(0))] = nress.squeeze(1)
 
     torch.save(
         {
             "ids"       : domids,
-            "embeddings": embeddings.cpu(),
+            "embeddings": embeddings.cpu().to(torch.float16),
             "nres"      : list(n_residues.cpu().numpy()),
             "notes"     : notes,
         },
         outputfile,
     )
```

### Comparing `progres-0.2.0/progres.egg-info/PKG-INFO` & `progres-0.2.1/progres.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 Metadata-Version: 2.1
 Name: progres
-Version: 0.2.0
+Version: 0.2.1
 Summary: Fast protein structure searching using structure graph embeddings
-Home-page: https://github.com/jgreener64/progres
+Home-page: https://github.com/greener-group/progres
 Author: Joe G Greener
 Author-email: jgreener@mrc-lmb.cam.ac.uk
 License: MIT
 Keywords: protein structure search graph embedding
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biopython
+Requires-Dist: mmtf-python
+Requires-Dist: einops
 
 # Progres - Protein Graph Embedding Search
 
-[![Build status](https://github.com/jgreener64/progres/workflows/CI/badge.svg)](https://github.com/jgreener64/progres/actions)
+[![Build status](https://github.com/greener-group/progres/workflows/CI/badge.svg)](https://github.com/greener-group/progres/actions)
 
 This repository contains the method from the pre-print:
 
-Greener JG and Jamali K. Fast protein structure searching using structure graph embeddings. bioRxiv (2022) - [link](https://www.biorxiv.org/content/10.1101/2022.11.28.518224v1)
+- Greener JG and Jamali K. Fast protein structure searching using structure graph embeddings. bioRxiv (2022) - [link](https://www.biorxiv.org/content/10.1101/2022.11.28.518224)
 
-It provides the `progres` Python package that lets you search structures against pre-embedded structural databases and pre-embed datasets for searching against. Searching typically takes 1-2 s and is faster for multiple queries. Currently [SCOPe](https://scop.berkeley.edu), [CATH](http://cathdb.info), [ECOD](http://prodata.swmed.edu/ecod) and the [AlphaFold structures for 21 model organisms](https://doi.org/10.1093/nar/gkab1061) are provided for searching against. We may add others such as the whole [AlphaFold database](https://alphafold.ebi.ac.uk) and the [ESM Metagenomic Atlas](https://esmatlas.com) in future.
-
-This is work in progress software - the implementation, API and results may change.
-Appropriate version numbers will distinguish versions.
-Since the pre-print the model has been updated and the AlphaFold structures have been made available to search against.
-Please open issues or [contact me](http://jgreener64.github.io) with any feedback.
-Training scripts and datasets will be made available on publication.
+It provides the `progres` Python package that lets you search structures against pre-embedded structural databases and pre-embed datasets for searching against.
+Searching typically takes 1-2 s and is much faster for multiple queries.
+For the AlphaFold database, initial data loading takes around a minute but subsequent searching takes a tenth of a second per query.
+Currently [SCOPe](https://scop.berkeley.edu), [CATH](http://cathdb.info), [ECOD](http://prodata.swmed.edu/ecod), the [AlphaFold structures for 21 model organisms](https://doi.org/10.1093/nar/gkab1061) and the [AlphaFold database TED domains](https://www.biorxiv.org/content/10.1101/2024.03.18.585509) are provided for searching against.
 
 ## Installation
 
-1. Python 3.6 or later is required. The software is OS-independent.
-2. Install [PyTorch](https://pytorch.org) 1.11 or later, [PyTorch Scatter](https://github.com/rusty1s/pytorch_scatter) and [PyTorch Geometric](https://github.com/pyg-team/pytorch_geometric) as appropriate for your system. A GPU is not required and will only provide speedup in certain situations since multiple workers can be used on CPU. Example commands:
+1. Python 3.8 or later is required. The software is OS-independent.
+2. Install [PyTorch](https://pytorch.org) 1.11 or later, [PyTorch Scatter](https://github.com/rusty1s/pytorch_scatter), [PyTorch Geometric](https://github.com/pyg-team/pytorch_geometric) and [FAISS](https://github.com/facebookresearch/faiss) as appropriate for your system. A GPU is not required and will only provide speedup in certain situations since multiple workers can be used on CPU. Example commands:
 ```bash
-conda install pytorch==1.12.0 -c pytorch
+conda create -n prog python=3.9
+conda activate prog
+conda install pytorch=1.11 faiss-cpu -c pytorch
 conda install pytorch-scatter pyg -c pyg
 ```
-
 3. Run `pip install progres`, which will also install [Biopython](https://biopython.org), [mmtf-python](https://github.com/rcsb/mmtf-python) and [einops](https://github.com/arogozhnikov/einops) if they are not already present.
-4. The first time you run the software the trained model and pre-embedded databases (~340 MB) will be downloaded to the package directory from [Zenodo](https://zenodo.org/record/7782088), which requires an internet connection. This can take a few minutes.
+4. The first time you search with the software the trained model and pre-embedded databases (~220 MB) will be downloaded to the package directory from [Zenodo](https://zenodo.org/record/7782088), which requires an internet connection. This can take a few minutes.
+5. The first time you search against the AlphaFold database TED domains the pre-embedded database (~33 GB) will be downloaded in a similar way. This can take a while. Make sure you have enough disk space!
 
 ## Usage
 
 On Unix systems the executable `progres` will be added to the path during installation.
 On Windows you can call the `bin/progres` script with python if you can't access the executable.
 
 Run `progres -h` to see the help text and `progres {mode} -h` to see the help text for each mode.
@@ -58,59 +60,65 @@
 progres search -q query.pdb -t scope95
 ```
 ```
 # QUERY_NUM: 1
 # QUERY: query.pdb
 # QUERY_SIZE: 150 residues
 # DATABASE: scope95
-# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.0
+# PARAMETERS: minsimilarity 0.8, maxhits 100, progres v0.2.1
 # HIT_N  DOMAIN   HIT_NRES  SIMILARITY  NOTES
       1  d1a6ja_       150      1.0000  d.112.1.1 - Nitrogen regulatory bacterial protein IIa-ntr {Escherichia coli [TaxId: 562]}
       2  d2a0ja_       146      0.9988  d.112.1.0 - automated matches {Neisseria meningitidis [TaxId: 122586]}
       3  d3urra1       151      0.9983  d.112.1.0 - automated matches {Burkholderia thailandensis [TaxId: 271848]}
       4  d3lf6a_       154      0.9971  d.112.1.1 - automated matches {Artificial gene [TaxId: 32630]}
       5  d3oxpa1       147      0.9968  d.112.1.0 - automated matches {Yersinia pestis [TaxId: 214092]}
 ...
 ```
 - `-q` is the path to the query structure file. Alternatively, `-l` is a text file with one query file path per line and each result will be printed in turn. This is considerably faster for multiple queries since setup only occurs once and multiple workers can be used.
 - `-t` is the pre-embedded database to search against. Currently this must be either one of the databases listed below or the file path to a pre-embedded dataset generated with `progres embed`.
 - `-f` determines the file format of the query structure (`guess`, `pdb`, `mmcif`, `mmtf` or `coords`). By default this is guessed from the file extension, with `pdb` chosen if a guess can't be made. `coords` refers to a text file with the coordinates of a Cα atom separated by white space on each line.
-- `-s` is the minimum similarity threshold above which to return hits, default 0.8.
+- `-s` is the minimum similarity threshold above which to return hits, default 0.8. As discussed in the paper, 0.8 indicates the same fold.
 - `-m` is the maximum number of hits to return, default 100.
 
 Query structures should be a single protein domain, though it can be discontinuous (chain IDs are ignored).
-You can slice out domains manually using software such as the `pdb_selres` command from [pdb-tools](http://www.bonvinlab.org/pdb-tools).
+Tools such as [Merizo](https://github.com/psipred/Merizo), [SWORD2](https://www.dsimb.inserm.fr/SWORD2) and [Chainsaw](https://github.com/JudeWells/chainsaw) can be used to predict domains from a larger structure.
+You can also slice out domains manually using software such as the `pdb_selres` command from [pdb-tools](http://www.bonvinlab.org/pdb-tools).
 
 Interpreting the hit descriptions depends on the database being searched.
 The domain name often includes a reference to the corresponding PDB file, for example d1a6ja_ refers to PDB ID 1A6J chain A, and this can be opened in the [RCSB PDB structure view](https://www.rcsb.org/3d-view/1A6J/1) to get a quick look.
+For the AlphaFold database TED domains, files can be downloaded from [links such as this](https://alphafold.ebi.ac.uk/files/AF-A0A6J8EXE6-F1-model_v4.pdb) where `AF-A0A6J8EXE6-F1` is the first part of the hit notes and is followed by the residue range of the domain.
 
 The available pre-embedded databases are:
 
-| Name      | Description                                                                                                                                                | Number of domains | Search time (1 query) | Search time (100 queries) |
-| --------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------- | --------------------- | ------------------------- |
-| `scope95` | ASTRAL set of [SCOPe](https://scop.berkeley.edu) 2.08 domains clustered at 95% seq ID                                                                      | 35,371            | 1.43 s                | 2.47 s                    |
-| `scope40` | ASTRAL set of [SCOPe](https://scop.berkeley.edu) 2.08 domains clustered at 40% seq ID                                                                      | 15,127            | 1.36 s                | 2.25 s                    |
-| `cath40`  | S40 non-redundant domains from [CATH](http://cathdb.info) 23/11/22                                                                                         | 31,884            | 1.44 s                | 2.42 s                    |
-| `ecod70`  | F70 representative domains from [ECOD](http://prodata.swmed.edu/ecod) develop287                                                                           | 71,635            | 1.48 s                | 3.36 s                    |
-| `af21org` | [AlphaFold](https://alphafold.ebi.ac.uk) structures for 21 model organisms split into domains by [CATH-Assign](https://doi.org/10.1038/s42003-023-04488-9) | 338,258           | 2.15 s                | 7.88 s                    |
+| Name      | Description                                                                                                                                                                                | Number of domains | Search time (1 query)      | Search time (100 queries)  |
+| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------- | -------------------------- | -------------------------- |
+| `scope95` | ASTRAL set of [SCOPe](https://scop.berkeley.edu) 2.08 domains clustered at 95% seq ID                                                                                                      | 35,371            | 1.35 s                     | 2.81 s                     |
+| `scope40` | ASTRAL set of [SCOPe](https://scop.berkeley.edu) 2.08 domains clustered at 40% seq ID                                                                                                      | 15,127            | 1.32 s                     | 2.36 s                     |
+| `cath40`  | S40 non-redundant domains from [CATH](http://cathdb.info) 23/11/22                                                                                                                         | 31,884            | 1.38 s                     | 2.79 s                     |
+| `ecod70`  | F70 representative domains from [ECOD](http://prodata.swmed.edu/ecod) develop287                                                                                                           | 71,635            | 1.46 s                     | 3.82 s                     |
+| `af21org` | [AlphaFold](https://alphafold.ebi.ac.uk) structures for 21 model organisms split into domains by [CATH-Assign](https://doi.org/10.1038/s42003-023-04488-9)                                 | 338,258           | 2.21 s                     | 11.0 s                     |
+| `afted`   | [AlphaFold database](https://alphafold.ebi.ac.uk) structures split into domains by [TED](https://www.biorxiv.org/content/10.1101/2024.03.18.585509) and clustered at 50% sequence identity | 53,344,209        | 67.7 s                     | 73.1 s                     |
 
 Search time is for a 150 residue protein (d1a6ja_ in PDB format) on an Intel i9-10980XE CPU with 256 GB RAM and PyTorch 1.11.
 Times are given for 1 or 100 queries.
+Note that `afted` uses exhaustive FAISS searching.
+This doesn't change the hits that are found, but the similarity score will differ by a small amount - see the paper.
 
 ## Pre-embed a dataset to search against
 
 To embed a dataset of structures, allowing it to be searched against:
 ```bash
 progres embed -l filepaths.txt -o searchdb.pt
 ```
 - `-l` is a text file with information on one structure per line, each of which will be one entry in the output. White space should separate the file path to the structure and the domain name, with optionally any additional text being treated as a note for the notes column of the results.
 - `-o` is the output file path for the PyTorch file containing a dictionary with the embeddings and associated data. It can be read in with `torch.load`.
 - `-f` determines the file format of each structure as above (`guess`, `pdb`, `mmcif`, `mmtf` or `coords`).
 
 Again, the structures should correspond to single protein domains.
+The embeddings are stored as Float16, which has no noticeable effect on search performance.
 
 ## Python library
 
 `progres` can also be used in Python, allowing it to be integrated into other methods:
 ```python
 import progres as pg
 
@@ -129,29 +137,40 @@
 graph = pg.read_graph("query.pdb")
 graph # Data(x=[150, 67], edge_index=[2, 2758], coords=[150, 3])
 
 # Embed a single structure
 embedding = pg.embed_structure("query.pdb")
 embedding.shape # torch.Size([128])
 
+# Load and reuse the model for speed
+model = pg.load_trained_model()
+embedding = pg.embed_structure("query.pdb", model=model)
+
 # Embed Cα coordinates and search with the embedding
 # This is useful for using progres in existing pipelines that give out Cα coordinates
 # queryembeddings should have shape (128) or (n, 128)
 #   and should be normalised across the 128 dimension
 coords = pg.read_coords("query.pdb")
 embedding = pg.embed_coords(coords) # Can take a list of coords or a tensor of shape (nres, 3)
 results = pg.progres_search(queryembeddings=embedding, targetdb="scope95")
 
 # Get the similarity score (0 to 1) between two embeddings
 # The distance (1 - similarity) is also available as pg.embedding_distance
 score = pg.embedding_similarity(embedding, embedding)
 score # tensor(1.) in this case since they are the same embedding
 
 # Get all-v-all similarity scores between 1000 embeddings
-embs = torch.nn.functional.normalize(torch.rand(1000, 128), dim=1)
+embs = torch.nn.functional.normalize(torch.randn(1000, 128), dim=1)
 scores = pg.embedding_similarity(embs.unsqueeze(0), embs.unsqueeze(1))
 scores.shape # torch.Size([1000, 1000])
 ```
 
+## Scripts
+
+Datasets and scripts for benchmarking (including for other methods), FAISS index generation and training are in the `scripts` directory.
+The trained model and pre-embedded databases are available on [Zenodo](https://zenodo.org/record/7782088).
+
 ## Notes
 
 The implementation of the E(n)-equivariant GNN uses [EGNN PyTorch](https://github.com/lucidrains/egnn-pytorch).
+
+Please open issues or [get in touch](http://jgreener64.github.io) with any feedback.
```

### Comparing `progres-0.2.0/setup.py` & `progres-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="progres",
-    version="0.2.0",
+    version="0.2.1",
     author="Joe G Greener",
     author_email="jgreener@mrc-lmb.cam.ac.uk",
     description="Fast protein structure searching using structure graph embeddings",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/jgreener64/progres",
+    url="https://github.com/greener-group/progres",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
```

