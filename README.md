# Multiclass-Protein-Research
## About

[https://ieeexplore.ieee.org/document/8993082](https://ieeexplore.ieee.org/document/8993049)

This paper investigates three machine learning models and a comparison was conducted using different performance measures to determine which algorithm would effectively predict protein classifications based on residue count, structure of molecular weight, and protein sequences. Decision Trees, Random Forests and Extra Trees models are applied on a structural protein sequences dataset. This dataset also contains other features for extraction methods and details on protein structures. Based on the experiments that were conducted on these models, it was demonstrated that Extra Trees model had comparable results but marginally better than the Decision Trees and Random Forests models.

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
 - Once Jupyter Notebook is running, go to Multiclass-Protein-Research Directory
 - Open Multiclass-Protein-Research.ipynb & Run 

## Accuracy Heat map & 5 Most Common Protein Heat map

<img src="/Readme/Heatmap_Accuracy.png" align="top"
width="300" hspace="10" vspace="10">
<img src="/Readme/Heatmap_DecisionTrees.png" align="top"
width="300" hspace="10" vspace="10">
<img src="/Readme/Heatmap_RandomForest.png" align="top"
width="300" hspace="10" vspace="10">
<img src="/Readme/Heatmap_ExtraTrees.png" align="top"
width="300" hspace="10" vspace="10">

## Most Common Protein Heat map

<img src="/Readme/Heatmap29_DecisionTrees.png" align="top"
width="300" hspace="10" vspace="10">
<img src="/Readme/Heatmap29_RandomForest.png" align="top"
width="300" hspace="10" vspace="10">
<img src="/Readme/Heatmap29_ExtraTrees.png" align="top"
width="300" hspace="10" vspace="10">

 
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
