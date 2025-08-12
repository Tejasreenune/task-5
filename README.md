# Titanic Survival Analysis – Exploratory Data Analysis (EDA)  

## 📌 Objective  
The goal of this project is to analyze the Titanic dataset to extract insights, identify trends, and explore key factors affecting passenger survival using **Exploratory Data Analysis (EDA)** techniques in Python.  
`
---

## 📂 Dataset  
- **Source:** [Kaggle – Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic)  
- **File Used:** `train.csv` – Training dataset containing passenger demographics, travel details, and survival status.
  


## 🛠 Tools & Libraries Used  
- **Python** (Google Colab / Jupyter Notebook)  
- **Pandas** – Data manipulation  
- **Matplotlib** & **Seaborn** – Data visualization  

---

## 📊 Steps Performed  

1. **Data Loading**  
   - Imported `train.csv` into Google Colab using Pandas.  

2. **Data Cleaning**  
   - Handled missing values in `Age` (filled with median) and `Embarked` (filled with mode).  
   - Noted high missing percentage in `Cabin`, so it was excluded from analysis.  

3. **Exploratory Data Analysis (EDA)**  
   - Generated statistical summaries using `.describe()`, `.info()`, and `.value_counts()`.  
   - Created visualizations for:  
     - Univariate Analysis - Survival count, Age distribution, Passenger class count, Gender distribution.
     - Bivariate Analysis - Survival by gender, Survival by passenger class, Age vs survival (boxplot).
     - Multivariate Analysis -  Correlation heatmap, Pairplot.
   - Used **`sns.pairplot()`** and **`sns.heatmap()`** for correlation checks.  
   - Identified relationships and trends in the dataset.  

4. **Observations & Insights**  
   - Survival strongly influenced by gender, passenger class, and fare paid.  
   - Women and children had higher survival chances compared to men.  
   - Higher-class passengers (especially 1st class) survived at greater rates than lower-class passengers.  
   - Higher fares correlated with better survival rates, indicating socio-economic impact.  

---

## 📈 Key Survival Statistics  

| Feature          | Category     | Survival Rate (%) | Count         |
|------------------|-------------|-------------------|--------------|
| Overall          | All         | 38.38%            | 342 / 891    |
| Gender           | Female      | 74.20%            | 233 / 314    |
|                  | Male        | 18.89%            | 109 / 577    |
| Passenger Class  | 1st Class   | 62.96%            | 136 / 216    |
|                  | 2nd Class   | 47.28%            | 87 / 184     |
|                  | 3rd Class   | 24.24%            | 119 / 491    |
| Age Group        | <18 years   | 51.08%            | 61 / 119     |
|                  | ≥18 years   | 36.19%            | 281 / 772    |

---

## 📝 Conclusion  
The analysis clearly shows that **gender, socio-economic status, and age group** played a significant role in survival probability on the Titanic. Women, children, and wealthier passengers had better survival rates. Handling missing data ensured a clean dataset for accurate analysis. Overall survival stood at approximately **38%**.  


##Author
Tejasree Nune
