# Project Name: Melanoma-Detection
Melonoma Detection. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
- Provide general information about your project here.
- What is the background of your project?
    - To build a CNN based model which can accurately detect melanoma which account to 75% of skin cancer detahs. The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC) 
- What is the business probem that your project is trying to solve?
    - A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
- What is the dataset that is being used?
    - The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.
    
    The data set contains the following diseases:
        Actinic keratosis
        Basal cell carcinoma
        Dermatofibroma
        Melanoma
        Nevus
        Pigmented benign keratosis
        Seborrheic keratosis
        Squamous cell carcinoma
        Vascular lesion

## Conclusions
- Conclusion 1: Based on the training results shown in first model, it appears that model is overfitting, as the training accuracy improves steadily while the validation accuracy fluctuates and the validation loss increases over time. 
- Conclusion 2: After augmentation and droping, training accuracy is increasing and approaches ~0.5 by the end of the 20 epochs, indicating the model is learning from the training data but the validation accuracy fluctuates and does not show consistent improvement, hovering around ~0.35–0.4, and even decreases towards the end of training. Additionally, training loss steadily decreases, which means that the model is minimizing the error for the training set. The validation loss, however, fluctuates significantly and does not decrease in the same way. This indicates that the model may be struggling to generalize on the validation set.
- Conclusion 3: Evidence of Overfitting: Despite the increasing training accuracy, the validation accuracy does not improve correspondingly, and the validation loss fluctuates. This gap between training and validation performance suggests that the model is overfitting to the training data.
Improvement from Previous Model Run: While the training accuracy has improved compared to the previous run (based on assumption), the issue of overfitting remains present.
- Conclusion 4: After augmentation when images were checked it was observed that Seborrheic keratosis have least number of samples and pigmented benign keratosis has highest number of samples.
- Conclusion 5: after applying normalization techniques like augmentation, early stoping, regularization and drop-out issue of overfitting was resolved.

## Technologies Used
- TensorFlow Version: 2.16.2
- Matplotlib Version: 3.9.2
- NumPy Version: 1.26.4
- Pandas Version: 2.2.2
- Pillow (PIL) Version: 10.4.0
- Augmentor Version: 0.2.12
- Keras Version: 3.5.0

## Acknowledgements
Give credit here.
- This project was inspired by https://my.clevelandclinic.org/health/diseases/14391-melanoma

## Contact
Created by [https://github.com/rvquintiles] - feel free to contact me!
