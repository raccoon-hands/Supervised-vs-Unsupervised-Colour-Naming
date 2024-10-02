# Supervised-vs-Unsupervised-Colour-Naming
This study aims to compare and evaluate the performance of supervised and unsupervised machine learning models when trained on qualitative crowd-sourced colour naming data for uniformly sampled points in CIELUV colour space. 

As a secondary aim, the effects of synthetic oversampling and Gaussian noise injection on the generalisation ability of these models will be examined. Three supervised machine learning models (K-NN, Neural Network, and Random Forest) and two unsupervised models (Fuzzy C-Means, Self Organising Map) were set a series of colour classification tasks, and their generalisation ability tested on outside colour sample data. 

The three supervised models significantly outperformed the unsupervised learners at regression and classification, with the Neural Network reducing the 
Hellinger distance from a baseline of 0.81 to 0.26 and achieving a macro averaged F1 score of 0.65 in leave-one-out cross-validation testing. Before data augmentation, the models struggled to correctly classify any outside data. After synthetic minority oversampling with SMOTE and Gaussian noise injection, the classification performance of the supervised models dramatically increased. They excelled at classifying colour samples from images and an outside colour sample dataset with the highest F1 score rising to 0.81 and highest accuracy being 86%. 

