# scrna-bacteria-integration
Batch correction and downstream analysis of prokaryotic scRNA datasets published by Kuchina et al. (2021) and Blattman et al. (2020). 
Report of results are accessible at: 
> https://docs.google.com/document/d/e/2PACX-1vSAcFnn0xipBVw7GKYQ0r9tojX6tFL2kz-HwIgsyxT-G9MsTrxH0BpqNR63gDCQO0-_sesVTKxiOm3M/pub

## Notebooks
### ecoli_preprocessing_integration_scVI_mnn.ipynb
Preprocessing and replication of Kuchina et al. (2021) results on E.coli data, batch correction using MNN Correct and scVI, clustering visualizations, differential gene expression analysis, manual exploration of clusters and marker genes, and Wishbone trajectory inference of imputed count matrix. 

### bsub_integration_mnn_harmony_combat.ipynb
Preprocessing and replication of Kuchina et al. (2021) results on B.sub data, batch correction using comBat, Harmony and MNN Correct, and visualizations. 
Blattman_Ecoli_ Data_Preprocessing.ipynb: 
Blattman et al. (2021) E. coli dataset preprocessing, principal component analysis, and 2D embeddings to confirm original results and validate presence of exponential and stationary growth stages.

### Blattman_Ecoli_ Data_Preprocessing.ipynb
Blattman et al. (2021) E. coli dataset preprocessing, principal component analysis, and 2D embeddings to confirm original results and validate presence of exponential and stationary growth stages.

### Blattman_Ecoli_Trajectory_Inference_and_DEG.ipynb
Trajectory inference using Wishbone and differentially expressed gene analysis for the Blattman E. coli dataset following preprocessing and clustering. 
Scanorama_Batch_Correction.ipynb:
Batch integration of Blattman and Kuchina datasets using Scanorama including dataset preparation, integration, DEG analysis, trajectory inference, clustering, and 2D embeddings.

### Scanorama_Batch_Correction.ipynb
Batch integration of Blattman and Kuchina datasets using Scanorama including dataset preparation, integration, DEG analysis, trajectory inference, clustering, and 2D embeddings.


## How to run
Run using Jupyter Notebook or Google Colab (preferred). Each notebook is independent and does not need to be run in any specific order. For scVI, GPU usage is recommended. All datasets must be uncompressed and kept within original paths for appropriate reference. 

## System requirements and dependencies

```
Package                     Version
----------------     ---------------------
anndata                       0.8.0
debugpy                       1.0.0
h5py                          3.1.0
igraph                        0.9.10
imageio                       2.4.1
matplotlib                    3.5.1
mnnpy                         0.1.9.5
MulticoreTSNE                 0.1
numba                         0.51.2
numpy                         1.21.6
oauthlib                      3.2.0
palantir                      1.0.0
pandas                        1.3.5
PhenoGraph                    1.5.7
scanorama                     1.7.2
scanpy                        1.8.2
scipy                         1.7.3
scprep                        1.1.0
scvi-colab                    0.10.0
scvi-tools                    0.16.1
seaborn                       0.11.2
setuptools                    59.5.0
sklearn                       0.0
sklearn-pandas                1.8.0
tensorflow                    2.8.0
umap-learn                    0.5.3
wishbone-dev                  0.5.2
```

## Datasets
**Blattman SB, Jiang W, Oikonomou P, Tavazoie S. Prokaryotic single-cell RNA sequencing by in situ combinatorial indexing. Nat Microbiol 2020 Oct;5(10):1192-1201.**
Gene Expression Omnibus (GEO) under accession number GSE141018.

**Kuchina A, Brettner LM, Paleologu L, Roco CM, Rosenberg AB, Carignano A, Kibler R, Hirano M, DePaolo RW, Seelig G. Microbial single-cell RNA sequencing by split-pool barcoding. Science. 2021 Feb 19;371(6531)**
Gene Expression Omnibus (GEO) under accession number GSE151940.
