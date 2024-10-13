# scMCGF
We present a multi-view clustering algorithm based on graph fusion (scMCGF) to cluster cells from scRNA-Seq data. scMCGF utilizes multi-view data generated from transcriptomic data to learn the consistent and complementary information of each view, and derives a unified graph matrix to obtain final cell clusters.    

See details in our paper: "Multi-view Clustering for Single-Cell RNA-seq Data Based on Graph Fusion".  
   
Quick start:  
Download the the Matlab Toolbox for Dimensionality Reduction(version 0.8b) and code files in this repository and import functions in them.  
1.Prepare datasets  and construct multi-view data
scMCGF preprocessed data and generate multi-view data with code in preprocessing.zip.  
2.Download and load the Matlab Toolbox in MATLAB. 
3.Run scMCGF algorithm 
Run the algorithm with scMCGF.m function.  




Requirements: 
Matlab---2014a
python---3.8.5 
numpy --- 1.18.5  
pandas --- 1.1.3 
h5py ---2.10.0
scanpy---1.7.1  
scikit-learn --- 1.0.1
matplotlib --- 3.3.2