# 📌 Project Summary

**Title:** Zomato Sentiment Analysis and Restaurant Clustering using NLP and Machine Learning

This project focuses on extracting valuable business insights from Zomato’s vast database of customer reviews and restaurant metadata. Zomato, a popular restaurant aggregator and food delivery platform in India, collects millions of customer reviews, ratings, and restaurant details from cities across the country. These reviews contain a wealth of unstructured data that, if analyzed effectively, can reveal key trends in customer satisfaction and restaurant performance.

In this project, we use **Natural Language Processing (NLP)** and **Machine Learning (ML)** to analyze customer sentiment and group restaurants based on key features. The dual goal is to build a sentiment classification model that predicts whether a review is positive, neutral, or negative, and to cluster restaurants using features like average rating, cost, number of reviews, and sentiment score. This enables improved business decisions for both customers and Zomato’s internal teams.

The data used in this project consists of two primary sources:
- **Zomato Restaurant Reviews.csv** – containing textual customer reviews
- **Zomato Restaurant Metadata.csv** – including numerical and categorical data such as cost, number of reviews, average rating, and followers

The datasets were cleaned, merged, and enriched with additional features to enable effective model training and analysis.

---

## 🔧 Workflow & Methodology

The project follows a systematic seven-step pipeline:

1. **Data Loading and Merging**  
   Both datasets were imported and merged using restaurant identifiers to create a unified dataframe for analysis.

2. **Data Cleaning & Feature Engineering**  
   We removed missing values, duplicates, and irrelevant entries. Useful columns like total reviews, cost for two, and follower count were retained and scaled. Feature engineering helped improve model input quality and overall interpretability.

3. **Sentiment Labeling**  
   The original review dataset lacked explicit sentiment labels. To address this, we used **TextBlob**, a simple NLP library, to compute the sentiment polarity of each review. Based on polarity:
   - Scores > 0 were labeled **positive**
   - Scores < 0 were labeled **negative**
   - Scores = 0 were labeled **neutral**

4. **Text Preprocessing for NLP**  
   The review texts underwent thorough preprocessing:
   - Lowercasing
   - Removing punctuation, special characters, and stopwords
   - Lemmatization  
   The cleaned text was then vectorized using **TF-IDF (Term Frequency–Inverse Document Frequency)** to convert it into numerical format suitable for ML models.

5. **Encoding Target Labels**  
   The sentiment classes (positive, neutral, negative) were encoded into numerical labels (e.g., 0, 1, 2) to be used in classification algorithms.

6. **Model Building and Evaluation**  
   We implemented two machine learning models for sentiment classification:
   - **Logistic Regression**
   - **Random Forest Classifier**  
   After splitting the data into training and testing sets, both models were evaluated on metrics such as accuracy, precision, recall, and F1-score. Random Forest achieved better performance overall and handled class imbalance more effectively.

7. **Clustering Restaurants using KMeans**  
   Using restaurant-level features including cost, rating, number of reviews, followers, and average sentiment, we applied **KMeans clustering** to segment the restaurants. The results yielded three distinct clusters:
   - **Cluster 0**: Budget restaurants with mixed sentiment
   - **Cluster 1**: Premium restaurants with high ratings and positive sentiment
   - **Cluster 2**: Average-cost restaurants with lower satisfaction ratings  
   These clusters provide actionable insights for marketing, quality assurance, and user recommendations.

---

## 📈 Business Value

This project provides meaningful benefits for multiple stakeholders:
- **Zomato can use the sentiment analysis model** to monitor customer feedback automatically and detect areas needing attention.
- **The clustering approach** enables segmentation of restaurants, aiding strategic decisions around partnerships, promotions, and user targeting.
- **For end users**, this translates to better recommendations and a more intuitive review filtering system.

By combining **NLP**, **classification**, and **clustering**, the project transforms unstructured review data into structured insights—bridging technical capabilities with real-world impact.
