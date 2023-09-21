# Medical Data Research Project: Tinnitus Data Classification Prediction

Project Overview

This project aims to address the challenge of diagnosing tinnitus, a subjective symptom, using machine learning algorithms. The goal is to classify tinnitus data and select the best classifier to assist in the clinical detection of tinnitus. By improving the efficiency of tinnitus detection, this research can contribute to faster and more effective treatment for tinnitus patients.

Dataset Information

The project involves binary classification of individuals as either tinnitus or healthy based on their EEG (Electroencephalogram) data. The dataset comprises raw EEG data from 33 tinnitus patients and 47 non-tinnitus patients. The Python-MNE package is used to extract and preprocess the raw EEG data, which includes exploratory analysis and visualization techniques such as PCA (Principal Component Analysis) and t-SNE (t-distributed Stochastic Neighbor Embedding). The final dataset used for binary classification is EEG connectivity data, representing the correlation between different brain areas.

Project Workflow

The project follows these key steps:

Data Preprocessing: Raw EEG data is processed, cleaned, and integrated using Python, including feature extraction and data exploration techniques like PCA and t-SNE.

Data Splitting: The dataset is divided into a training dataset and a testing dataset. Attention is given to balancing the training set to avoid classifier bias.

Classification and Prediction: Five different machine learning algorithms, including Logistic Regression, K-Nearest Neighbors (KNN), Decision Tree, Support Vector Machine (SVM), and Random Forest, are employed to classify and predict tinnitus cases using the balanced dataset with all features (325 dimensions).

Dimension Reduction: PCA is used to reduce the dimensionality of the data to 200, 150, 100, 50, and 20 dimensions, respectively. Classification is performed using the five algorithms on the reduced-dimension data.

Feature Importance: Important features are extracted using a feature importance process in Python. Features of 200, 150, 100, 50, and 20 are selected, and classification is carried out using the five different machine learning algorithms.

Optimal Algorithm Selection: Based on classification prediction accuracy on the testing data, the optimal machine learning algorithm is identified. SVM is found to have the highest average accuracy rate of 92%, making it the best classifier for this experiment.

The project includes:

Julia code segments showcasing the algorithmic models used in the project.

A section of the raw tinnitus patient dataset for reference.

Presentation slides providing a comprehensive overview of the research, including methodologies, results, and findings.
 




