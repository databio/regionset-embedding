# Regionset-embedding

Regionset-embedding builds representation for large genomic data. This code includes the functions to build representations and evaluate that through the classification of the biological information and finding similarity between bed files on a simulated dataset. 

## Dataset:

The data is available at : http://big.databio.org/papers/region_embedding/

## Building representations:

[representations_regionset2vec](https://github.com/databio/regionset-embedding/blob/main/representations_regionset2vec.ipynb): this file contains functions to shuffle the samples in the training set and training word2vec models. 
  
[representation_tf_idf](https://github.com/databio/regionset-embedding/blob/main/representations_tf_idf.ipynb): this file contains functions to generate tf_idf representation. 
  
 
## Classification Task:

[classification_performance](https://github.com/databio/regionset-embedding/blob/main/src/classification_performance.ipynb): this file contains functions to read files, train a classifier on the training data and report the performance on the test dataset. The results are saved as the CSV file in the results folder.
  
## UMAP-plots:

[umap_plots_simialritydetection](https://github.com/databio/regionset-embedding/tree/main/umap_plots_similaritydetection): this file contains functions to plot simulated dataset with different representations, the plots are saved in the umap_plots_simialritydetection folder.
  
[umap_plots_classification](https://github.com/databio/regionset-embedding/tree/main/umap_plots_classification): this file contains functions to plot antibody, cell line and tissue datasets with different representations, the plots are saved in the umap_plots_classification folder.

[peak_calling_analysis](https://github.com/databio/regionset-embedding/tree/main/peak_calling_analysis): this file contains functions to analysis the effect of peak calling thresholds on classification performance and similarity detection of different representations.

## Outputs & Metadata folders:

[meta_data](https://github.com/databio/regionset-embedding/tree/main/meta_data): this folder contains the metadata information for each dataset (antibody, cell line, tissue).
  
[representations](https://github.com/databio/regionset-embedding/tree/main/representations): different universes created by the union and tf_idf approaches are saved in this folder (antibody, cell line, tissue).
  
[region_embedding_models](https://github.com/databio/regionset-embedding/tree/main/word2vecmodels): the trained word2vec models, output of the representation_regionset2vec are saved in this folder. 

[results](https://github.com/databio/regionset-embedding/tree/main/results): the performance of the classifiers is saved in this folder as the 

## Functions:

[functions_ailist](https://github.com/databio/regionset-embedding/blob/main/functions_ailist.ipynb): this file contains the function to run ailist.
  
[functions_readbedfiles](https://github.com/databio/regionset-embedding/blob/main/functions_readbedfiles.ipynb): this file contains functions for reading bedfiles, convert the binary representation to text document format, reading and writing JSON files. 
  
[functions_plot](https://github.com/databio/regionset-embedding/blob/main/functions_plot.ipynb): this file contains functions to reprocess the data, reduce dimensions and plot using umap technique. 
  
