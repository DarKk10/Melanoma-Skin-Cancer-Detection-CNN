# Melanoma-Skin-Cancer-Detection-CNN
> To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- The dataset comprises 2357 images depicting malignant and benign oncological conditions, sourced from the International Skin Imaging Collaboration (ISIC). These images were categorized based on the classification provided by ISIC, with each subset containing an equal number of images.

- In order to address the challenge of class imbalance, the Augmentor Python package (https://augmentor.readthedocs.io/en/master/) was employed to augment the dataset. This involved generating additional samples for all classes, ensuring that none of the classes had insufficient representation.


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
 #### 1st model
- The model shows a steady improvement in training accuracy, reaching around 80%, while validation accuracy remains relatively low at about 52%
- The significant disparity between training and validation accuracy suggests that the model may be overfitting to the training data, meaning it has learned patterns specific to the training set rather than generalizing well to new data.
- To address this issue, data augmentation techniques will be implemented. Since the training dataset is relatively small, additional samples will be created by applying transformations such as horizontal and vertical flips, slight rotations, and other modifications. These augmented images will help enhance the model's ability to generalize to unseen data.ity

 #### 2nd model
- Applying data augmentation has successfully reduced overfitting, leading to better generalization. However, the training and validation accuracy now fall within a similar range, indicating potential underfitting.
- After 20 epochs, the model achieves an accuracy of 58% on the training set and around 56% on the validation set.
- Even with the steps taken to minimize overfitting, the model is still not achieving optimal performance on either the training or validation data. This suggests that the current model may be too simplistic or lacks the capacity to capture complex patterns within the dataset, which is a common characteristic of underfitting.
-To enhance performance, further modifications may be necessary, such as refining the model’s architecture or extending the training duration by increasing the number of epochse.
 
 #### 3rd model
- Incorporating batch normalization into the model resulted in a modest increase in both training and validation accuracy.

- After 20 epochs, the model achieves an accuracy of 70% on the training set and around 64% on the validation set.

- To explore potential enhancements in accuracy, an alternative model will be developed without batch normalization for comparison.

#### 4th model
- The final model demonstrates a well-balanced performance, with no indications of underfitting or overfitting.

- Implementing class rebalancing has significantly improved the model’s accuracy on both the training and validation datasets..

- After 20 epochs, the final model achieves an accuracy of 75% on the training set and around 74% on the validation set.

- The minimal gap between training and validation accuracy highlights the strong generalization ability of the final CNN model.y.

- Incorporating batch normalization did not lead to any improvement in training or validation accuracy

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python - version 3.11.4
- Matplotlib - version 3.7.1
- Numpy - version 1.24.3
- Pandas - version 1.5.3
- Seaborn - version 0.12.2
- Tensorflow - version 2.15.0

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
- UpGrad tutorials on Convolution Neural Networks (CNNs) on the learning platform
- Melanoma Skin Cancer
- Introduction to CNN
- Image classification using CNN




## Contact
Created by Pratham Desai  - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
