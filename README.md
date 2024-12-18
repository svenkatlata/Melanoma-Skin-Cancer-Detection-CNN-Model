# Melanoma (Skin Cancer) Detection using custom CNN models

> Development of a multiclass classification model using a custom convolutional
> neural network (CNN) in TensorFlow to accurately detect melanoma from skin
> lesion images, aiding in early diagnosis and treatment.

## Table of Contents

- [General Info](#general-information)
- [Technologies Used](#technologies-used)
- [Conclusions](#conclusions)
- [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information

### Introduction

Skin cancer is one of the most common forms of cancer worldwide, with melanoma
being its most aggressive and life-threatening type. Early detection is crucial,
as it significantly improves survival rates and treatment outcomes. Melanoma
arises from melanocytes, the cells responsible for producing pigment in the
skin. Although it accounts for only a small fraction of skin cancer cases, it is
responsible for 75% of skin cancer-related deaths, underscoring the critical
need for timely diagnosis and treatment.

### Background

Traditional methods for melanoma diagnosis involve visual inspections by
dermatologists and the use of dermoscopy tools. While these methods are
effective, they require specialized expertise and can be time-consuming. With
advancements in medical imaging and machine learning, artificial intelligence
(AI) presents an opportunity to augment dermatological diagnostics by providing
automated, accurate, and fast detection of melanoma. A well-trained AI system
can assist healthcare professionals by evaluating skin lesion images and
flagging potentially cancerous cases for further analysis, thereby reducing the
workload and improving diagnostic accuracy.

### Problem Statement

The goal of this project is to develop a **multiclass classification model using
a custom convolutional neural network (CNN) in TensorFlow** that can accurately
detect melanoma from images of skin lesions. Given the high mortality rate
associated with melanoma, an automated detection system can play a crucial role
in early diagnosis and treatment. By leveraging deep learning, this solution
aims to minimize the manual effort required by dermatologists and ensure
consistent, reliable evaluations of skin lesion images. The proposed system will
act as a decision-support tool, helping to identify melanoma cases efficiently
and potentially saving lives.

### Dataset

The dataset used in this project consists of **2,357 images** representing both
malignant and benign oncological diseases. It is derived from the
**International Skin Imaging Collaboration (ISIC)**, a widely recognized source
of dermatological imaging data. The dataset is meticulously organized according
to the ISIC classification system, ensuring consistency and reliability for
training and evaluation.

The images are divided into subsets with an approximately equal distribution,
except for melanomas and moles, which are slightly more prevalent. This reflects
the practical scenario where certain conditions may occur more frequently.

The dataset includes the following skin conditions:

#### **Pre-Malignant Disease**

1. **Actinic Keratosis:** A precancerous, rough, scaly skin patch from sun
   damage.

#### **Malignant Diseases**

1. **Basal Cell Carcinoma (BCC):** A slow-growing skin cancer from basal cells.
2. **Squamous Cell Carcinoma (SCC):** A potentially invasive cancer from
   squamous cells.
3. **Melanoma:** The most aggressive skin cancer from pigment-producing cells.

#### **Benign Diseases**

1. **Dermatofibroma:** A harmless, firm skin growth, often on the legs.
2. **Nevus (Mole):** A benign collection of melanocytes (pigment cells).
3. **Pigmented Benign Keratosis:** Non-cancerous pigmented, rough skin patches.
4. **Seborrheic Keratosis:** Waxy, raised, benign skin growths.
5. **Vascular Lesion:** Non-cancerous blood vessel abnormalities.

This comprehensive dataset serves as the foundation for building and validating
the CNN-based melanoma detection model, enabling it to learn from a diverse
range of skin conditions and improving its accuracy and generalizability in
real-world applications.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions

- High Class Imbalance leads to Dominance of certain diseases.
- Data gets easily overfitted due to small size of the dataset.
- Data Augmentation in Tensorflow helped reducing Overfitting but did not
  improve the Accuracy of the model.
- Data Augmentation using Augmentor library improved the Train Accuracy (96%)
  and Validation Accuracy (87%) significantly. It also yielded a very small loss
  in both cases.
- However, Data Augmentation using Augmentor library caused Data leakeage
  between the train and the validation dataset due to which the model performs
  poorly on the Test dataset with an accuracy of 38% and loss of 5.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Technologies Used

- TensorFlow - version 2.17.1
- Augmentor - version 0.2.12
- Matplotlib

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements

**This is an Assignment done as a part of Executive PG Programme in AI & ML from
IIIT, Bangalore & upGrad.**

_Batch: ML C65_

## Contact

Reach out to the creators on GitHub using,

- [Venkat Lata](https://github.com/svenkatlata)

<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
