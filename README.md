# Chest X-Ray Classification Using Deep Learning

This project focuses on classifying chest X-ray images into multiple pulmonary disease categories using deep learning techniques and transfer learning.

##  Project Overview
Chest X-rays are widely used to detect lung diseases, but interpreting them requires high expertise and time.  
This project aims to build a **deep learning-based decision support system** that assists doctors by automatically classifying chest X-ray images.

 This system is intended to support medical professionals, not replace them.

##  Disease Classes
The model classifies chest X-ray images into **6 categories**:
- Normal
- COVID-19
- Pneumonia (Bacterial)
- Pneumonia (Viral)
- Tuberculosis
- Emphysema

##  Dataset
- **Dataset name:** Chest X-Ray 6-Class Dataset  
- **Source:** Kaggle  
- **Total images:** 18,036  
- **Image size:** 224 × 224  

Dataset link:  
https://www.kaggle.com/datasets/mohamedasak/chest-x-ray-6-classes-dataset

 The dataset is not included in this repository due to its large size.

##  Technical Approach
- **Model:** DenseNet121 (pre-trained on ImageNet)
- **Technique:** Transfer Learning
- **Frameworks:** TensorFlow & Keras
- **Preprocessing:**
  - Image resizing (224×224)
  - Normalization
  - Data augmentation
- **Optimizer:** Adam
- **Loss Function:** Categorical Crossentropy

##  Hyperparameter Tuning
Several combinations were tested:
- Learning rates: 0.001, 0.0001, 0.00001
- Epochs: 5, 10, 20

 Best configuration:
- Learning rate = 0.0001  
- Epochs = 10

## Results
- **Test Accuracy:** ~80.5%
- **Test Loss:** ~0.43
- Strong performance on:
  - Normal
  - Tuberculosis
- Main challenge:
  - Distinguishing between Pneumonia-Viral and Pneumonia-Bacterial

## Evaluation Metrics
- Precision
- Recall
- F1-score
- Confusion Matrix

## Future Work
- Apply advanced fine-tuning
- Try other models (ResNet, EfficientNet)
- Improve class balance
- Increase dataset size

## How to Run
1. Install required libraries:
   pip install -r requirements.txt
2. Open the Jupyter Notebook and run all cells.

## Disclaimer
This project is for educational and research purposes only.

