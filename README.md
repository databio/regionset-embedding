# regionset-embedding

Regionset-embedding build representation for large genomic data.This code includes the functions to build representations and evaluate that through  the classification of the biological information and finding similairty between bed files on a simulated dataset. 

# Dataset:

The data is available at: http://big.databio.org/papers/region_embedding/

Building representations:

representations_regionset2vec: this file contains functions to shuffle the samples in the training set and training word2vec models. 
  
representation_tf_idf: this file contains functions to generate tf_idf representation. 
  
 
# Classification Task:

classification_performance: this file contains functions to read files, train a classifier on the training data and report the performance on the test dataset. The results are saved as the CSV file in the results folder.
  
# Visulization:

umap_plots_simialritydetection: this file contains functions to plot simulated dataset with different representations, the plots are saved in the umap_plots_simialritydetection folder.
  
umap_plots_classification: this file contains functions to plot antibody, cell line and tissue datasets with different representations, the plots are saved in the umap_plots_classification folder.

# Folders:

meta_data: this folder contains the metadata information for each dataset (antibody, cell line, tissue).
  
representations: different universes created by the union and tf_idf approaches are saved in this folder (antibody, cell line, tissue).
  
region_embedding_models: the trained word2vec models, output of the representation_regionset2vec are saved in this folder. 

results: the performance of the classifiers is saved in this folder as the 

# Functions:

functions_ailist: this file contains the function to run ailist.
  
functions_readbedfiles: this file contains functions for reading bedfiles, convert the binary representation to text document format, reading and writing JSON files. 
  
functions_plot: this file contains functions to reprocess the data, reduce dimensions and plot using umap technique. 
  