# 🛒 Rossmann Store Sales Forecasting
This project aims to forecast daily sales for Rossmann drug stores using historical data and store-related information. The dataset contains sales records from over 1,000 stores across several European countries, capturing trends influenced by promotions, holidays, customer behavior, and local competition.

# 📌 Problem Statement
Rossmann store managers must forecast daily sales up to six weeks in advance to plan resources effectively. This project provides a machine learning solution to automate and improve the accuracy of these predictions.

# 📁 Dataset Overview
The dataset includes:

Store, Date, Sales, Customers, Open

Holiday info: StateHoliday, SchoolHoliday

Store characteristics: StoreType, Assortment, CompetitionDistance, Promo, Promo2, etc.

Our target variable is Sales, which we aim to predict.

# 🔍 Exploratory Data Analysis (EDA)
EDA was performed to:

Understand the distribution of sales and customers.

Examine the effect of holidays, promotions, and store types.

Visualize missing data and anomalies (e.g., closed stores).

# ⚙️ Feature Engineering & Selection
Key engineered features:

Date decomposition: extracting year, month, day, week, etc.

Promo timelines: encoded intervals and durations since promos started.

Competition factors: computed how long a nearby competitor has been open.

Feature selection was done using correlation analysis and importance scores from tree-based models.

# 🤖 Models Used
Several regression models were tested:

* Random Forest Regressor (best performance)

* Decision Tree

* Linear Regression (baseline)

* Gradient Boosting

Evaluation was based on RMSE and visual inspection of prediction trends.

# 🏁 Conclusion
Random Forest performed the best, effectively capturing non-linear relationships and categorical variables.

Promo campaigns and competition distance had a significant impact on sales.

Feature engineering notably improved performance by highlighting temporal and promotional patterns.

# 🛠️ Tools & Libraries
Python, Pandas, NumPy, Matplotlib, Seaborn

Scikit-learn, XGBoost

Jupyter Notebook
