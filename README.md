# AI-Driven Pneumonia Detection and Information System

**Author:** Rayna Solanki  
**Date:** 07/04/2024

## Table of Contents
1. [Project Overview](#project-overview)
2. [Use Case Justification and Benefits](#use-case-justification-and-benefits)
3. [Dataset](#dataset)
4. [Model Selection](#model-selection)
5. [Model Comparisons](#model-comparisons)
6. [Evaluation Process](#evaluation-process)
7. [Conclusion](#conclusion)
8. [References](#references)
9. [Appendix](#appendix)

## Project Overview
This project combines Machine Learning (ML) and Artificial Intelligence (AI) to detect pneumonia from chest X-ray images and provides educational resources via a chatbot. The system aims to:
- Assist healthcare providers in making faster and more accurate diagnoses.
- Offer users crucial information about pneumonia symptoms, treatments, and prevention measures.

## Use Case Justification and Benefits
Pneumonia is a severe respiratory condition, particularly affecting children under five. This project addresses the challenges in diagnosing pneumonia, especially in low-resource settings with limited access to radiologists. The system offers:
- Automated analysis of chest X-rays to detect pneumonia.
- Timely and accurate diagnoses, allowing for quicker treatment.
- Reduced strain on healthcare professionals and lower diagnostic costs.
- An educational chatbot providing reliable information about pneumonia.

## Dataset
The dataset comprises 5,863 chest X-ray images from Guangzhou Women and Children’s Medical Center, specifically for pediatric patients aged 1-5 years. The images are categorized into 'Pneumonia' and 'Normal' states and are divided into train, test, and validation sets.

### Dataset Characteristics
- **Source:** Guangzhou Women and Children’s Medical Center
- **Number of Images:** 5,863
- **Age Group:** 1-5 years
- **Categories:** Pneumonia, Normal
- **Structure:** Organized into training, testing, and validation directories

## Model Selection
For the task of pneumonia detection from chest X-ray images, the Vision Transformer (ViT) was selected due to its advanced capabilities in image processing. ViT treats images as sequences of patches and applies self-attention mechanisms to capture global dependencies, making it highly effective for complex visual tasks.

### Key Features of Vision Transformer (ViT)
- **Global Context Understanding:** ViT processes entire images through self-attention, allowing for a deeper understanding of complex visual relationships.
- **High Accuracy:** ViT has set new benchmarks in image classification, making it ideal for nuanced tasks like medical image analysis.
- **Transfer Learning:** ViT can leverage pre-trained models, reducing the need for large datasets and extensive computational resources.
- **High-Resolution Processing:** Maintains intricate details in chest X-rays, crucial for accurate diagnosis.

## Model Comparisons
Several models were evaluated for their suitability in detecting pneumonia from chest X-rays:

| Model Type                | Validation Accuracy | Precision | Recall | F1 Score |
|---------------------------|---------------------|-----------|--------|----------|
| Convolutional Neural Network (CNN) | 0.7892              | 0.7489    | 0.9712 | 0.8457   |
| Residual Network (ResNet)         | 0.8023              | 0.7612    | 0.9835 | 0.8562   |
| Vision Transformer (ViT)          | 0.8141              | 0.7729    | 0.9949 | 0.8700   |

### Reasons for Choosing Vision Transformer (ViT)
- **Superior Performance:** ViT achieved the highest accuracy and F1 score among the models tested.
- **Efficiency with Small Datasets:** ViT's transfer learning capabilities allowed for effective training on the relatively small dataset.
- **Preservation of Image Details:** ViT's ability to process high-resolution images without significant downsampling ensures that subtle pneumonia indicators are not lost.

## Evaluation Process
The Vision Transformer model was evaluated using accuracy, precision, recall, and F1 score to measure its performance comprehensively. The dataset was split into 80% for training, 10% for validation, and 10% for testing. Cross-validation was also employed to ensure the model's robustness.

### Evaluation Metrics
- **Accuracy:** 0.8141
- **Precision:** 0.7729
- **Recall:** 0.9949
- **F1 Score:** 0.8700

These metrics highlight the model's strong capability in detecting pneumonia from chest X-rays, with particular emphasis on high recall, minimizing false negatives.

## Conclusion
The AI-Driven Pneumonia Detection and Information System demonstrates the potential of leveraging advanced AI models like Vision Transformer to support healthcare professionals and improve patient outcomes. The system's ability to quickly and accurately diagnose pneumonia, combined with the educational chatbot, provides a comprehensive tool for both medical and general users.
