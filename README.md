# MPI-VGAE: protein-metabolite enzymatic reaction link learning by variational graph autoencoders
[workflow](https://github.com/mmetalab/mpi-vgae/blob/master/figures/Figure1.tiff)
## Background
Enzymatic reactions are crucial to explore the mechanistic function of metabolites and proteins in cellular processes and to understand the etiology of diseases. The increasing number of interconnected metabolic reactions allows the development of in silico deep learning-based methods to discover new enzymatic reaction links between metabolites and proteins to further expand the landscape of existing metabolite-protein interactome. Computational approaches to predict the enzymatic reaction link by metabolite-protein interaction (MPI) prediction are still very limited. In this study, we developed a Variational Graph Autoencoders (VGAE) based framework to predict MPI in genome-scale heterogeneous enzymatic reaction networks across ten organisms. By incorporating molecular features of metabolites and proteins as well as neighboring information in the MPI networks, our MPI-VAGE predictor achieved the best predictive performance compared to other machine learning methods. Moreover, when applying the MPI-VGAE framework to reconstruct hundreds of metabolic pathways, functional enzymatic reaction networks, and a metabolite-metabolite interaction network, our method showed the most robust performance among all scenarios. To the best of our knowledge, this is the first MPI predictor by VGAE for enzymatic reaction link prediction. Furthermore, we implemented the MPI-VGAE framework to reconstruct the disease-specific MPI network based on the disrupted metabolites and proteins in Alzheimer’s disease and colorectal cancer, respectively. A substantial number of novel enzymatic reaction links were identified. We further validated and explored the interactions of these enzymatic reactions using molecular docking. These results highlight the potential of the MPI-VGAE framework for the discovery of novel disease-related enzymatic reactions and facilitate the study of the disrupted metabolisms in diseases. 
## Requirements
We run the following code on Python3.7 or above with the packages listed below. <br>
pip install networkx torch pickle tensorflow
## Source code for web application is here
https://github.com/mmetalab/mpi-vgae-web
Click [here](https://mpi-vgae-web.streamlit.app/) to try
## How to use MPI-VGAE
Here we list the process of computational pipeline to predict genome-scale enzymatic reaction via metabolite-protein interaction prediction. There are there jupyter notebooks in the notebook folder. 
The features of MPI network for each organism is deposited in folder “features”. <br>
The code for VGAE code is deposited in folder “vgae”.<br>
For prediction of metabolite-protein interaction, simply run mpi_vgae_run.ipynb, and follow the instructions on the jupyter notebook.<br>
For prediction of metabolite-protein interaction by GraphSAGE model, simply run mpi_vgae_graphsage.ipynb, and follow the instructions on the jupyter notebook.<br>
For prediction of metabolite-metabolite interaction, simply run mpi_vgae_kegg.ipynb, and follow the instructions on the jupyter notebook. 

## Contribution
The original source code was developed by Wang, Cheng et al.
