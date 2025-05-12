# Spam Email Filter

This project is a Machine Learning-based system to detect spam emails using Natural Language Processing (NLP), feature extraction (TF-IDF), and classifiers such as Logistic Regression, Naive Bayes, and an Ensemble Voting Classifier. It also demonstrates dataset shift analysis between earlier and recent spam trends.

## Features
- Real-time spam prediction
- Preprocessing: Tokenization, stemming, lemmatization
- Time-based email analysis (1980–2020)
- TF-IDF vectorization and topic modeling
- Logistic Regression and Ensemble classifier comparison
- Dataset shift evaluation

## Dataset
The dataset combines:
- CEAS 2008
- SpamAssassin
- Nigerian Scam emails

These are merged, cleaned, and split into:
- `df_earlier`: 1980–2007
- `df_recent`: 2008–2020

## Setup Instructions

### Step 1: Install Dependencies
Make sure you have Python 3.7+ and install required libraries:

```bash
pip install pandas numpy matplotlib seaborn nltk scikit-learn imbalanced-learn wordcloud
```

### Step 2: Download Required NLTK Resources

```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
```

### Step 3: Run the Notebook
Open and run `SpamFilter.ipynb` in Jupyter or Google Colab. It includes:
- Training on older email datasets
- Performance visualization
- Real-time prediction with custom email text input

## Try It Out
At the bottom of the notebook, input your own email content and the model will tell you if it's **Spam** or **Ham**.

## Author
Your Name
