# scMCGF
We present a multi-view clustering algorithm based on graph fusion (scMCGF) to cluster cells from scRNA-Seq data. scMCGF utilizes multi-view data generated from transcriptomic data to learn the consistent and complementary information of each view, and derives a unified graph matrix to obtain final cell clusters. Experiments results of thirteen real datasets reveal that scMCGF outperforms eight state-of-the-art methods in clustering accuracy and robustness. Furthermore, biological analysis validates that the clustering results of scMCGF provide an accurate basis for downstream analysis.  

See details in our paper: "Multi-view Clustering for Single-Cell RNA-seq Data Based on Graph Fusion".  
   
Quick start:  
Download the the Matlab Toolbox for Dimensionality Reduction(version 0.8b) and code files in this repository and import functions in them.  
1.Prepare datasets  and construct multi-view data
scMCGF preprocessed data and generate multi-view data with code in preprocessing.zip.  
2.Download and load the Matlab Toolbox in MATLAB. 
3.Run scMCGF algorithm 
Run the algorithm with scMCGF.m function.  

Parameter setting:
1.For all algorithm expect Seurat, the number of cell clusters of each data sets is determined according to its ground truth. For Seurat, we adjust the number of cell clusters by the parameter resolution.
2.For data sets with less than 3000 cells,the number of the neighbor nodes k is limited to the range [2-10], while for data sets with more than 3000 cells, k is restricted to the range [11-20]. 


Requirements: 
Matlab---2014a
python---3.8.5 
numpy --- 1.18.5  
pandas --- 1.1.3 
h5py ---2.10.0
scanpy---1.7.1  
scikit-learn --- 1.0.1
matplotlib --- 3.3.2
