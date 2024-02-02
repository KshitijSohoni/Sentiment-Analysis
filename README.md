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
- [Machine Learning Algorithms](Sentiment-Analysis/Machine Learning Algorithms/)
- [Deep Learning Algorithms](Sentiment-Analysis/Deep Learning Algorithms/)
