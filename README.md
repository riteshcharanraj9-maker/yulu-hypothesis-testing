<h1 align='center'> 🚲 YULU - Business Case Study 🚲 </h1>
<h2 align='center'> Hypothesis Testing </h2>
<h3 align='right'>Analysed by : <b>Ritesh Charan Raj</b></h3>

---

## 📝 Case Report

- Access the complete Python notebook here  
➡️ [Python Notebook](Ritesh_Yulu_Business_case_study.ipynb)

- Access the complete case study report here  
➡️ [Project Report](Ritesh_Yulu_Business_case_study_Colab.pdf)

---

# 📌 Business Problem

Yulu is a micro-mobility service that provides shared electric bikes for urban transportation.  
The company wants to understand the factors affecting bike rental demand.

By analyzing the dataset, we aim to identify whether variables such as **working day, weather conditions, and seasons** influence the number of bike rentals.

---

# 🎯 Objective

The goal of this project is to:

- Perform exploratory data analysis (EDA)
- Understand patterns in bike rentals
- Conduct statistical hypothesis testing
- Determine factors that influence bike rental demand

---

# 📊 Dataset Overview

The dataset contains **10886 rows and 12 columns** of bike rental information. :contentReference[oaicite:2]{index=2}

Key variables include:

| Feature | Description |
|-------|-------------|
| datetime | Timestamp of bike rental |
| season | Season of the year |
| holiday | Whether the day is a holiday |
| workingday | Whether it is a working day |
| weather | Weather condition |
| temp | Temperature |
| atemp | Feels-like temperature |
| humidity | Humidity level |
| windspeed | Wind speed |
| casual | Casual users |
| registered | Registered users |
| count | Total bike rentals |

---

# 🔎 Exploratory Data Analysis

Key observations from EDA:

- Dataset does **not contain missing values**.
- The total rental count is the **sum of casual and registered users**.
- Temperature and apparent temperature show strong correlation.
- Humidity has a **negative relationship with bike rentals**.
- Registered users contribute significantly more to total rentals.

---

# 📈 Statistical Tests Performed

The following hypothesis tests were conducted:

### 1️⃣ Shapiro-Wilk Test
Used to test whether the data follows a normal distribution.

Result:
The p-value is **less than 0.05**, indicating the data is **not normally distributed**.

---

### 2️⃣ Levene's Test
Used to test equality of variances between groups.

Result:
The p-value is **greater than 0.05**, indicating the variances are approximately equal.

---

### 3️⃣ Independent T-Test
Used to check if there is a difference in bike rentals between working and non-working days.

Result:
The p-value is **greater than 0.05**, indicating **no significant difference in rentals between working days and non-working days**.

---

### 4️⃣ ANOVA Test
Used to test whether bike rental demand differs across weather conditions.

This helps determine whether weather has a statistically significant impact on rentals.

---

# 📊 Key Insights

- Summer months show higher bike rental demand.
- Temperature positively influences bike rentals.
- High humidity negatively affects rental demand.
- Registered users contribute the majority of rentals.
- Working day vs non-working day does not show a statistically significant difference in rentals.

---

# 🛠 Tools & Technologies Used

Python  
Pandas  
NumPy  
Seaborn  
Matplotlib  
SciPy  
Statsmodels  

---

# 📂 Repository Structure
