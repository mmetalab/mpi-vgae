# Genome-scale enzymatic reaction prediction by variational graph autoencoders
![workflow](https://github.com/mmetalab/mpi-vgae/blob/master/figures/Figure1.tiff)
## Background
Enzymatic reaction networks are crucial to explore the mechanistic function of metabolites and proteins in biological systems and understanding the etiology of diseases and potential target for drug discovery. The increasing number of metabolic reactions allows the devel-opment of deep learning-based methods to discover new enzymatic reactions, which will expand the landscape of existing enzymatic reaction networks to investigate the disrupted metabolisms in diseases. 
## Results
In this study, we propose the MPI-VGAE framework to predict metabolite-protein interac-tions (MPI) in a genome-scale heterogeneous enzymatic reaction network across ten organ-isms with thousands of enzymatic reactions. We improved the Variational Graph Autoen-coders (VGAE) model to incorporate both molecular features of metabolites and proteins as well as neighboring features to achieve the best predictive performance of MPI. The MPI-VGAE framework showed robust performance in the reconstruction of hundreds of meta-bolic pathways and five functional enzymatic reaction networks. The MPI-VGAE frame-work was also applied to a homogenous metabolic reaction network and achieved as high performance as other state-of-art methods. Furthermore, the MPI-VGAE framework was to reconstruct the disease-specific MPI network based on hundreds of disrupted metabo-lites and proteins in Alzheimer’s disease and colorectal cancer, respectively. A substantial number of new potential enzymatic reactions were predicted and validated. These results highlight the potential of the MPI-VGAE framework for the discovery of novel disease-related enzymatic reactions and drug targets in real-world applications. 
## Requirements
We run the following code on Python3.7 or above with the packages listed below. <br>
pip install networkx torch pickle tensorflow
## How to use MPI-VGAE
Here we list the process of computational pipeline to predict genome-scale enzymatic reaction via metabolite-protein interaction prediction. There are there jupyter notebooks in the notebook folder. 
The features of MPI network for each organism is deposited in folder “features”. <br>
The code for VGAE code is deposited in folder “vgae”.<br>
For prediction of metabolite-protein interaction, simply run mpi_vgae_run.ipynb, and follow the instructions on the jupyter notebook.<br>
For prediction of metabolite-protein interaction by GraphSAGE model, simply run mpi_vgae_graphsage.ipynb, and follow the instructions on the jupyter notebook.<br>
For prediction of metabolite-metabolite interaction, simply run mpi_vgae_kegg.ipynb, and follow the instructions on the jupyter notebook. 

## Contribution
The original source code was developed by Wang, Cheng et al.
