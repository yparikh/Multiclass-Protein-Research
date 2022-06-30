# Multiclass-Protein-Research
## About

[Link to the Paper](https://ieeexplore.ieee.org/document/8993049)

This paper investigates three machine learning models and a comparison was conducted using different performance measures to determine which algorithm would effectively predict protein classifications based on residue count, structure of molecular weight, and protein sequences. Based on the experiments that were conducted on these models, it was demonstrated that Extra Trees model had comparable results but marginally better than the Decision Trees and Random Forests models.

Classifiers applied on the protein sequence dataset:
* Decision Forest
* Extra Trees
* Random Forest

## Dataset

[Link to the Dataset](https://www.kaggle.com/datasets/shahir/protein-data-set)

- The dataset used in this research is the Structural Protein Sequences Dataset provided by RCSB Protein Data Bank. 
- The dataset includes 467,304 instances with 13 Features. 
- These primary features include various methods of classification, extraction details, and information on protein structures.
- Features:
  - Structure ID
  - Classification
  - Experimental Technique
  - Macromolecule Type
  - Residue Count
  - Etc.
- Restrictions had to be considered for the number of features used in classificaiton as well as the number of classes incorporated in the training due to computational and visual restraints.
  - Classes with count above 2000 were considered
  - Sequeuence, Residue Count, and Structure molecular weight were only utilizied for protein identification
  - The top 29, 10, 8, 6, and 5 highest frequency classes were presented due to the visual space 

## Dependencies
* [scikit-learn](http://scikit-learn.org/stable/)
* [numpy](http://www.numpy.org/)
* [pandas](https://pandas.pydatakeras.org/)
* [seaborn](https://seaborn.pydata.org/)
* [keras](https://keras.io/)

## Installation & Usage

 Open the terminal:
 ```
 $ cd \<required-path>
 $ git clone https://github.com/yparikh/Multiclass-Protein-Research.git
 $ jupyter notebook
 ```
 - Include the Dataset in the directory 
 - Once Jupyter Notebook is running, go to Multiclass-Protein-Research Directory
 - Open Multiclass-Protein-Research.ipynb & Run 

## Labels
- The labels on each of the graphs represent the classification of the protein. 
- Various proteins will share similar sequences or structural properties, thus  allowing proteins to be classified into groups. 
- These groups with well defined characteristics can help with proposing functional properties when a novel protein is identitified. 
- In the top 5 most common classifications, classes such as Hydrolase and Transferase will be seen often since these are large classes of enyzmes. 
- Hydrolase will be seen the most since it is the largest class of enzymes with more than 200 enyzmes. 


## Accuracy Heat map & 5 Most Common Protein Confusion Matrices 
- From the [confusion matricies](https://en.wikipedia.org/wiki/Confusion_matrix), we were able to display the summarize and display the performance for each of the models used to train and test the dataset. 
- The Accuracy Heat Map demonstrates the accuracy for the different number of classes tested against the models. 
- The accuracy was derived from the precision, recall, and f1-scores for each of the machine learning classifiers. 


Heatmap & Confusion Matricies  | Image
------------- | -------------
Accuracy Among Various Class Sizes (The top 5 are accuracies for the Decision Trees, The middle 5 are accuracies for Random Forest, and the Bottom 5 are accuracies for the Extra Trees. Each Classifier gradually improved accuracy when the number of classes to test against was reduced.)| ![](/Readme/Heatmap_Accuracy.png)
Decision Trees of Top 5 Classes | ![](/Readme/Heatmap_DecisionTrees.png)
Random Forest of Top 5 Classes | ![](/Readme/Heatmap_RandomForest.png)
Extra Trees of Top 5 Classes | ![](/Readme/Heatmap_ExtraTrees.png)

## Top 29 Most Common Protein Confusion Matrices


Heatmap  | Image
------------- | -------------
Decision Trees of Top 29 Classes | ![](/Readme/Heatmap29_DecisionTrees.png)
Random Forest of Top 29 Classes | ![](/Readme/Heatmap29_RandomForest.png)
Extra Trees of Top 29 Classes | ![](/Readme/Heatmap29_ExtraTrees.png)

# Citation
If you use this software in academic research, please, cite it using the following BibTeX:
```latex
@misc{YashParikh2019,
author = {Yash Parikh, Eman Abdelfattah},
title = {Comparison of Machine Learning Models to Predict Twitter Buzz},
year = {2019},
publisher = {IEEE},
journal = {2019 IEEE 10th Annual Ubiquitous Computing, Electronics & Mobile Communication Conference (UEMCON)},
howpublished = {\url{https://ieeexplore.ieee.org/document/8993082}},
}
```
