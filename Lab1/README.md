# Lab 1
The lab consisted of classifying neurodegenerative disorders such as Alzheimer’s disease, mild cognitive impairment and cognitively normal. This by constructing a Convolutional Neural Network (CNN) where PET-scans of humans brains where used.
The PET-scans consisted totally of 468 images where each neurodedegenerate disorder had 156 images (156 Alzheimer’s disease, 156 mild cognitive impairment, 156 cognitively normal). 
79x95x79 were the dimensions of each scan. The images were fed to the CNN was of size 79x95x60, where the first 10 and last 9 where discarded in the third dimension. 
K-fold cross validation was performed on 90% of the data. Meaning the test set was 10% of the data. Model fine tuning was performed in attempts in approving the model. For evaluating the model, a confusion  matrix, specificity, sensitivity and ROC curve was used.
