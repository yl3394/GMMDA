# GMMDA


# Overview

Here we provide the implementation of GMMDA, *GMMDA: Gaussian Mixture Modeling of Graph in Latent Space for Graph Data Augmentation*, along with a minimal execution example (on the Cora, Citeseer, Pubmed, Cora-full, Coauthor-CS and Coauthor-physics datasets). 

The six notebooks contains the implementation and experiment code of the GMMDA on all six datasets mentioned previously, and all three notebooks can be directly ran on Google colab after uploading the notebook files to your google drive folders and putting the needed datasets under the corresponding Google drive directories. For example, saving the Cora datasets under `/content/drive/MyDrive/gda_dnml/cora/data/`. 

**[Recoomend]** You can also run the following colabs without uploading notebooks to your google drive:
- [Cora colab gist](https://colab.research.google.com/gist/yl3394/27cfba9f242499583152bbca37023f85/gmmda_cora.ipynb)
- [Coauthor-CS colab gist](https://colab.research.google.com/gist/yl3394/7988b30a318daa0b966c5623efd61f44/gmmda_coauthor_cs.ipynb)
- [Coauthor-physics colab gist](https://colab.research.google.com/gist/yl3394/8dafff6454aadeb0af176ae0187efc47/gmmda_coauthor_physics.ipynb)
- [Cora-full colab gist](https://colab.research.google.com/gist/yl3394/3d4d68e95af2e7103090c4f609518278/gmmda_corafull.ipynb)
- [PubMed colab gist](https://colab.research.google.com/gist/yl3394/41bf3d2fc7ebd323ae5de3d67a480b7d/gmmda_pubmed.ipynb)

The colab code will auto-complete other folder creation process, such as `model/` directory if you want to train your own models. Otherwise, you can save the pre-tained models for directly applying our proposed data augmentation method, which will be explained in the following section, to `model/` directory. For example, saving the pre-trained model on Cora, named `GAT_aux_gmm_v2`, under `/content/drive/MyDrive/gda_dnml/cora/model/`. 

The proposed GMMDA framework includes several hyper parameters, which we have provide parameter sensitivity analysis in the paper. In summary, we have 
- $B$: budget size in proportion (1 = 100%), $B * N$ equals to the number of nodes to augment 
- $C$: number of candidates 


# Additional Notes 

Due to the large size of the preprocessed datasets and pre-trained models, we save them in a dropbox, which can be accessed via the following link: https://www.dropbox.com/sh/9sv5lahyj1g0c6z/AABI6xiTbWAEnz4BHZEHR1ZJa?dl=0

The Dropbox directory is organised as follows. Models are under the `model` folder under each dataset name based folder. Preprocessed datasets are under the `data` folder under each dataset name based folder. Under each dataset's directory, there are: 
- `data/` contains the necessary dataset files for a given datasets;
- `models/` contains the pertained of the GMMDA's for given datasets. 

We provide the pre-trained GMMDA models for all six datasets (Cora, Citeseer, Pubmed, Cora-full, Coauthor-CS and Coauthor-physics) and 3 GNN architectures (GCN, GAT, GraphSAGE). In order to run the pre-trained models, you need to download the models from the above link and save them following the same directory hierarchy as above, and then directly running the section named “**⛳️ GMMDA Data Augmentation and Downstream Node Classification**” will both return the optimal augmented graph and demonstrate the downstream node classification task performance under each setting. 




