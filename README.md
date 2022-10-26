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

Before creating the model its necessary to load the dataset using Keras to create the training and validation datasets. 
Creating the model will require the usage of machine learning (more details on https://en.wikipedia.org/wiki/Machine_learning) and to do so, several steps  need to be made to ensure we understand the data and making sure the dataset is ready to be submited to the algorithms. The steps will be executed with a Jupyter Notebook file and will follow the following order:

The model is based on a sequential CNN

- Step 0 » Importing the necessary python modules and packages
- Step 1 » Reading, understanding the data
- Step 2 » Creating the dataset
- Step 3 » Visualize the patial data
- Step 4 » Creating the first model
- Step 5 » Predictions and evaluations on the test set

## Conclusions
- Conclusion 1 from the analysis
- Conclusion 2 from the analysis
- Conclusion 3 from the analysis
- Conclusion 4 from the analysis

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


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
