# 📩 Email/SMS Spam Detection with Machine Learning

## 📌 Project Overview

This project uses Natural Language Processing (NLP) and Machine Learning to classify text messages as **Spam** or **Ham (Legitimate)**. It applies text preprocessing and TF-IDF feature extraction to convert text into numerical features, then trains and evaluates two classification models.

The project demonstrates how machine learning can help identify unwanted messages and reduce the risk of spam reaching users.

## 🎯 Objectives

- Build a binary text classification model for spam detection.
- Perform text preprocessing to clean raw messages.
- Convert text into numerical features using TF-IDF.
- Train and compare two machine learning algorithms.
- Evaluate models using standard classification metrics.
- Visualize class distribution, confusion matrices, and common words.
- Predict whether a new message is spam or legitimate.

## 🛠️ Tech Stack

- **Language:** Python
- **Data Processing:** pandas, NumPy
- **Machine Learning:** scikit-learn
- **NLP:** Regular Expressions (re), NLTK
- **Data Visualization:** Matplotlib
- **Bonus Visualization:** WordCloud
- **Development Environment:** Jupyter Notebook

## 📂 Dataset

This project uses the **SMS Spam Collection Dataset**, a publicly available dataset containing labeled SMS messages.

Each message belongs to one of two classes:

- `spam` — Unwanted or suspicious messages.
- `ham` — Legitimate messages.

**Dataset sources:**
- [UCI Machine Learning Repository – SMS Spam Collection](https://archive.ics.uci.edu/dataset/228/sms+spam+collection)
- [Kaggle – SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)

Download the dataset and place the CSV file in the project directory. The notebook should be configured to match the downloaded file's name and column structure.

## ⚙️ Project Workflow

### 1. Data Loading and Exploration
- Load the dataset using pandas.
- Inspect rows, columns, and missing values.
- Identify and remove duplicate records.
- Analyze the distribution of spam and ham messages.

### 2. Text Preprocessing
- Convert text to lowercase.
- Remove URLs and punctuation.
- Remove numbers and extra whitespace.
- Optionally remove English stopwords using NLTK.

### 3. Feature Extraction Using TF-IDF

TF-IDF (Term Frequency–Inverse Document Frequency) converts text into numerical vectors that machine learning models can process. It assigns importance to words based on their frequency in a message and their rarity across the dataset.

The project uses `TfidfVectorizer` with a maximum of 5,000 features and unigrams and bigrams.

### 4. Train-Test Split
Split the dataset into:
- **80% training data**
- **20% testing data**

Stratified splitting helps preserve the original class distribution in both sets.

### 5. Model Training

Two classification algorithms are trained:

- **Multinomial Naive Bayes:** A probabilistic classifier commonly used for text classification.
- **Logistic Regression:** A linear classification algorithm used to predict the probability of a message belonging to a class.

### 6. Model Evaluation

Evaluate both models using:

- **Accuracy:** Overall proportion of correct predictions.
- **Precision:** Proportion of predicted spam messages that are actually spam.
- **Recall:** Proportion of actual spam messages correctly detected.
- **F1-score:** Harmonic mean of precision and recall.
- **Confusion Matrix:** Shows correct and incorrect predictions for each class.

### 7. Visualization
- Spam versus ham class distribution.
- Confusion matrices for both classifiers.
- Model performance comparison.
- WordClouds for common words in spam and ham messages.

### 8. Custom Message Prediction

The trained model can classify a new message as `SPAM` or `HAM` using the same text preprocessing and TF-IDF transformation applied during training.

## 📊 Why Is Recall Important?

Recall is especially important in spam detection because it measures how many actual spam messages the model successfully identifies.

A false negative occurs when a spam message is classified as legitimate, allowing unwanted or potentially fraudulent content to pass through.

However, precision is also important because low precision can cause legitimate messages to be incorrectly marked as spam. A good spam detection system should balance these two metrics according to its intended use.

## 🚀 Installation and Setup

### Prerequisites

Install Python and Jupyter Notebook, then install the required libraries.

```bash
pip install pandas numpy scikit-learn matplotlib nltk wordcloud jupyter
```

### Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

Navigate to the project directory:

```bash
cd YOUR_REPOSITORY
```

### Download the Dataset

Download the SMS Spam Collection dataset from one of the sources listed above and place the CSV file in the project directory.

For the common Kaggle CSV format, the notebook may need to select the `v1` and `v2` columns and rename them to `label` and `message`.

### Run the Notebook

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open the project notebook and execute the cells in order, from data loading through model evaluation and custom prediction.

## 📁 Suggested Project Structure

```text
Email-SMS-Spam-Detection/
│
├── spam_detection.ipynb
├── spam.csv
├── README.md
└── requirements.txt
```

*Note: `spam.csv` is the downloaded dataset and does not need to be committed to GitHub if you prefer to keep the repository lightweight.*

## 🔍 Example Predictions

| Message | Expected Classification |
|---|---|
| Congratulations! You have won a free prize. Click now! | SPAM |
| Hey, are we meeting for lunch today? | HAM |
| URGENT! You won a cash reward! | SPAM |
| Can you send me the assignment? | HAM |

*These are illustrative examples. Actual predictions depend on the trained model and its learned patterns.*

## 📈 Results

The notebook reports accuracy, precision, recall, and F1-score for both models, along with their confusion matrices.

Record the actual evaluation results produced by your notebook here after running the experiments.

| Model | Accuracy | Precision | Recall | F1-score |
|---|---:|---:|---:|---:|
| Multinomial Naive Bayes | To be measured | To be measured | To be measured | To be measured |
| Logistic Regression | To be measured | To be measured | To be measured | To be measured |

The best model should be selected based on the evaluation metrics and the relative cost of missed spam versus incorrectly flagged legitimate messages.

## 🌟 Key Learnings

- Text cleaning and preprocessing for NLP.
- Feature extraction using TF-IDF.
- Training supervised machine learning classifiers.
- Comparing classification algorithms.
- Evaluating imbalanced classification tasks.
- Understanding precision, recall, and F1-score.
- Visualizing model performance and word frequencies.
- Applying a trained model to new text messages.

## 🔮 Future Improvements

- Add Support Vector Machine (SVM) for further model comparison.
- Apply stemming or lemmatization.
- Tune hyperparameters using cross-validation.
- Handle class imbalance where necessary.
- Save the trained model and vectorizer for reuse.
- Build an interactive web interface using Flask or Streamlit.
- Extend the system to email datasets and evaluate performance on real-world email content.

## 👩‍💻 Author

**Anshika Jain**

Computer Science Engineering – Data Science

Acropolis Institute of Technology and Research, Indore

## 📄 License

This project is intended for educational and learning purposes. Check the dataset's license and terms before redistributing the dataset or using it commercially.
