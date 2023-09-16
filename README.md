# Brain_tumor_Classification

![image](https://github.com/AkshayRamakrishnann/Brain_tumor_Classification/assets/111365771/392b9426-352b-4ec7-919d-be7f3ddf75d3)


## Introduction 

In this section, we introduce another machine learning project focused on brain tumor classification using MRI images. The objective of this project is to develop and evaluate deep learning models for classifying brain tumors into different categories, such as glioma, meningioma, no tumor, and pituitary tumor, based on MRI scans.

## Data Collection

We began this project by downloading the brain tumor classification dataset from Kaggle using the `opendatasets` library. The dataset contains MRI images of brain tumors categorized into different classes.

## Data Exploration

Before diving into model building, we conducted initial data exploration to gain insights into the dataset. We displayed random images from each class to visualize the diversity of MRI scans in the dataset.

## Model Building

### Data Preprocessing and Augmentation

To prepare the MRI images for training deep learning models, we performed data preprocessing and augmentation:

- Rescaled pixel values to the range [0, 1].
- Applied data augmentation techniques, including rotation, width and height shifts, and horizontal flips, to increase the model's robustness.
- Split the data into training and validation sets using a validation split of 20%.

  ![image](https://github.com/AkshayRamakrishnann/Brain_tumor_Classification/assets/111365771/26e3fbcc-db20-4717-ac6c-4702f583202d)


### Model Architectures

We created and trained two deep learning models using pre-trained architectures: VGG16 and ResNet50. Both models were designed for image classification tasks.

#### VGG16 Model

- Utilized the VGG16 architecture with weights pre-trained on ImageNet.
- Added global average pooling, dense layers, and dropout for regularization.
- Compiled the model using the Adam optimizer and categorical cross-entropy loss.

#### ResNet50 Model

- Leveraged the ResNet50 architecture with pre-trained weights.
- Added global average pooling, dense layers, and dropout layers.
- Compiled the model with the Adam optimizer and categorical cross-entropy loss.

## Model Training

We trained both the VGG16 and ResNet50 models for 20 epochs using the augmented data. Below are the training results:

### VGG16 Model

- Achieved an initial training accuracy of approximately 73% and a validation accuracy of 69%.
- The training accuracy gradually improved, while the validation accuracy showed fluctuations.

### ResNet50 Model

- Started with an initial training accuracy of around 66% and a validation accuracy of 28%.
- The ResNet50 model experienced variations in validation accuracy during training.

![image](https://github.com/AkshayRamakrishnann/Brain_tumor_Classification/assets/111365771/a433621f-c225-481c-8b42-3e9b6090ea55)


## Conclusion

In this part of the project, we introduced a brain tumor classification task using MRI images. We explored the data, implemented data preprocessing and augmentation, and built and trained deep learning models using the VGG16 and ResNet50 architectures. While the models' performances were promising, there is room for further optimization and tuning to enhance their accuracy.

Please feel free to explore the code and results in this repository for a deeper understanding of the brain tumor classification project. If you have any questions or suggestions, don't hesitate to reach out.

Thank you for your interest in our Machine Learning projects!
