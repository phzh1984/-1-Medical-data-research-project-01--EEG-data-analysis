# Medical Data Research Project-01--EEG-Data

Problem: Tinnitus is a subjective symptom or feeling; there is still a lack of an objective method to diagnose and detect tinnitus symptoms.

This project aims to use machine learning algorithms to classify tinnitus data, select the best classifier, and apply it in the clinical detection of tinnitus. This study would help doctors improve the efficiency of tinnitus detection so that tinnitus patients could get faster and more effective treatment in the later stages.

The goal of the tinnitus data analysis is to do a binary classification of whether a person is tinnitus or healthy based on their EEG data. During the experiment, different machine learning algorithms are used, and an optimal algorithm is selected for future classification prediction. The experimental steps are as follows：

1. The original data is the raw EEG data that includes the EEG data of 33 tinnitus patients and 47 non-tinnitus patients. Python-MNE package is first used to extract and integrate the original data, including exploratory analysis and visualization (PCA and TSNE). The EEG connectivity data (correlation between two brain areas) is the final raw data used to do this binary classification in Julia.
 
2. Split the raw data into a training set and a testing dataset, notice the training set was imbalanced based on the classification, so need to balance the training set as a classifier built based on an imbalanced training set may just classify any dataset to the majority votes in the training dataset.
 
3. Balanced data with all the features (325 dimensions) were classified and predicted using five different machine learning algorithms, including Logistic regression, KNN, Decision tree, SVM, and Random Forest.
   
4. Carry out dimension reduction on the balanced data and use PCA to reduce 325 dimensions to 200, 150, 100, 50, and 20 respectively, and then carry out classification by using the five algorithms on the dimension reduction data respectively.
   
5. Use the feature importance process in Python to extract the important features, select important features of 200, 150, 100, 50, and 20 respectively, and then use five different machine learning algorithms to do classification respectively.
    
6. Finally, find the optimal machine learning algorithm based on the classification prediction accuracy rate on the testing data. I found SVM had the best accuracy rate; the average accuracy is 92%. Logistic Regression, KNN, Decision Tree, and Random Forest achieved an average accuracy of 78%, 82%, 68%, and 69%, respectively. The SVM classifier should be selected as the best classifier in this experiment as it had the highest classification accuracy rate and lowest number of features.


I utilized Python to preprocess raw data, including data cleaning and integration. I prepared the training and testing datasets and selected and extracted features. To perform exploratory data analysis on the selected features, I employed Machine learning algorithms, including Logistic Regression, KNN, Decision Tree, SVM, and Random Forest, using Julia to design and implement algorithmic models. I conducted algorithm model optimization, parameter selection, model evaluation, and data classification prediction.

For more details please refer to the PDF version of the project presentation slides.
