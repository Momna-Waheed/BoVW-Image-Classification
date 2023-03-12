# BoVW-Image-Classification

End to end implementation of Bag of Visual Words based image classification network

The model is build on Google Collab with Pytorch


<!--ts-->
Contents
<!--te-->

<!--ts-->
* [Heading 1](## Introduction)
* [Heading 3](#heading-3)
* [Heading 3](#heading-3)
<!--te-->

## Introduction
The Bag of Visual Words (BoVW) is a method for representing images in computer vision and image processing. It is based on the concept of Bag of Words (BoW) model used in natural language processing.

The BoVW model is used to represent an image as a collection of visual words, which are obtained by clustering similar image patches together. These visual words are then used to generate a histogram that represents the distribution of these words in the image. The histogram can then be used as a feature vector to represent the image for various applications such as image classification, object recognition, and image retrieval.

This project aimed to demonstrate the use of BoVW for image classification using two data sets including Objects and Flowers data. The feature detector chosen for that matter was SIFT and image descriptors and key points were extracted using it. The descriptors were then used to develop the vocabulary for BoVW using K-means clustering technique. In order to determine the optimal cluster size elbow method was used and the  values in the surrounding window of k value given by it was tested and the value with the best results was chosen. After vocabulary construction the histogram analysis was performed on all the training and testing images to extract the frequency of each visual word in the image. Lastly, based on the histogram, classification was applied on the dataset by splitting it into test and train data and the classification results were analyzed for performance measures like  F1 score, accuracy, True Positive Rate, False Positive Rates etc. for two classifiers i.e. Support Vector Machines (SVM) and Random Forest.



