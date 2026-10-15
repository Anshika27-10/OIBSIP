# 📊 Unemployment Analysis with Python

## 📌 Project Overview

Unemployment Analysis with Python is a data analysis project that explores unemployment trends across different regions of India, with a special focus on the impact of the COVID-19 pandemic.

The project uses Exploratory Data Analysis (EDA) to identify regional differences, monthly trends, relationships between employment indicators, and changes in unemployment rates before and after the onset of COVID-19.

## 🎯 Objectives

- Analyze unemployment rates across different Indian states and regions.
- Identify monthly and time-based unemployment trends.
- Visualize unemployment trends for selected states.
- Identify the top 10 regions with the highest average unemployment rates.
- Examine correlations between unemployment rate, estimated employment, and labour participation rate.
- Compare employment indicators before and after the onset of COVID-19.
- Present insights using data visualizations.

## 🛠️ Technologies Used

- **Python** – Data analysis and programming
- **Pandas** – Data manipulation and cleaning
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Jupyter Notebook** – Interactive development and analysis

## 📂 Project Structure

```text
Unemployment-Analysis/
│
├── unemployment_analysis.ipynb
├── Unemployment in India.csv
├── README.md
└── requirements.txt
```

*Note: The dataset filename and notebook filename may differ depending on your downloaded files.*

## 📁 Dataset

The project uses the **Unemployment in India** dataset, which contains unemployment and labour-market indicators for different regions of India.

### Dataset Features

| Column | Description |
|---|---|
| Region | Indian state or region |
| Date | Date of observation |
| Frequency | Reporting frequency |
| Estimated Unemployment Rate (%) | Estimated unemployment percentage |
| Estimated Employed | Estimated number of employed people |
| Estimated Labour Participation Rate (%) | Estimated labour participation percentage |

### Download the Dataset

1. Visit [Kaggle Datasets](https://www.kaggle.com/datasets).
2. Search for **Unemployment in India**.
3. Open a suitable dataset and download the ZIP file.
4. Extract the ZIP file.
5. Place the CSV file in the project directory.

Make sure the CSV filename in your notebook matches the actual downloaded filename.

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Unemployment-Analysis.git
```

### 2. Navigate to the Project Directory

```bash
cd Unemployment-Analysis
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

Alternatively, install the required libraries directly:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `unemployment_analysis.ipynb` and run the cells in order.

## 🔍 Project Workflow

### 1. Data Loading and Inspection
- Load the dataset using Pandas.
- Inspect the number of rows and columns.
- Review column names, data types, and descriptive statistics.
- Identify missing values.

### 2. Data Cleaning and Preprocessing
- Remove unnecessary spaces from column names.
- Handle missing values appropriately.
- Convert the date column into a datetime format.
- Create additional time-based columns for analysis.

### 3. Exploratory Data Analysis
- Calculate average unemployment rates by region.
- Analyze monthly unemployment patterns.
- Visualize unemployment rates over time for selected states.
- Identify the 10 regions with the highest average unemployment rates.

### 4. Correlation Analysis
- Calculate correlations between unemployment rate, estimated employment, and labour participation rate.
- Display the relationships using a correlation heatmap.
- Interpret the strength and direction of the relationships.

### 5. COVID-19 Impact Analysis
- Divide observations into pre-COVID and COVID/post-COVID periods.
- Calculate average unemployment, employment, and labour participation rates for both periods.
- Compare the results using bar charts and time-series visualizations.

**Period definition:** Pre-COVID is defined as dates before March 2020, while COVID/post-COVID includes March 2020 onwards. These are analytical periods, not a claim that every observation after March 2020 reflects the same pandemic conditions.

## 📈 Key Visualizations

The project includes the following visualizations:

- **Region-wise Bar Chart:** Compares average unemployment rates across regions.
- **Monthly Trend Line Chart:** Shows how unemployment varies by month.
- **Time-Series Line Chart:** Compares unemployment trends across at least three selected states or regions.
- **Top 10 Bar Chart:** Highlights regions with the highest average unemployment rates.
- **Correlation Heatmap:** Shows relationships among key employment indicators.
- **COVID-19 Comparison Chart:** Compares average indicators before and after March 2020.
- **Overall Time-Series Chart:** Displays changes in unemployment over the study period.

Each visualization is accompanied by written observations to explain the patterns and trends found in the data.

## 💡 Expected Insights

The analysis aims to identify:

- Regional variations in unemployment rates across India.
- Changes in unemployment over time and across months.
- Regions with relatively high average unemployment rates.
- Relationships between unemployment, employment, and labour participation.
- Differences in employment indicators between the pre-COVID and COVID/post-COVID periods.

Actual findings should be reported after running the notebook on the selected dataset. Results may vary depending on the dataset version, coverage, and preprocessing decisions.

## 📊 Results and Conclusion

This project demonstrates how Python-based data analysis can be used to investigate unemployment patterns and visualize economic indicators.

By combining data cleaning, exploratory analysis, statistical summaries, and visualization, the project provides a structured approach to understanding regional and temporal unemployment trends in India.

The analysis can support further investigation into labour-market changes, but the observed associations alone cannot establish that COVID-19 caused a particular change in unemployment.

## 🚀 Future Enhancements

- Build an interactive dashboard using Streamlit or Plotly.
- Add state-wise comparisons with interactive filters.
- Extend the analysis using more recent and additional labour-market datasets.
- Apply statistical tests to evaluate differences between periods.
- Develop a forecasting model to estimate future unemployment trends.

## 👩‍💻 Skills Demonstrated

- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- Statistical Analysis
- Time-Series Analysis
- Data Visualization
- Python Programming
- Data Interpretation and Reporting

## 📜 License

This project is intended for educational and portfolio purposes. Check the original dataset's license and usage conditions before redistributing the dataset.

## 🙌 Acknowledgements

- Kaggle for dataset discovery and access.
- The Python, Pandas, Matplotlib, and Seaborn communities for their documentation and tools.
