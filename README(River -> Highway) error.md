# EuroSAT – CNN Error Analysis (River → Highway)

## Overview
This notebook focuses on analysing misclassifications made by a custom CNN trained on the EuroSAT RGB dataset.

The primary objective is to investigate why satellite images belonging to the **River** class are incorrectly classified as **Highway**.

## Analysis Performed

1. **Misclassification Extraction:** Identifying images where the actual class is River but the predicted class is Highway.
2. **Confusion Analysis:** Examining confusion matrix results and identifying frequently confused classes.
3. **Image Inspection:** Visualizing misclassified satellite images to understand their visual characteristics.
4. **RGB and HSV Analysis:** Comparing colour characteristics of river and surrounding land regions.
5. **Threshold-based Segmentation:** Experimenting with Hue and Saturation thresholds to generate candidate water masks.
6. **Connected Component Analysis (CCA):** Identifying connected regions in binary masks using OpenCV.
7. **Geometric Analysis:** Examining component area, bounding box, aspect ratio, extent and solidity.
8. **Comparative Analysis:** Testing whether the observations and segmentation approach remain useful across different misclassified images.

## Technologies Used
- Python
- PyTorch
- OpenCV
- NumPy
- Matplotlib
- Pandas
- Scikit-learn

## Key Findings

- River and surrounding vegetation can have overlapping colour characteristics.
- Fixed HSV thresholds do not consistently generalize across satellite images.
- Connected Component Analysis helps identify spatially connected regions but cannot independently identify geographical features.
- Geometric properties provide useful insights but are insufficient for reliable river identification.

## Objective of Further Work

The findings from this investigation will help guide improvements to the CNN's feature-learning capabilities and classification performance.

## Dataset
[EuroSAT RGB Dataset – Kaggle](https://www.kaggle.com/datasets/apollo2506/eurosat-dataset)

## Related Notebook
[Data Processing and CNN Training](https://github.com/adityaDev-2005/Satellite-Image-Analysis-for-land-cover/blob/main/Satellite_Image_Analysis(Data%2BTraining).ipynb)

## Notebook
[River → Highway Error Analysis](https://github.com/adityaDev-2005/Satellite-Image-Analysis-for-land-cover/blob/main/Satellite_Image_Analysis_Error_Analysis(River_%3E_Highway).ipynb)
