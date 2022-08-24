Dimension reduction
=========================================================
Cited from https://kzhang.org/SnapATAC2/algorithms/dimension_reduction.html#spectral-embedding

[Fang_2021]: Fang, R., Preissl, S., Li, Y. et al. Comprehensive analysis of single cell ATAC-seq data with SnapATAC. Nat Commun 12, 1337 (2021). https://doi.org/10.1038/s41467-021-21583-9

The dimension reduction method is a pairwise-similarity based method, which requires defining and computing
similarity between each pair of cells in the data.
This method was first proposed in [Fang_2021], the version 1 of SnapATAC, and was called "diffusion map".

Spectral embedding
------------------

1. Start with NxP cell by feature count matrix M, we first compute the NxN pairwise similarity matrix S.

2. Compute the normalized graph Laplacian

3. The eigenvectors correspond to the k+1-smallest eigenvalues of L are selected as the lower dimensional embedding.



Cell-type Assignment
=====================

K-Nearest Neighorbors
---------------------
KNN is a supervised machine learning algorithm that relies on labeled input data to learn a function that produces an appropriate output when given new unlabeled data.
