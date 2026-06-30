# 🐦 Twitter Sentiment Analysis using Machine Learning

## 📌 Project Overview

This project performs **Sentiment Analysis** on Twitter data using Natural Language Processing (NLP) and Machine Learning techniques. The objective is to classify tweets into **Positive**, **Negative**, or **Neutral** sentiment based on their textual content.

The project implements a complete NLP pipeline, including text preprocessing, feature extraction with **TF-IDF**, model training using multiple machine learning algorithms, and comprehensive model evaluation.

---

## 🎯 Objectives

- Analyze the sentiment expressed in Twitter posts.
- Preprocess noisy social media text using NLP techniques.
- Convert textual data into numerical features using TF-IDF.
- Train and compare multiple machine learning models.
- Evaluate model performance using classification metrics.
- Predict the sentiment of unseen tweets.

---

## 📂 Dataset

The project uses the **Twitter_Data.csv** dataset containing approximately **163,000 tweets**, primarily related to Indian politics.

### Dataset Columns

| Column | Description |
|--------|-------------|
| clean_text | Pre-cleaned tweet text |
| category | Sentiment label (-1 = Negative, 0 = Neutral, 1 = Positive) |

### Sentiment Labels

| Label | Meaning |
|-------|---------|
| -1 | Negative |
| 0 | Neutral |
| 1 | Positive |

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NLTK
- WordCloud
- Scikit-learn

---

## 📚 Natural Language Processing Techniques

- Text Cleaning
- Lowercase Conversion
- URL Removal
- Punctuation Removal
- Stopword Removal
- Tokenization
- Lemmatization
- TF-IDF Vectorization

---

## 🤖 Machine Learning Models

The following classification algorithms were implemented and compared:

- Multinomial Naive Bayes
- Logistic Regression
- Linear Support Vector Machine (Linear SVM)

---

## 📊 Project Workflow

### 1. Data Loading

- Load Twitter dataset
- Inspect data structure
- Handle missing values
- Check sentiment distribution

### 2. Text Preprocessing

- Convert text to lowercase
- Remove URLs
- Remove punctuation and numbers
- Remove stopwords
- Perform lemmatization
- Generate cleaned tweets

### 3. Exploratory Data Analysis

- Sentiment distribution
- Tweet length analysis
- Word Clouds
- Top frequent words
- Class balance visualization

### 4. Feature Engineering

- TF-IDF Vectorization
- Unigrams and Bigrams
- Vocabulary size limitation

### 5. Model Training

- Train-Test Split (80:20)
- Train Naive Bayes
- Train Logistic Regression
- Train Linear SVM

### 6. Model Evaluation

- Accuracy
- Precision
- Recall
- F1-Score
- Weighted F1
- Classification Report
- Confusion Matrix
- Model Comparison

### 7. Prediction

- Predict sentiment for new tweets entered by the user.

---

## 📈 Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Weighted F1 Score
- Confusion Matrix

Weighted F1 Score was used because the dataset is moderately imbalanced.

---

## 📊 Visualizations

The project includes several visualizations to better understand the data:

- Sentiment Distribution
- Tweet Length Distribution
- Word Clouds for each sentiment
- Top Frequent Words
- Model Performance Comparison
- Confusion Matrices
- Most Predictive Words (Logistic Regression)

---

## 📁 Project Structure

```
Twitter-Sentiment-Analysis/
│
├── Twitter_Data.csv
├── Twitter_Sentiment_Analysis.ipynb
├── README.md
└── requirements.txt
```

---

## 🚀 Installation

### Clone the repository

```bash
git clone https://github.com/yourusername/Twitter-Sentiment-Analysis.git
```

### Navigate to the project directory

```bash
cd Twitter-Sentiment-Analysis
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```
Twitter_Sentiment_Analysis.ipynb
```

---

## 📦 Requirements

```
numpy
pandas
matplotlib
seaborn
nltk
wordcloud
scikit-learn
jupyter
```

---

## 🔍 Sample Prediction

Example tweets and predicted sentiments:

| Tweet | Predicted Sentiment |
|--------|---------------------|
| *I absolutely love how this policy is helping people!* | 😊 Positive |
| *This is the worst decision the government has ever made.* | 😠 Negative |
| *Not sure how I feel about this.* | 😐 Neutral |

---

## 📌 Key Findings

- The dataset contains approximately **163K tweets**.
- Positive tweets are the most common, followed by neutral and negative tweets.
- TF-IDF proved to be an effective feature extraction technique for text classification.
- Logistic Regression and Linear SVM outperformed Naive Bayes on this dataset.
- Weighted F1 Score provided a fair evaluation due to class imbalance.
- The Logistic Regression model offers interpretability by identifying the most influential words for each sentiment class.

---

## 🚀 Future Improvements

Possible enhancements include:

- Hyperparameter tuning using Grid Search or Random Search
- Word Embeddings (Word2Vec, GloVe, FastText)
- Deep Learning models (LSTM, GRU)
- Transformer-based models (BERT, RoBERTa)
- Handling class imbalance with class weighting or SMOTE
- Deployment as a web application using Flask or Streamlit

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Your Name**

GitHub: https://github.com/yourusername

---

## ⭐ Acknowledgements

- NLTK
- Scikit-learn
- Pandas
- Matplotlib
- Seaborn
- WordCloud
