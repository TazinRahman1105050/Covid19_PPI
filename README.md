# Covid19_PPI
Viruses are parasites that lack the capacity to live and reproduce outside of a host body. Protein-protein interaction (PPI) between viral proteins and host proteins is indispensable for viral proteins to reach the host cells. Consequently, identification of the virus-host PPI network is the key to predicting the behavior of viruses, which in turn can be useful in designing antiviral drugs. 

In this work, the main objective is to identify the proteins targeted by the COVID-19 virus. There are several studies that have shown proteins are correlated with the topological properties of protein-protein interaction networks, for example, hubs that are \textit{"highly connected"} in a protein-protein interaction network tend to correspond to essential proteins. Similarly, multiple centrality measures are used to discover essential proteins based on the network topological features.

Pair-wise protein interactions can be modeled as an unweighted, undirected graph, in which each node represents a protein and each edge (between two nodes) represents an interaction between two proteins. The modeling of PPI networks by simple graph structures is common in many applications, including the prediction of essential proteins within protein networks. But different edges may actually be of different levels of importance in biological networks as well as in other networks. On the other hand, gene expression data provides information about the genome under many different experimental conditions despite the large amount of inherent noise. The challenging task is to integrate the two data sources in order to treat each interaction in the PPI network in a quantitatively or qualitatively different way.
<img width="1896" height="1032" alt="flow1" src="https://github.com/user-attachments/assets/f56bb058-f689-44ec-9258-24a7e8766a27" />

We tried to find out if any centrality measure alone can identify hub and non-hub proteins. For this purpose, we first need to calculate the feature importance. One particular application of a random forest classifier is feature selection, which helps to get the relative importance of features in prediction. It uses the Gini coefficient to calculate feature importance. The Gini coefficient tells us how much the accuracy decreases if one feature is discarded. The larger the reduction of accuracy, the more important the feature is. Random  Forest classifier also generally achieves good accuracy as lots of decision trees participate in the decision-making process.

Repository Files:
There are three files in the repository

## Analyze_cytoscape_result.py conatins the codes to analyze the result from file generated from cytoscape. This file contains 6 different centrlaity measures

## Calculate_z_score.py contains the code to generate different centrality measures from python igraph and calculate z_score

## RandomForest.py contains the file for random forest classifier
