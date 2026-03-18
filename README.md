#  Airbnb Listings Data Analysis Project

##  Project Overview

This project performs an **end-to-end Exploratory Data Analysis (EDA)** on an Airbnb listings dataset to understand pricing patterns, demand, and factors affecting listing performance.

The analysis follows a structured data analysis workflow including **data profiling, cleaning, visualization, statistical analysis, and feature engineering**.

---

## Tech Stack

- **Python:** Pandas, NumPy  
- **Visualization:** Matplotlib, Seaborn  
- **Statistics:** SciPy  
- **Environment:** Jupyter Notebook  

---

##  Project Workflow

### Day 1: Data Understanding & Profiling

- Loaded dataset and inspected structure (`shape`, `info`, `describe`)
- Identified numerical, categorical, and date columns
- Detected missing values in:
  - `last_review`
  - `reviews_per_month`
- Observed extreme values in the `price` column

---

### Day 2: Data Cleaning & Preprocessing

- Converted `last_review` to datetime
- Handled missing values:
  - `reviews_per_month` → filled with **0**
  - Text columns → filled with **"unknown"**
- Removed extreme price outliers using the **IQR method**
- Created **log_price** to reduce skewness
- Standardized categorical values

---

### Day 3: Visual Exploration (EDA)

#### Univariate Analysis

- Price distribution is **heavily right-skewed**
- Majority of listings are **low to mid-priced**
- Entire homes and private rooms **dominate the market**

#### Bivariate Analysis

- Entire homes have **higher prices**
- Private rooms receive **more reviews (higher demand)**
- Some locations have **significantly higher prices**
- Weak correlation between **price and numeric features**

---

### Day 4: Statistical Testing & Feature Engineering

#### Feature Engineering

Created new variables:

- `host_type`
- `price_per_review`
- Time-based features from review dates

#### Statistical Tests

- **T-Test:** Entire homes cost significantly more than private rooms *(p < 0.05)*
- **ANOVA:** Price differs significantly across locations *(p < 0.05)*
- **Chi-Square:** Room type distribution varies by location

---

##  Key Business Insights

- **Location drives pricing:** Certain neighbourhoods are significantly more expensive
- **Entire homes generate the highest revenue but receive fewer bookings**
- **Affordable listings receive more reviews**, indicating higher demand
- **High prices reduce booking frequency**
- **Private rooms dominate booking volume**
- **Price distribution shows most listings fall within an affordable range**

---

##  Conclusion

This project demonstrates a complete **real-world data analysis workflow**:

- Data understanding  
- Cleaning & preprocessing  
- Visual exploration  
- Statistical validation  
- Business insights  

The findings help Airbnb hosts and analysts make informed decisions about:

- Pricing strategy  
- Location targeting  
- Room type selection  
- Demand patterns  

---

###  Final Output

Actionable insights for improving **Airbnb listing performance and pricing strategy**.
