# contrex_time_series_contrastive_learning
CONTREX is a novel contrastive representation learning approach for multivariate time series data, addressing challenges of temporal dependencies and extreme class imbalance. Our method involves extracting dynamic features from the multivariate time series instances, deriving two extremes from positive and negative class feature vectors that provide maximum separation capability, and training a sequence representation embedding module with the original multivariate time series data guided by our custom contrastive reconstruction loss to generate embeddings aligned with the extreme points. These embeddings capture essential time series characteristics and enhance discriminative power. Our approach shows promising classification results on the SWAN-SF benchmark dataset against baseline methods.

# Content Details
* <code> DATA\catch22 </code> contains data points, including extracted catch22 feature vectors and the contrastive extremes.

* <code> DATA\Preprocessed-SWANSF-main </code> contains preprocessed SWAN-SF data points, in case of training all components from scratch, the folders to keep data files must be placed under here (names and paths can be specified while running the relevant notebook cells).
  
* <code> CODE/ </code> The details for each notebook file are as follows:
  - <code>contrex_module.ipynb</code>: This module is a step-by-step guide to our experiments in a single notebook file.
    
# Execution Details 
* To view our modules, experiments, and results in a single file, contrex_module.ipynb file is sufficient.
* Since SWAN-SF is a large dataset, we do not include the preprocessed dataset in DATA\Preprocessed-SWANSF-main, if you need to train the components and start the experiments from scratch, don't hesitate to contact us!
* Original SWAN-SF data comes from: https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/EBCFKM,
we use the preprocessed version as discussed in our paper.
* All experiments are done with python 3.9.13, pytorch 2.1.0, numpy 1.25.2, pycatch22 0.4.2
