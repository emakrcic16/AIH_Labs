# Lab 1
The lab consisted of classifying neurodegenerative disorders such as Alzheimer’s disease, mild cognitive impairment and cognitively normal. This by constructing a Convolutional Neural Network (CNN) where PET-scans of humans brains where used.
The PET-scans consisted totally of 468 images where each neurodedegenerate disorder had 156 images (156 Alzheimer’s disease, 156 mild cognitive impairment, 156 cognitively normal). 
79x95x79 were the dimensions of each scan. The images were fed to the CNN was of size 79x95x60, where the first 10 and last 9 where discarded in the third dimension. 
K-fold cross validation was performed on 90% of the data. Meaning the test set was 10% of the data. Model fine tuning was performed in attempts in approving the model. For evaluating the model, a confusion  matrix, specificity, sensitivity and ROC curve was used.

# The Model
The constructed model is shown in the figure below. Where the model contained of two 3D convolutional blocks. The first convolutional layer (conv1_1) has 8 filters and the second layer(conv1_2) has 16 filters. The convolutional blocks was of size 3x3x3. Followed by 3D max pooling layer with size of 3x3x3 and batch normalization. This was then fed into two layers of 3D convolutional blocks with 32 respectively 64 filters to be later fed in an additional layer of 3D max pooling. This was later flattened before moving on to two connected layers followed by dropout. The first layer in the connected layer had 4096 hidden nodes, and the second layer had 1024 hidden nodes. At last fed to the output layer with activation function SoftMax.
![The implemented model](AIH_Labs/Lab1/Result/TheModel.png)
