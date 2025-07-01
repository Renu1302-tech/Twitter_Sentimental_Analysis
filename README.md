# Twitter Sentiment Analysis

This project performs sentiment analysis on a Twitter dataset using various machine learning and deep learning models. It involves extensive text preprocessing, feature extraction, and model evaluation to classify tweets as positive or negative.

[![Open In Colab](https://colab.research.google.com/github/Renu1302-tech/Twitter_Sentimental_Analysis/blob/master/Twitter_Analysis.ipynb)

---

## 📁 Files in This Repository

- `Twitter_Analysis.ipynb`: The complete Jupyter Notebook containing preprocessing, model building, and evaluation.
- `README.md`: Description of the project and instructions to run it.

---

## 📊 Dataset

The dataset used (`Twitter_Dataset.csv`) contains 1.6 million tweets with sentiment labels (0 = negative, 4 = positive). Due to GitHub's 100MB file limit, it is not included in this repository.

**To access the dataset:**
- Place your copy of `Twitter_Dataset.csv` in the appropriate path when running the notebook.
- File encoding: `ISO-8859-1`
- Columns:  
  - `sentiment_label`, `ids`, `date`, `flag`, `user`, `text`

---

## 🛠️ Steps Performed

1. **Mount Google Drive** (for dataset access in Colab)
2. **Load dataset and assign headers**
3. **Data Cleaning**
   - Remove punctuation, numbers, and stopwords
   - Lowercasing and lemmatization
4. **EDA**
   - Class distribution
   - Word clouds for positive and negative tweets
5. **Feature Engineering**
   - TF-IDF Vectorization
   - Tokenization and padding for LSTM
6. **Model Training**
   - Logistic Regression
   - Support Vector Machine (LinearSVC)
   - XGBoost
   - LSTM (deep learning)
7. **Evaluation Metrics**
   - Accuracy, Recall, F1-Score
   - Classification report for each model

---

## 📦 Libraries Used

- `pandas`, `numpy`, `nltk`, `re`, `string`
- `matplotlib`, `wordcloud`
- `sklearn`: for ML models and evaluation
- `xgboost`
- `tensorflow`, `keras`: for LSTM model

---

## 🚀 How to Run

1. Upload `Twitter_Dataset.csv` to your Colab/working directory.
2. Open `Twitter_Analysis.ipynb` in Google Colab or Jupyter Notebook.
3. Run the cells step by step to:
   - Preprocess the text
   - Train multiple models
   - Compare their performance

---

## 📌 Notes

- The dataset is large (~227 MB). Consider uploading it to Google Drive and referencing the path from Colab.
- Adjust the number of training samples if running on limited hardware (e.g., in Colab free tier).

