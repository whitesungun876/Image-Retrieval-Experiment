Image Retrieval with SIFT Features
This repository demonstrates an image retrieval system using SIFT features, bag-of-words (BoW) model, and multiple similarity measures (TF-IDF, KL Divergence).

Requirements
Python 3.x
OpenCV
Scikit-learn
NumPy
Matplotlib
Functionality
Data Loading: Loads image data, splits into training and testing datasets, and labels images by categories.
Feature Extraction: Extracts SIFT features from images for each category.
Visual Vocabulary: Creates a vocabulary using K-Means clustering on the extracted features.
BoW Histograms: Computes BoW histograms for each image using the visual vocabulary.
Similarity Measures: Evaluates similarity between images using:
TF-IDF similarity
Kullback-Leibler (KL) Divergence
Image Retrieval: For a given test image, retrieves the top 3 similar images from the training set using the chosen similarity measure.
Evaluation: Calculates Mean Reciprocal Rank (MRR) and Top-3 Accuracy to assess retrieval performance.
Usage
Modify data_path to point to your dataset directory.
Specify categories in the categories list.
Run the script to perform image retrieval experiments using TF-IDF and KL Divergence.
Example Output
bash
复制代码
Experiment 1 (TF-IDF Similarity):
Mean Reciprocal Rank (MRR): 0.XXXX
Top-3 Accuracy: XX.XX%

Experiment 2 (KL Divergence):
Mean Reciprocal Rank (MRR): 0.XXXX
Top-3 Accuracy: XX.XX%
