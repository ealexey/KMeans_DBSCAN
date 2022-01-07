# KMeans_DBSCAN

Application KMeans and DBSCAN to cluster cancer cell lines based on gene expression signature.

The goal of this project is to classify (cluster) tumor cell based on the gene expression profiling.

Dataset

 In the current project, a data set from the US Irvine Machine Learning Repository will be analyzed. That data set contains 881 samples. Each sample derived from one out of 
 five cancer type-PRAD, LUAD, BRCA, KIRS, and COAD. Each sample contains data for expression of 20,551 genes. Thus, the dataframe contains 881 samples and 20,551 columns
 (features). 
 
Methods

1.	Principle component analysis (PCA) will be used to reduce dimensionality of the data set. Using PCA is important because analyzed dataset has more than 20 thousand features. 
But the major disadvantage of PCA is that the PCA components are hardly interpretable. 

2.	K-means. The elbow method was used to determine the optimal numbers of k. If the optimal number of k will be difficult to determine using the elbow point method. 
The silhouette coefficient and the adjusted rand index (ARI) were used to measure the similarity between true and predicted classes using known true classes.

3.	Density-based Spatial Clustering of Application with Noise (DBSCAN). The elbow method will be used to determine the optimal eps and min_samples values. 
The silhouette coefficient and the adjusted rand index (ARI) were used to measure the similarity between true and predicted classes using known true classes.
 
Conclusion

K-means and DBSCAN algorithms were used to separate analyzed cancer cell lines into clusters based on gene expression signature. The k-means algorithm showed a 
better performance (silhouette_score=0.512, adjusted_rand_index=0.722) in comparison with the DBSCAN algorithm (silhouette_score=0.379, adjusted_rand_index=0.523).
It proves that cancer cell lines can be separated based on the gene signature expression.



