# Satellite-Image-Analysis-for-land-cover

# Satellite Image Analysis for Land Cover Classification

## Overview
This project explores satellite image classification using Deep Learning and the **EuroSAT RGB dataset**. The objective is to classify satellite images into 10 different land-cover categories using a custom Convolutional Neural Network (CNN).

## Dataset
- **Dataset:** EuroSAT RGB
- **Image dimensions:** 64 × 64 pixels
- **Channels:** 3 (RGB)
- **Number of classes:** 10
- **Training images:** 18,900
- **Validation images:** 5,400
- **Test images:** 2,700

## Implementation

The notebook covers the following stages:

1. **Data Loading:** Downloading and accessing the EuroSAT dataset.
2. **Data Preparation:** Loading image paths and labels using CSV files.
3. **Preprocessing:** Decoding images, converting them into tensors and scaling pixel values.
4. **Dataset & DataLoader:** Creating a custom PyTorch Dataset and DataLoaders.
5. **CNN Architecture:** Implementing a custom CNN using PyTorch.
6. **Model Training:** Training the network using Adam optimizer and Cross-Entropy Loss.
7. **Validation:** Monitoring training and validation loss and accuracy across epochs.
8. **Model Saving:** Saving trained model weights for subsequent evaluation.

## Technologies Used
- Python
- PyTorch
- Torchvision
- NumPy
- Pandas
- Matplotlib
- Google Colab

## Model
The project uses a custom CNN consisting of convolutional layers, ReLU activation, max-pooling and fully connected layers to perform 10-class land-cover classification.

*Note: The dataset and trained model checkpoint are stored separately and are not included in the repository.*

## Next Steps
- Perform detailed error analysis.
- Experiment with data augmentation and CNN architecture improvements.
- Explore advanced architectures such as Swin Transformer.
- Compare models using validation and final test performance.

## Notebook
[Open Data Processing & Training Notebook](https://github.com/adityaDev-2005/Satellite-Image-Analysis-for-land-cover/blob/main/Satellite_Image_Analysis(Data%2BTraining).ipynb)
