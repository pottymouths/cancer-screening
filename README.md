# Smart Screening: Predicting Cancer Risk from Stool with Machine Learning

Team Potty Mouths presents Smart Screening: Predicting Cancer Risk from Stool with Machine Learning, a project for BDA 602: Machine Learning Engineering, a course part of the M.S. program in Big Data Analytics at SDSU.

This GitHub repository contains the code used in this study, data samples for the model training, as well as notebook outputs highlighting results.

## Abstract

Colorectal cancer (CRC) represents the second most common cause of non-gender-related cancer deaths, and accounted for nearly 12% of all cancer treatment costs in the United States in
2020. This risk (and treatment cost) significantly decreases with early intervention strategies like
screening. Advancements in CRC detection screenings have been made, but are often expensive,
invasive, and underutilized. This study explores a possible screening method via a robust and
generalizable machine learning classification model. Data from INRAE consisting of 2,340 gut microbiome profiles (consisting of bacterial species classified as gut and/or oral) of healthy patients
and patients with CRC or colorectal adenomas (CRA) was analyzed, visualized, and used to train
several ensemble machine learning classification models: bagged logistic regression, random forests,
bagged multilayer perceptrons, and bagged extreme learning machines. Of these 2,340 samples,
202 were identified by INRAE as contaminated and excluded from the exploratory analysis and
model training. Linear discriminant analysis revealed distinct clusters for healthy (n = 1056),
CRC (n = 897), and CRA (n = 185) groups based on both gut and total metagenomic species
pangenomes (MSPs). As such, a total of 8 models were trained: 4 were trained on only gut MSPs,
with the remaining 4 trained on all MSPs in the data. Every model pipeline aside from the random
forest models included a standard scaler and PCA as the data preprocessing steps. The multilayer
perceptron and logistic regression ensemble models trained on all MSPs outperformed the others,
with ROC-AUC of 0.81 and 0.80 respectively upon final evaluation with the test set. Upon final
evaluation, the bagged multilayer perceptron model was found to be the best performing; deep
learning ensemble models show great promise for use in CRC detection.

