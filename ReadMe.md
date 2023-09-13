# Support-Vector-Machine-for-Arabic-Handwritten-Character-Recognition-using-DOST-PCA-Features



## Table of Contents
- [Dataset](#dataset)
- [Introduction](#introduction)
- [Methodology](#Methodology)
- [Sample Visualization](#sample-visualization)
- [Results](#Results)
- [Credits](#credits)




### Dataset

[Preprocessed Data](https://www.kaggle.com/datasets/mloey1/ahcd1) <br>

## Introduction

- Arabic is one of the oldest and most influential languages globally, with a rich and diverse script.
- This research paper presents a novel model for Optical Character Recognition focused on Handwritten Arabic characters.
- The proposed model employs a hybrid Discrete Orthonormal Stockwell Transform combined with a Principal Component Analysis feature extraction technique, which captures important information in the form of Discrete coefficients from each 
individual character’s intensity.
- The extracted features are then sent for dimensionality reduction to form feature vectors. These feature vectors are then condensed into a single vector and fed into the Support Vector Machine classifier for accurate classification.



## Objectives

- The distinct variations among its 28 letters and additional diacritical marks require a careful analysis of the intricate contours and shapes of each character for accurate identification. 
- The presence of ligatures, cursive writing styles, and contextual shaping further contribute to the complexity of Arabic handwritten character recognition. 
- Therefore, developing effective algorithms and models that can accurately capture the nuanced characteristics of Arabic handwritten characters remains an ongoing research area with immense potential for applications in digitizing Arabic
texts and enabling efficient text analysis.

## Methodology

- The proposed model for Arabic Handwritten Characters in optical character recognition encompasses three main stages: pre-processing, feature extraction, and model fitting.
- The pre-processing stage primarily focuses on cleaning the characters through the application of morphological functions, employing a series of sequential steps on each image.
- The feature extraction stage involves the identification of pixel intensities, texture information, and shape descriptors for each character image, followed by the utilization of the Principal Component Analysis (PCA) to decrease their dimensionality.
- Finally, the Support Vector Machine classifier model is utilized to achieve precise recognition of each character and allocate it to its appropriate class within the dataset.


High-level overview of the process: <br>
![High level overview](https://github.com/calicartels/Support-Vector-Machine-for-Arabic-Handwritten-Character-Recognition-using-DOST-PCA-Features/blob/main/HIGH%20LEVEL%20OVERVIEW.png) <br>


## Sample Visualization

Visualization of the DOST points plotted on the image: <br>
![Feature extraction in Live time](https://github.com/calicartels/Support-Vector-Machine-for-Arabic-Handwritten-Character-Recognition-using-DOST-PCA-Features/blob/main/DOST%20feature%20point.png) <br>

Sample Visualization of the images after going through dimensionality reduction: <br>

![First 3 dimensions being represented](https://github.com/calicartels/Support-Vector-Machine-for-Arabic-Handwritten-Character-Recognition-using-DOST-PCA-Features/blob/main/Sample%203d%20viz%20for%20the%20first%203%20dimensions%20.png)





## Results

- The proposed DOST feature extraction coupled with the SVM model shows improved performance with respect to the other models by achieving an accuracy of 87.44%.
- The possible reasons attributed to the reduction in accuracy are postulated through a variety of factors.
- The analysis reveals that there are certain challenges in accurately recognizing pairs of classes, which include, but are not limited to classes 10 and 9, as well as classes 5 and 11.
- This difficulty arises due to the similarity in shape between these pairs.


![Similarity in pair 1](https://github.com/calicartels/Support-Vector-Machine-for-Arabic-Handwritten-Character-Recognition-using-DOST-PCA-Features/blob/main/Example%20Similarity%20in%20shape.png) <br>

![Similarity in pair 2](https://github.com/calicartels/Support-Vector-Machine-for-Arabic-Handwritten-Character-Recognition-using-DOST-PCA-Features/blob/main/Example%20Similarity%20in%20shape%202.png) <br>

![Confusion Matrix](https://github.com/calicartels/Support-Vector-Machine-for-Arabic-Handwritten-Character-Recognition-using-DOST-PCA-Features/blob/main/Confusion%20Matrix.png) <br>

![ROC curve for all the classes](https://github.com/calicartels/Support-Vector-Machine-for-Arabic-Handwritten-Character-Recognition-using-DOST-PCA-Features/blob/main/ROC%20curve.png) <br>

NOTE: THIS CODE DOES NOT CONTAIN THE HYPERPARAMETER-OPTIMIZED RESULT SINCE THE TUNING REQUIRED WAS COMPUTATIONALLY INTENSIVE, IT HAD TO BE DONE THROUGH A CLOUD-BASED SYSTEM.

## Credits 

- TM Vishnu Mukundan 
- Ghada Eladeb

