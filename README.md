# zomato-eda-sentiment-clustering
NLP-based sentiment analysis and restaurant clustering using Zomato review data.
# 🍽️ Zomato Sentiment Analysis & Restaurant Clustering

A complete end-to-end machine learning project that:
- Analyzes customer review sentiments on Zomato
- Builds classification models using review text
- Clusters restaurants based on cost, rating, reviews, followers, and sentiment

---

## 📌 Project Overview

Zomato, one of India’s top food delivery and restaurant discovery platforms, has millions of user reviews. This project analyzes those reviews and restaurant metadata to extract useful business insights.

The project goals:
- Analyze sentiment from customer reviews using NLP
- Train machine learning models for sentiment classification
- Cluster restaurants using metadata and predicted sentiment
- Help Zomato identify customer satisfaction and segment restaurants

> **This project was provided by [AlmaBetter](https://www.almabetter.com/) as part of the Data Science curriculum.**

---

## 🧠 Workflow

| Step | Description |
|------|-------------|
| 1.   | Load Dataset |
| 2.   | Data Cleaning & Feature Engineering |
| 3.   | Sentiment Labeling |
| 4.   | Text Preprocessing (TF-IDF) |
| 5.   | Encode Target Labels |
| 6.   | ML Model Building (Logistic Regression, Random Forest) |
| 7.   | Clustering with KMeans |
| 8.   | Final Visualizations & Stakeholder Insights |

---

## 📊 Models & Performance

### ✅ Sentiment Classification

- **TF-IDF Vectorizer** for feature extraction
- **Logistic Regression** and **Random Forest Classifier** for sentiment prediction

| Model              | Accuracy |
|--------------------|----------|
| Logistic Regression|  **(fill in actual score here)**  |
| Random Forest      |  **(fill in actual score here)**  |

✅ Random Forest performed better overall with higher precision and recall for all sentiment classes.

---

### 🔍 Clustering Insights

Restaurants were clustered using:
- `Cost`
- `Rating`
- `Number of Reviews`
- `Number of Followers`
- `Sentiment (encoded)`

**KMeans Clustering** revealed 3 segments:
- **Cluster 0**: Budget restaurants with mixed reviews
- **Cluster 1**: Premium, high-rated, positive sentiment (Zomato should promote)
- **Cluster 2**: Average-cost but low-rated (potential improvement area)

---

## 📂 Dataset

All datasets used in this project are included in the `/data` folder of this repository:

- `data/Zomato Restaurant reviews.csv`
- `data/Zomato Restaurant names and Metadata.csv`

---

## 📦 Project Files

| File Name | Description |
|-----------|-------------|
| `Zomato_Sentiment_Clustering_Project.ipynb` | Main project notebook |
| `README.md` | This file |
| *(Optional)* PNG/CSV files | Supporting charts or data |

---

## 💼 Business Value to Stakeholders

- **For Zomato**: Identify top-performing and underperforming restaurants
- **For Customers**: Improve review-based restaurant recommendations
- **For Management**: Prioritize marketing and improvement efforts
- **For Analysts**: Build predictive models and cluster-based targeting

---

## 👨‍💻 Author

**Muhammad Hammaad Haque**  
*Machine Learning & Data Analysis Enthusiast*  
📧 hammaadhaque@gmail.com  

