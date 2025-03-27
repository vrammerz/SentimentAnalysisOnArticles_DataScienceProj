# 📰 NYT Sentiment Analysis on Automation & Technology Articles

This project queries the **New York Times Article Search API** to collect, clean, and analyze articles that mention **Automation**, **Technology**, and **Robotics**. The goal is to understand the **sentiment distribution** of news coverage on these topics.

## 📌 Project Overview

1. **Data Collection**  
   Uses the New York Times API to fetch recent articles with relevant keywords. Extracts useful fields like headline, abstract, publication date, source, and web URL.

2. **Data Preprocessing**  
   Applies natural language processing techniques including:
   - Lowercasing  
   - Tokenization  
   - Punctuation removal  
   - Stopword removal  
   - Lemmatization  
   
   Focused on the article `headline` and `abstract` fields.

3. **Sentiment Analysis**  
   Uses the `VADER SentimentIntensityAnalyzer` from NLTK to analyze the sentiment of the headlines and abstracts. Each is categorized into:
   - **Positive**
   - **Neutral**
   - **Negative**

4. **Visualization**  
   Generates plots to visualize sentiment trends, including:
   - Sentiment distribution histograms  
   - Scatter plot showing the correlation between headline and abstract sentiment scores  

## 📁 Files

- `Sentiment Analysis on Automation & Technology Articles.ipynb` – Main Jupyter Notebook
- `nyt_articles.json2` – Raw NYT articles dataset (fetched from API)
- `preprocessed_nyt_articles.json` – Cleaned and preprocessed articles
- `README.md` – You’re reading it!

## 🛠️ Dependencies

Install the following libraries before running the notebook:

```bash
pip install requests nltk matplotlib
