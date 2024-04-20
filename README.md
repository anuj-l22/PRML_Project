# Face Identification from the LFW Dataset Using LinearSVC

## Problem Statement
The Labeled Faces in the Wild (LFW) dataset presents a challenge for automated facial recognition due to its real-world, unconstrained conditions. Face identification requires precise recognition, matching, and ranking individuals' faces against a large database of known identities.

## Proposed Approach
We propose a system that utilizes a Linear Support Vector Classification (LinearSVC) approach to process and classify facial features. Our method involves applying Principal Component Analysis (PCA) to reduce dimensionality, followed by training LinearSVC models to predict the likelihood of identity matches. For any given input image, the system outputs the top 5 identity predictions, providing a ranked list of potential matches and significantly narrowing down search results for efficient identification.

## Project Structure
- **Link for Web Demo repository**: [GitHub Repository](https://github.com/Stardust-01/Face-classification-using-LinearSVC/tree/main)
- **Link for Web Demo**: [Face Classification Web Demo](https://face-classification-using-linearsvc-9mqdfclrzf5wdkmvj9ndj7.streamlit.app/)
- **PRML_Project.ipynb**: Contains data preprocessing and exploratory data analysis (EDA) for the LFW dataset.
- **PRML_Feat_ext.ipynb**: Includes code used for feature extraction.
- **Feature_extraction.ipynb**: Details the models trained on the extracted features, beginning with PCA and logistic regression.
- **CNN_Models.ipynb**: Will house models trained on CNN features.
- **Saved models**: Consists of the trained models ready for deployment and testing.

![Face Identification Interface](path_to_image)  <!-- Replace with the path to the image after adding it to your repository -->
