# Face Identification from the LFW Dataset 

## Problem Statement
The Labeled Faces in the Wild (LFW) dataset presents a challenge for automated facial recognition due to its real-world, unconstrained conditions. Face identification requires precise recognition, matching, and ranking individuals' faces against a large database of known identities.

## Proposed Approach

Feature Extraction Methods
We employed three distinct methods to extract features from the images:
1. Pre-trained ResNet Features[6]: Utilizing a pre-trained ResNet model, we extracted high-level
features from the images, resulting in a 2048-dimensional feature vector per image. This approach
leverages deep learning to capture intricate patterns and characteristics of faces.
2. Histogram of Oriented Gradients (HOG)[3]: The HOG feature descriptor was used to capture
edge and gradient structure information from the images, producing a 70,308-dimensional vector.
This method is traditionally renowned for its effectiveness in object detection tasks.
3. Local Binary Patterns (LBP)[5]: We extracted texture features using the LBP technique,
which provided a 256-dimensional feature vector per image. LBP is particularly useful for capturing
fine-grained texture details that are often pivotal in facial recognition.
Dimensionality Reduction with PCA
Given the high dimensionality of the extracted features, especially from the ResNet and HOG methods,
we applied Principal Component Analysis (PCA) [9] to reduce the feature dimensions. This step was
crucial to alleviate computational demands and to standardize the feature space across different methods
for a fair comparison of model performances. PCA was tailored for each feature type, ensuring optimal
dimension reduction while retaining significant variance in the data.
Classification Models
We experimented with the following classification models on the dimensionally reduced features:
• K-Nearest Neighbors (KNN)[4]: A simple yet effective model that classifies images based on
the closest feature vectors in the training set.
• Logistic Regression: A fundamental statistical model used to estimate probabilities using a
logistic function, ideal for binary classification tasks.
• Support Vector Machine (SVM)[7]: This model finds the hyperplane that best separates
different classes in the feature space, which is critical in high-dimensional spaces.
• Random Forest[1]: An ensemble method that uses multiple decision trees to improve classifica-
tion accuracy and control over-fitting.
• XGBoost[2]: An implementation of gradient boosted decision trees designed for speed and per-
formance, which has proven effective in various machine learning competitions
## Project Structure
- **Link for Web Demo repository**: [GitHub Repository](https://github.com/Stardust-01/Face-classification-using-LinearSVC/tree/main)
- **Link for Web Demo**: [Face Classification Web Demo](https://face-classification-using-linearsvc-9mqdfclrzf5wdkmvj9ndj7.streamlit.app/)
- **PRML_Project.ipynb**: Contains data preprocessing and exploratory data analysis (EDA) for the LFW dataset.
- **PRML_Feat_ext.ipynb**: Includes code used for feature extraction.
- **Feature_extraction.ipynb**: Details the models trained on the extracted features, beginning with PCA and logistic regression.
- **CNN_Models.ipynb**: Will house models trained on CNN features.
- **Saved models**: Consists of the trained models ready for deployment and testing.

![Face Identification Interface](path_to_image)  <!-- Replace with the path to the image after adding it to your repository -->
