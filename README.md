# Face Identification from the LFW Dataset  (PRML Project Group-14)
## Overview
The Labeled Faces in the Wild (LFW) dataset challenges automated facial recognition with its real-world, uncontrolled conditions. Our project aims to accurately identify individuals by matching and ranking facial features against a comprehensive database.

## Proposed Approach

### Feature Extraction Methods
To interpret the complex facial data, we implemented three feature extraction strategies:

1. **Pre-trained ResNet Features**:
   Utilizing ResNet's deep learning capabilities, we extract a 2048-dimensional feature vector that encapsulates high-level facial attributes.

2. **Histogram of Oriented Gradients (HOG)**:
   HOG descriptors provide a detailed 70,308-dimensional vector, emphasizing edge and gradient structures crucial for object detection.

3. **Local Binary Patterns (LBP)**:
   We used LBP to produce a 256-dimensional vector, effectively capturing the essential textural nuances of facial features.

### Dimensionality Reduction with PCA
To manage the computational load and harmonize feature dimensions, Principal Component Analysis (PCA) streamlined the feature vectors, preserving the most significant data variances.

### Classification Models
Our analytical arsenal included diverse models to ensure robust identification:

- **K-Nearest Neighbors (KNN)**: Classifies images by analyzing feature vector proximity.
- **Logistic Regression**: Estimates probabilities for binary classifications.
- **Support Vector Machine (SVM)**: Distinguishes classes with an optimal feature space hyperplane.
- **Random Forest**: Enhances accuracy with a collective of decision trees.
- **XGBoost**: A speed-optimized gradient boosting framework, celebrated for its competitive performance.

## Project Structure

- **Web Demo Repository**: [View on GitHub](https://github.com/Stardust-01/Face-classification-using-LinearSVC/tree/main)
- **Project Page Link**: [View Project Page](https://anuj-l22.github.io/PRML_Project/)
- **Spotlight Video**: [View Spotlight Video](https://youtu.be/1AO8YunbgLs)
- **Project Slides**: [View Project Slides](https://drive.google.com/file/d/1vsw37vBgCabxMDzO2PGN_UXN6wJ3DGzC/view?usp=sharing)
- **Project Report**: [View Project Report](https://drive.google.com/file/d/1Fqjq3UV_l51ADNIQLj_Ix7QMpLmtnjq2/view?usp=sharing)
- **Web Demo**: [Try the Live Demo](https://face-classification-using-linearsvc-9mqdfclrzf5wdkmvj9ndj7.streamlit.app/)
- **PRML_Project.ipynb**: Data preprocessing and EDA for LFW. [Used in Midreport]
- **CNN_Models.ipynb**: Upcoming models utilizing CNN-extracted features.
- **Saved Models**: Repository for deployed and tested models.

![Face Identification Interface](lfw_image.png) <!-- Replace with the actual path to the image -->

