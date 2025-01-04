# Fake News Analysis and Prediction  

This project focuses on analyzing and predicting article popularity using Natural Language Processing (NLP) techniques and Machine Learning models. The dataset includes fake and real news articles from various sources. The project performs tasks like text preprocessing, Named Entity Recognition (NER), feature engineering, and model evaluation using classification and regression techniques.  

---

## Table of Contents  
- [Introduction](#introduction)  
- [Dataset](#dataset)  
- [Project Workflow](#project-workflow)  
- [Features Extracted](#features-extracted)  
- [Models Used](#models-used)  
- [Evaluation Metrics](#evaluation-metrics)  
- [Results](#results)  
- [Visualizations](#visualizations)  
- [Usage](#usage)  
- [Requirements](#requirements)  
- [License](#license)  

---

## Introduction  
The goal of this project is to analyze the content of fake and real news articles, extract meaningful features, and build predictive models to classify news as real or fake and predict article engagement metrics.  

---

## Dataset  
The dataset is sourced from the [FakeNewsNet repository](https://github.com/KaiDMML/FakeNewsNet). It consists of:  
- **Politifact**: Fake and real news articles.  
- **Gossipcop**: Fake and real news articles.  

Each article contains fields like the title, text, and engagement metrics (e.g., likes, shares).  

---

## Project Workflow  
1. **Text Preprocessing**: Cleaning text, removing HTML tags, special characters, and stopwords.  
2. **Named Entity Recognition (NER)**: Extracting counts of organizations, locations, and persons from the articles.  
3. **Feature Engineering**:  
   - Article length (word count).  
   - Sentiment scores using TextBlob.  
   - Engagement metrics (derived from tweet IDs).  
4. **Model Training and Evaluation**:  
   - Classification using a Random Forest Classifier.  
   - Regression using a Random Forest Regressor.  
5. **Cross-Validation**: 10-fold cross-validation for model evaluation.  
6. **Visualizations**: Bar plots, scatter plots, and heatmaps to analyze data.  

---

## Features Extracted  
The following features are used for analysis:  
- **NER Features**:  
  - `org_count`: Number of organizations mentioned.  
  - `gpe_count`: Number of locations mentioned.  
  - `person_count`: Number of persons mentioned.  
- **Article Length**: Word count of the article's title.  
- **Sentiment Score**: Polarity score using TextBlob.  
- **Engagement Metric**: Proxy for likes/shares/comments.  

---

## Models Used  
1. **Random Forest Classifier**: To classify news as fake or real.  
2. **Random Forest Regressor**: To predict engagement metrics.  

---

## Evaluation Metrics  
The models are evaluated using the following metrics:  
- **Classification**:  
  - Accuracy  
  - F1 Score  
- **Regression**:  
  - R² Score  
  - Mean Absolute Error (MAE)  

---

## Results  
1. **Classification Results**:  
   - **Accuracy**: ~XX.XX%  
   - **F1 Score**: ~XX.XX  

2. **Regression Results**:  
   - **R² Score**: ~XX.XX  
   - **Mean Absolute Error (MAE)**: ~XX.XX  

---

## Visualizations  
The following visualizations are included:  
- **Entity Frequency Bar Chart**: Displays counts of `org_count`, `gpe_count`, and `person_count`.  
- **Sentiment vs. Engagement Scatter Plot**: Highlights the relationship between sentiment and engagement metrics.  
- **Feature Correlation Heatmap**: Shows correlations among features and engagement metrics.  

---

## Usage  
1. Clone the repository:  
   ```bash  
   git clone https://github.com/<your-username>/fake-news-analysis.git
