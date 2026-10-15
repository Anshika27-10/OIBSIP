# Sales Prediction Using Python 📊

## 📌 Project Overview

This project uses Machine Learning and Regression techniques to predict product sales based on advertising expenditure across three media channels: **TV, Radio, and Newspaper**.

The project explores the relationship between advertising budgets and sales, performs Exploratory Data Analysis (EDA), trains multiple regression models, and compares their performance using evaluation metrics.

## 🎯 Objectives

- Analyze the relationship between advertising expenditure and product sales.
- Perform Exploratory Data Analysis (EDA) using statistical summaries and visualizations.
- Build a Linear Regression model as a baseline.
- Train a Random Forest Regressor for comparison.
- Evaluate models using MAE, RMSE, and R² score.
- Identify the most influential advertising channel.
- Visualize prediction errors using residual plots.

## 🛠️ Technologies Used

- **Python** — Programming language
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical computations
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization
- **Scikit-learn** — Machine Learning and model evaluation
- **Jupyter Notebook** — Development environment

## 📂 Dataset

The project uses the classic `Advertising.csv` dataset, which contains advertising expenditure and sales data.

**Features:**

| Column | Description |
|---|---|
| `TV` | Advertising expenditure on TV |
| `Radio` | Advertising expenditure on Radio |
| `Newspaper` | Advertising expenditure on Newspaper |
| `Sales` | Product sales (target variable) |

The dataset typically contains 200 observations.

**Dataset source:** [Search for Advertising Sales Prediction datasets on Kaggle](https://www.kaggle.com/search?q=advertising+sales+prediction+dataset)

Download the CSV file and place it in the project directory.

## 📁 Project Structure

```text
Sales-Prediction/
│
├── Advertising.csv
├── Sales_Prediction.ipynb
└── README.md
```

*Note: Your notebook filename may differ depending on how you saved it.*

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/your-username/Sales-Prediction.git
```

### 2. Navigate to the project directory

```bash
cd Sales-Prediction
```

### 3. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `Sales_Prediction.ipynb` and execute the cells in order.

## 🔍 Project Workflow

### 1. Data Loading and Inspection
- Load the dataset using Pandas.
- Inspect the dataset structure and column names.
- Check for missing values and duplicate records.
- Generate descriptive statistics.

### 2. Exploratory Data Analysis (EDA)
- Create pairplots to visualize relationships among features.
- Plot Sales against TV, Radio, and Newspaper advertising expenditure.
- Generate a correlation matrix and heatmap.

### 3. Data Preparation
- Select TV, Radio, and Newspaper as input features.
- Select Sales as the target variable.
- Split the dataset into training and testing sets using an 80:20 ratio.

### 4. Model Training

**Linear Regression:** Used as the baseline model to learn the relationship between advertising expenditure and sales.

**Random Forest Regressor:** Used as an additional model to capture potentially nonlinear relationships.

### 5. Model Evaluation

The models are evaluated using the following metrics:

| Metric | Purpose |
|---|---|
| MAE | Measures average absolute prediction error |
| RMSE | Penalizes larger prediction errors more strongly |
| R² Score | Measures how much variation in sales is explained by the model |

Lower MAE and RMSE values indicate smaller prediction errors, while a higher R² score generally indicates a better fit.

### 6. Model Comparison
- Compare Linear Regression and Random Forest results.
- Identify the better-performing model based on test-set metrics.
- Visualize model performance.

### 7. Feature Importance
- Analyze Linear Regression coefficients.
- Examine Random Forest feature importance.
- Identify which advertising channel contributes most to the model's predictions.

### 8. Residual Analysis
- Plot residuals against predicted sales.
- Check for patterns that may indicate systematic prediction errors.
- Compare actual sales with predicted sales.

### 9. Sales Prediction
Use the trained model to predict sales for new advertising budgets across TV, Radio, and Newspaper.

## 📈 Expected Results

The analysis is expected to show that:

- TV advertising has a strong positive relationship with sales.
- Radio advertising also provides useful predictive information.
- Newspaper advertising generally has a weaker relationship with sales than TV and Radio.
- Model performance depends on the algorithm and test data.

The actual evaluation scores and the best-performing model should be reported using the results produced by your notebook rather than assumed in advance.

## 💡 Key Learnings

- Understanding regression-based Machine Learning.
- Performing EDA and interpreting correlation.
- Splitting data into training and testing sets.
- Training and comparing regression models.
- Evaluating predictions using MAE, RMSE, and R².
- Interpreting model coefficients and feature importance.
- Analyzing residuals to identify model limitations.

## 🚀 Future Improvements

- Experiment with Polynomial Regression and other regression algorithms.
- Perform cross-validation and hyperparameter tuning.
- Build an interactive sales prediction application using Flask or Streamlit.
- Add more business-related features to improve predictive performance.
- Deploy the trained model as a web application.

## 📝 Conclusion

This project demonstrates how Machine Learning regression techniques can be used to predict product sales from advertising expenditure. Exploratory Data Analysis helps reveal relationships between advertising channels and sales, while model evaluation helps determine which approach provides better predictions.

The findings can support data-driven analysis of advertising budgets, although the observed relationships alone do not establish that advertising expenditure causes changes in sales.

## 👩‍💻 Author

**Anshika Jain**

Aspiring Software Engineer | Data Science & Machine Learning Enthusiast

