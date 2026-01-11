# Twitter Sentiment Analysis: COVID-19 Vaccination 📊🐦

## 📌 Project Overview
This project performs **automated sentiment analysis** on Twitter data related to **COVID-19 vaccinations**.  
Using **Natural Language Processing (NLP)** and **Machine Learning**, the system classifies public opinion into three categories:

- ✅ Positive  
- ➖ Neutral  
- ❌ Negative  

The objective is to understand **public sentiment trends during the vaccination drive**, which can help **healthcare organizations, researchers, and policymakers** make informed decisions.

---

## 🚀 Features

- **Data Preprocessing**
  - URL removal  
  - Hashtag and mention stripping  
  - Lowercasing and tokenization  
  - Stopword removal and stemming using **NLTK**

- **Sentiment Labeling**
  - Automated sentiment labeling using **TextBlob polarity scores**

- **Visual Insights**
  - Sentiment distribution using **count plots** and **pie charts**
  - **WordClouds** to visualize frequently occurring words

- **Machine Learning Classification**
  - Feature extraction using **CountVectorizer**
  - Sentiment prediction using **Logistic Regression**

---

## 🛠️ Tech Stack

| Category          | Tools / Libraries |
|------------------|------------------|
| Language          | Python 3 |
| NLP               | NLTK, TextBlob |
| Machine Learning  | Scikit-learn (Logistic Regression) |
| Data Handling     | Pandas, NumPy |
| Visualization     | Matplotlib, Seaborn, WordCloud |

---

## 📊 Methodology

1. **Exploratory Data Analysis (EDA)**
   - Analyzed missing values and dataset statistics from `vaccination_tweets.csv`

2. **Text Cleaning**
   - Converted text to lowercase
   - Removed URLs, mentions, hashtags, punctuation, and special characters

3. **Feature Extraction**
   - Converted cleaned text into numerical features using **CountVectorizer**

4. **Sentiment Calculation**
   - Used **TextBlob** to assign polarity scores ranging from `-1` (negative) to `+1` (positive)

5. **Model Training**
   - Dataset split into **80% training** and **20% testing**
   - Trained a **Logistic Regression** classifier

---

## 📈 Results

The model achieved strong performance in classifying tweet sentiments.

### 🔹 Overall Performance
- **Accuracy:** 88%
- **Weighted Average F1-Score:** 0.87

### 🔹 Classification Report (Snapshot)

| Sentiment | Precision | Recall | F1-Score |
|----------|-----------|--------|----------|
| Neutral  | 0.84 | 0.98 | 0.90 |
| Positive | 0.94 | 0.85 | 0.90 |

> The model performs especially well in identifying **Neutral** and **Positive** sentiments.

---

## ⚙️ Installation & Usage

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/twitter-sentiment-analysis.git
cd twitter-sentiment-analysis
