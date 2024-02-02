# Sentiment-Analysis

## Overview

Sentiment analysis, also referred to as opinion mining, is a fundamental natural language processing (NLP) task dedicated to automating the identification of sentiment or emotional tone within textual content. The central objective is to discern whether the conveyed sentiment is positive, negative, or neutral. This project represents an exploration of sentiment analysis, using a combination of machine learning, deep learning, and NLP techniques. Its goal is to dissect textual data, unveiling the sentiments embedded within the text, thereby providing a comprehensive understanding of the emotional context expressed in diverse forms of language.


### Key Features

- **Web Scraping:** The project utilizes web scraping techniques to gather textual data from various sources, creating a diverse dataset for sentiment analysis within the context of NLP.
  
- **Preprocessing:** The collected data undergoes thorough preprocessing, including text cleaning, tokenization, and normalization, leveraging advanced NLP techniques to ensure high-quality input for the sentiment analysis models.

- **Machine Learning Models:** Multiple machine learning  and deep learning algorithms are implemented to capture complex relationships within the textual data and each model is trained and evaluated to understand its performance.

- **Natural Language Processing Techniques:** The project incorporates advanced NLP techniques, such as POS tagging , word embeddings, and Principal Component Analysis (PCA) to enrich the understanding and processing of natural language in the context of sentiment analysis.

- **Evaluation Metrics:** The project includes comprehensive evaluation metrics to assess the performance of each sentiment analysis model within the broader field of NLP, providing insights into their strengths and weaknesses.


### Objective

Sentiment analysis within the framework of NLP is crucial for businesses and organizations to understand public opinion and user feedback with a deeper understanding of language context. This project aims to provide a practical and scalable solution for sentiment analysis within the broader field of NLP, offering a range of models to cater to different datasets and requirements.

---

### Dataset Overview and Preprocessing Details

For detailed information about the dataset used in this project and the preprocessing steps applied, please refer to the [Data_Overview.md](Data_Overview.md) file.

---

# First Approach: Categorizing by Review Ratings

The reviews were categorized into three distinct sentiment categories: "Good," "Moderate," and "Bad." Reviews with ratings of 5 or 4 were categorized as "Good," those with a rating of 3 fell into the "Moderate" category, and any ratings of 2 or 1 were classified as "Bad."

### The following algorithms were implemented along with the respective evaluation metrics 

**Machine Learning Algorithms**
- Decision Tree
- Naive Bayes Classifier
- Random Forest
- Support Vector Machines (SVM)
- K-Nearest Neighbors (KNN)

**Deep Learning Algorithms**
- LSTM
- Bidirectional LSTM
- CuDNNLSTM (LSTM variant optimized for GPUs)
- Gated Recurrent Unit (GRU)
- XGBoost
- Convolution Neural Network (CNN)

For more details on the algorithms used, please refer to the respective folders:
- [Machine Learning Algorithms](Machine%20Learning%20Algorithms/)
- [Deep Learning Algorithms](Deep%20Learning%20Algorithms/)


### Resampling  
The distribution chart was analyzed for the three sentiment categories ("Good," "Moderate," and "Bad"). Due to an uneven distribution, resampling was performed to ensure a balanced representation of each sentiment category. This process was applied consistently across all machine learning and deep learning algorithms used previously.


### Principal Component Analysis to check for improvements
Principal Component Analysis (PCA) is a dimensionality reduction technique commonly used in various fields, including Natural Language Processing (NLP). It can be employed to enhance machine learning models in NLP by reducing the dimensionality of the feature space while preserving essential information. PCA is used to transform the original high-dimensional feature space into a lower-dimensional space while retaining as much of the variance in the data as possible. This reduction in dimensionality can lead to more efficient model training and potentially improved model performance. The number of principal components (PCs) to retain is a hyperparameter that can be tuned.

Principal Component Analysis (PCA) was employed for feature selection to reduce dimensionality and enhance the efficiency of the sentiment analysis models. 


### Dynamic Classifier Selection 
Dynamic Classifier Selection (DCS) is a machine learning technique used to improve classification performance by dynamically selecting an appropriate base classifier for each instance in the dataset. DCS can be particularly useful in scenarios where different base classifiers perform better on different subsets of the data. In traditional machine learning, a single base classifier (e.g., a decision tree, SVM, or neural network) is trained on the entire dataset. However, different instances within the dataset may exhibit varying levels of complexity or require different modeling approaches.

DCS Application: DCS improves model performance by selecting the most appropriate classifier for each data instance. Here's how it works:
- Classifier Pool: DCS typically starts with a pool of diverse base classifiers, each of which may have strengths and weaknesses.
- Instance-Level Selection: For each data instance to be classified, DCS analyzes the instance's characteristics and selects the most suitable base classifier from the pool.
- Combination or Voting: The predictions made by multiple base classifiers can be combined (e.g., by weighted voting) to produce the final classification decision.
- Dynamic Adaptation: The choice of the base classifier is dynamic, meaning it can vary from one instance to another.

This was employed to check for any improvements in the accuracy of the models.

### Ensemble Methods

Ensemble methods were employed to further enhance the performance of the sentiment analysis models. The following ensemble methods were utilized:

- **LSTM + BiLSTM + Random Forest**
- **CNN + Random Forest + Decision Tree**

These combinations leverage the strengths of multiple algorithms, contributing to a robust and accurate sentiment analysis system.

---

# Second Approach: Categorizing by Review Ratings

The reviews were now categorized into five distinct sentiment categories: "Excellent", "Good", "Moderate", "Bad" and "Poor" for ratings 5,4,3,2,1 respectively. The same steps as above was repeated for further analysis.

---

# Analysis 

For detailed information about the analysis, please refer to the [Data_Overview.md](Data_Overview.md) file.


