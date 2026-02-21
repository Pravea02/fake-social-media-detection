# 🔍 Fake Social Media Post Detection using Machine Learning

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3+-orange.svg)](https://scikit-learn.org)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

&gt; **MBA Business Analytics Project** | Marwadi University

## 📋 Overview
A Machine Learning system that detects fake social media posts by analyzing **sentiment patterns** and **content features**. Built using Natural Language Processing (NLP) and supervised learning algorithms.

**Research Title:** *"A Machine Learning–Based System for Detecting Fake Social Media Posts Using Sentiment and Content Analysis"*

## 🎯 Research Objectives
- Analyze how fake content influences sentiment-based social media analysis
- Develop ML models to automatically identify fake posts using text analysis

## 🛠️ Tech Stack
| Category | Tools |
|----------|-------|
| **Language** | Python |
| **ML Libraries** | scikit-learn, Pandas, NumPy |
| **NLP** | SpaCy, NLTK |
| **Visualization** | Matplotlib, Seaborn |
| **Feature Extraction** | TF-IDF Vectorization |

## 📊 Dataset
- **Source:** Twitter Validation Dataset (public academic dataset)
- **Size:** 1,000 tweets
- **Labels:** Positive, Negative, Neutral, Irrelevant

## 🔧 Methodology

### 1. Data Preprocessing
- Text cleaning (URLs, symbols, special characters removed)
- Tokenization & lemmatization using SpaCy
- Stop words removal
- TF-IDF vectorization

### 2. Machine Learning Models
| Model | Accuracy | Best For |
|-------|----------|----------|
| **Multinomial Naive Bayes** | 54.5% | Text classification |
| **Random Forest** | 51.0% | Feature importance |

## 📈 Results
- ✅ Successfully classified sentiment in social media posts
- ✅ Identified key patterns in fake vs. genuine content
- ⚠️ Challenge: Distinguishing Neutral vs. Irrelevant posts (language overlap)

## 🖼️ Visualizations
![Confusion Matrix](images/confusion_matrix.png)
*Confusion Matrix - Multinomial Naive Bayes*

![Model Comparison](images/model_comparison.png)
*Accuracy Comparison between Models*

![Sentiment Distribution](images/sentiment_distribution.png)
*Distribution of Sentiment Labels in Dataset*

## 💼 Business Applications
- **Brand Management:** Monitor fake reviews and misleading content
- **Marketing Analytics:** Filter genuine customer sentiment
- **Social Media Platforms:** Automated content moderation
- **Reputation Management:** Early misinformation detection

## 🚀 How to Run

```bash
# Clone repository
git clone https://github.com/Pravea02/fake-social-media-detection.git

# Install dependencies
pip install -r requirements.txt

# Download spaCy model
python -m spacy download en_core_web_sm

# Run the project
python fake_post_detection.py

fake-social-media-detection/
├── fake_post_detection.py    # Main Python script
├── requirements.txt          # Dependencies
├── Final project file.pdf    # Complete research paper
├── images/                   # Visualizations
│   ├── confusion_matrix.png
│   ├── model_comparison.png
│   └── sentiment_distribution.png
└── README.md                 # Project documentation
