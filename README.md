# Automated Diagnosis of Hydroxychloroquine Retinopathy Using AI

This project explores the possibility of using AI to diagnose HCQ retinopathy on OCT scans, specifically convolutional neural networks (CNNs) like ResNet and Vision Transformers (ViT). Given the limited size of the dataset, this study explores various approaches, including pre-trained models and ensemble methods, to optimize performance.

## Dataset

The dataset consists of 657 OCT scans from 308 patients. Each patient has multiple scans of both eyes, captured at different times, representing the progression of the disease. Of these, 122 scans show signs of retinopathy.

- **Training Set**: 60% of the dataset.
- **Validation Set**: 20% of the dataset.
- **Test Set**: 20% of the dataset.

- **Validation**: 5-fold cross-validation on the training set/

## Key Approaches and Models

Two main approaches were explored to diagnose HCQ retinopathy:

1. **Single Model Approach**: Fine-tuning pre-trained models such as ResNet and testing with different slices of the scans.
2. **Ensemble Model Approach**: Using the same model on all slices, then combining the results to improve the performance.

For detailed methodology and results, refer to the full report.

## Results

The best models achieved the following performance at 90% recall:

- **Single Model Approach**: 54% specificity.
- **Ensemble Model Approach**: 58% specificity.

For additional results, ROC curves, and training plots, please refer to the detailed report. 

## Usage

The notebook is intended to run on Google Colab. To save or access files such as the model config or the dataset, it is necessary to mount a Google Drive.
**Access the project with this link :** https://drive.google.com/drive/folders/1GFUV0wFicjKe_1vFqpnPL56a3qRcTgud?usp=sharing
