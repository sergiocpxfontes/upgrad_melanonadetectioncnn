# Melanoma Detection Assignment
> This project aims to build CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Methodology](#methodology)
* [Conclusions](#conclusions)
* [Contact](#contact)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- This project is based on materials and classes under the upGrad & IIITB Global Program in Machine Learning & AI.
- With this project want to obtain a model that can help model which can accurately detect melanoma:
  - Professionals around the work analise hundreds of images trying to detect cancer. Imagine that we could create a model that could be used on mobile devices allowing each person to run basic exams to their skin signs!
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC).
  - All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.
  - You can download the dataset [here](https://drive.google.com/file/d/1xLfSQUGDl8ezNNbUkpuHOYvSpTyxVhCs/view?usp=sharing).
  - The data set contains the following diseases:
    - Actinic keratosis
    - Basal cell carcinoma
    - Dermatofibroma
    - Melanoma
    - Nevus
    - Pigmented benign keratosis
    - Seborrheic keratosis
    - Squamous cell carcinoma
    - Vascular lesion

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->
## Methodology

To create the CNN model several steps need to be made, from loading the necessary libraries and data to the creation of a sequential CNN and analisys of indicators as accuracy and loss.

The steps will be executed with a Jupyter Notebook file and will follow the order:

- Step 0 » Importing the necessary python modules and packages
- Step 1 » Reading, understanding the data
- Step 2 » Creating the dataset
- Step 3 » Visualize the patial data
- Step 4 » Creating the first model
- Step 5 » Evaluating the first model
- Step 6 » Add augmentation to enrich the dataset (only on the training set)
- Step 7 » Creating the second model
- Step 8 » Evaluating the second model
- Step 9 » Determine and handle imbalance
- Step 10 » Creating the third model
- Step 11 » Evaluating the third model

## Conclusions

The CNN that was created was sequencial CNN with 18 layers and then reduced to 17 layers since the first layer of the first model is a rescaling and on the second and third layer already apply rescaling on data generation for aumentation and imbalance handling:

 - Rescaling       
 - Conv 2d     
 - Activation (relu)
 - Conv 2d
 - Activation (relu)  
 - Max Pooling 2d
 - Dropout
 - Conv 2d
 - Activation (relu)
 - Conv 2d
 - Activation (relu)
 - Max Pooling 2d
 - Dropout
 - Flatten
 - Dense
 - Activation (relu)
 - Dropout
 - Dense
 - Activation (softmax)

Total training paramenters 60 658 729.

- The first version of the model was clearly overffiting:
  - The model works very well with training but doesn't handle correctly on new unseen data.
  - We also saw that the loss is increasing on validation data. 
  - Training accuracy is of 69% while validation accuracy is 17%.
- The second model, where augmentation was added, is less affected by overffiting but accuracy reduced to 52% and 13% respectivly
  - The overfitting its not so strong if we see that we have a moderate training loss at the beginning that will gradually decreases when adding training examples and will gradually flatten. 
- the third model, where imbalance was added, is also less affected by overffiting but accuracy reduced to 52% and 13% respectivly
  - The overfitting its not so strong if we see that we have a moderate training loss at the beginning that will gradually decreases when adding training examples and will gradually flatten. 
- Finally we can conclude that the model is not good and needs to be improved. How?
  - Testing other models with diferent number of layers.
  - Review the augmentation strategy.
  - Consider a diferent optimizer.
  - Consider reducing the number of epochs:
    - If the model is to complex.
  - Consider early stopping
  
## Technologies Used
- library - skimage
- library - numpy
- library - matplotlib
- library - tensorflow
- library - matplotlib

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Contact
Created by [@sergiocpxfontes] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
