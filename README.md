# Remote Sensing Image Classification

Computer vision project comparing traditional machine learning and deep learning approaches for classifying remote-sensing images.

## Project Overview

- **Dataset:** 12,000 remote-sensing images
- **Classes:** 15 landscape categories
- **Models compared:** SIFT + KNN, SIFT + SVM, ResNet-18, EfficientNet
- **Evaluation:** Accuracy, Precision, Recall, F1-score, and Confusion Matrix

### Dataset Samples

![Dataset samples](images/dataset_samples.jpg)

## Results on the Original Dataset

| Model | Accuracy |
|---|---:|
| SIFT + KNN | 55.50% |
| SIFT + SVM | 63.25% |
| ResNet-18 | 88.38% |
| **EfficientNet** | **97.00%** |

EfficientNet achieved the best performance on the original dataset, while both deep learning models outperformed the traditional machine learning approaches.

### EfficientNet Confusion Matrix

![EfficientNet confusion matrix](images/efficientnet_confusion_matrix.jpg)

## Data Processing Experiment

To study a more imbalanced setting, the original balanced dataset was converted into a long-tail distribution and then rebalanced using data augmentation such as flipping, rotation, and cropping.

The processed dataset produced higher scores, but further analysis suggested that similar augmented images may have appeared across the training and test sets, potentially inflating the evaluation results. For this reason, the **97.0% accuracy on the original dataset** is used as the main reported result.

## Methods

`SIFT` `KNN` `SVM` `ResNet-18` `EfficientNet` `Computer Vision` `Machine Learning` `Deep Learning`

---

*UNSW COMP9517 Computer Vision group project.*
