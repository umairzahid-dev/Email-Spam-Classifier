# Email Spam Classification

A machine learning project that classifies emails as **Spam** or **Ham (Not Spam)** using Natural Language Processing (NLP) techniques and the **Multinomial Naive Bayes** algorithm.

The project includes text preprocessing, feature extraction using TF-IDF, model training, evaluation, visualization, and model persistence using Pickle.

---

## Project Overview

Email spam detection is one of the most common applications of machine learning in cybersecurity and communication systems. This project builds an automated classifier capable of identifying unwanted spam emails from legitimate emails.

The workflow includes:

* Data Cleaning
* Text Preprocessing
* Feature Engineering
* TF-IDF Vectorization
* Model Training
* Performance Evaluation
* Model Saving

---

## Dataset

**Source:** Kaggle

**Dataset:** Ling Spam Dataset

https://www.kaggle.com/datasets/rtatman/ling-spam-dataset

### Dataset Information

* Real email messages
* Spam and Ham labels
* Text-based email content
* Suitable for NLP and text classification tasks

After preprocessing and duplicate removal:

* Total Emails: 5,695

---

## Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* NLTK
* Scikit-learn
* Matplotlib
* Seaborn
* Pickle

---

## Project Workflow

### 1. Data Preprocessing

The following preprocessing steps were applied:

* Convert text to lowercase
* Remove "Subject:" prefixes
* Remove URLs
* Remove HTML tags
* Remove punctuation
* Tokenization
* Stopword removal
* Porter stemming

---

### 2. Feature Engineering

Additional features were generated for analysis:

* Character Count
* Word Count
* Sentence Count

---

### 3. Feature Extraction

TF-IDF Vectorization was used to convert email text into numerical representations.

```python
TfidfVectorizer(max_features=5000)
```

---

### 4. Model Training

Algorithm Used:

```text
Multinomial Naive Bayes
```

Dataset Split:

```text
80% Training
20% Testing
```

---

## Results

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 98.07% |
| Precision | 98.06% |
| Recall    | 93.70% |
| F1 Score  | 95.83% |

The model achieved strong performance in detecting spam emails while maintaining high precision and overall classification accuracy.

---

## Visualizations

The project includes:

* Spam vs Ham Distribution
* Confusion Matrix

---

## Model Persistence

The trained model and TF-IDF vectorizer are saved using Pickle.

Generated files:

```text
spam_classifier.pkl
tfidf_vectorizer.pkl
```

These files allow predictions without retraining the model.

---


---

## Project Structure

```text
Email-Spam-Classification/
│
├── emails.csv
├── Email_Spam_Classification.ipynb
├── spam_classifier.pkl
├── tfidf_vectorizer.pkl
├── README.md
```
## Author

Umair Zahid


LinkedIn: https://www.linkedin.com/in/umair-zahid-b23444252/
