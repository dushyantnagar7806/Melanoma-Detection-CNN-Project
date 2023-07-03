
# Melanoma-Detection-Deep Leaning-Project

build a CNN-based model that detects melanoma. A data set will be provided, which contains images of malignant and benign tumours. Understand the problem statement carefully and go through the evaluation rubrics before solving the problem

## Problem Statement :
build a multiclass classification model using a custom convolutional neural network in TensorFlow.

 

Problem statement: Build a CNN-based model that can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma can potentially reduce a lot of manual effort needed in diagnosis.




## Documentation

You can download the data set from
[Here]( https://drive.google.com/file/d/1xLfSQUGDl8ezNNbUkpuHOYvSpTyxVhCs/view?usp=sharing)

The data set consists of 2,357 images of malignant and benign tumours, which were identified by the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification by ISIC, and all subsets were divided into the same number of images, except for melanomas and moles, whose images are slightly dominant.


The data set contains images relating to the following diseases:

- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

## Project Pipeline

Following are all the steps to consider while working on the data set and subsequently the model:

- **Data reading/data understanding:** Define the path for training and testing images.
- **Data set creation:** Create, train and validate the data set from the train directory with a batch size of 32. Also, make sure you resize your images to 180*180.
- **Data set visualisation:** Create code to visualise one instance of all the nine classes present in the data set.
- **Model building and training:** Create a model and report the findings. You can follow the below-mentioned steps:
  - Create a CNN model that can accurately detect nine classes present in the data set. While building the model, rescale images to normalise pixel values between (0,1).
   - Choose an appropriate optimiser and a loss function for model training.
  - Train the model for ~20 epochs.
  - Write your findings after the model fit. You must check if - there is any evidence of model overfit or underfit.
- **Resolving underfitting/overfitting issues:** Choose an appropriate data augmentation strategy to resolve model underfitting/overfitting.
- **Model building and training on the augmented data:** Follow the below-mentioned steps for building and training the model on augmented data:
  - Create a CNN model that can accurately detect nine classes present in the data set. While building the model, rescale images to normalise pixel values between (0,1).
  - Choose an appropriate optimiser and a loss function for model training.
   - Train the model for ~20 epochs.
  - Write your findings after the model fit, and check whether the earlier issue is resolved.
- **Class distribution:** Examine the current class distribution in the training data set and explain the following:
  - Which class has the least number of samples?
  - Which classes dominate the data in terms of the proportionate number of samples?
- **Handling class imbalances:** Rectify class imbalances present in the training data set with the augmentor library.
- **Model building and training on the rectified class imbalance data:** Follow the below-mentioned steps for building and training the model on the rectified class imbalance data:
   - Create a CNN model that can accurately detect nine classes present in the data set. While building the model, rescale images to normalise pixel values between (0,1).
  - Choose an appropriate optimiser and a loss function for model training.
  -  Train the model for ~30 epochs.
  - Write your findings after the model fit, and check if the issues are resolved or not.
