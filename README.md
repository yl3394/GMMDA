# GMMDA


# Overview

Here we provide the implementation of GMMDA, *GMMDA: Gaussian Mixture Modeling of Graph in Latent Space for Graph Data Augmentation*, along with a minimal execution example (on the Cora, Citeseer, Pubmed, Cora-full, Coauthor-CS and Coauthor-physics dataset). 

The three notebooks contains the implementation and experiment code of the GMMDA on Cora, Citeseer and Pubmed datasets, all three notebooks can be directly ran on Google colab after putting the needed datasets under the corresponding Google drive directories. For example, saving the Cora datasets under `/content/drive/MyDrive/gda_dnml/cora/data/`. 

The colab code will auto-complete other folder creation process, such as `model/` directory if you want to train your own models. Otherwise, you can save the pre-tained models, which will be explained in the following section, to `model/` directory. For example, saving the pre-trained model on Cora, named `GAT_aux_gmm_v2`, under `/content/drive/MyDrive/gda_dnml/cora/model/`. 


# Additional Notes 

Due to the large size of the preprocessed datasets and pre-trained models, we save them in a dropbox, which can be accessed via the following link: https://www.dropbox.com/sh/9sv5lahyj1g0c6z/AABI6xiTbWAEnz4BHZEHR1ZJa?dl=0

The Dropbox directory is organised as follows. Models are under the `model` folder under each dataset name based folder. Preprocessed datasets are under the `data` folder under each each dataset name based folder. Under each dataset's directory, there are: 
- `data/` contains the necessary dataset files for a given datasets;
- `models/` contains the pertained of the GMMDA's for given datasets. 

