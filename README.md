📊 Car Price Data Cleaning & Analysis
📌 Project Overview

This project focuses on data cleaning and exploratory data analysis (EDA) of a car price dataset. The goal is to preprocess raw data, handle inconsistencies, and perform statistical analysis to extract meaningful insights about factors affecting car prices.

📂 Dataset
->Dataset used: CarPrice_Assignment.csv
->Contains information about:
->Car features
->Fuel type
->Price
->Other specifications

⚙️ Technologies Used
Python
->Pandas – Data manipulation
->NumPy – Numerical operations
->Matplotlib & Seaborn – Data visualization
->SciPy – Statistical testing

🧹 Data Cleaning Steps

The following preprocessing steps were performed:

✅ Loaded dataset using Pandas
✅ Checked dataset structure (head, tail, info)
✅ Removed duplicate records
✅ Checked for missing values
✅ Verified data types
✅ Performed statistical summary using describe()

📊 Exploratory Data Analysis (EDA)
1. Distribution Analysis
Visualized the distribution of car prices
Observed that the data was not normally distributed
2. Data Transformation

Applied log transformation:

df['log_price'] = np.log(df['price'])
Result:
Improved distribution
Reduced skewness

📈 Statistical Analysis
🔍 Hypothesis Testing (T-Test)

Objective:
Check whether fuel type affects car price.

Null Hypothesis (H₀): No difference in price
Alternative Hypothesis (H₁): There is a difference

Test Used: Independent T-Test

from scipy.stats import ttest_ind

Result:

If p < 0.05 → Reject H₀
Concluded that fuel type impacts car price

📌 Key Insights
Car prices are right-skewed (not normally distributed)
Log transformation helps in normalization
Fuel type (gas vs diesel) significantly affects price
Clean data improves reliability of analysis

🎯 Future Improvements
Feature engineering
Outlier detection & handling
Machine learning model for price prediction
Advanced visualization dashboards
🙌 Conclusion

This project demonstrates the importance of:

Proper data cleaning
Understanding data distribution
Applying statistical tests to validate assumptions
