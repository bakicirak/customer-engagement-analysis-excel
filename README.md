# Customer Engagement Analysis in Excel

This project analyzes student engagement data for the 365 company using Microsoft Excel. The analysis compares Q4 2021 and Q4 2022 engagement levels to evaluate whether new platform features introduced in 2022 (XP system, coins, leaderboard, streaks, expanded course library) contributed to increased user activity.

## 📁 Folder Structure

- `data.xlsx`: Contains the original dataset file.
- `Engagement_Project.xlsx`: Excel files with calculations and results per task.
- `README.md`: Project summary and instructions.

---

## 📊 Dataset Overview

The dataset includes anonymized data for students with free and paid accounts who used the platform in:
- **Q4 2021 (Oct 1 – Dec 31, 2021)**
- **Q4 2022 (Oct 1 – Dec 31, 2022)**

### Columns:
- `student_id`: Unique identifier
- `student_country`: Country of origin
- `paid`: 1 = Paid plan, 0 = Free plan
- `minutes_watched_21`: Minutes watched in Q4 2021
- `minutes_watched_22`: Minutes watched in Q4 2022

---

## 🔍 Project Tasks

### Task 1: Descriptive Statistics
- Focused on students with **1–100 minutes watched in Q4 2021**
- Compared engagement levels in 2021 vs. 2022 for recurring students
- Summary statistics: mean, median, and standard deviation
- Compared results by subscription type (free vs paid)

### Task 2: Skewness and Kurtosis
- Calculated skewness and kurtosis of engagement distributions for both years
- Compared results across free and paid students
- Interpreted whether distributions aligned with earlier statistics

### Task 3: Confidence Intervals
- Calculated 95% confidence intervals for:
  - Free users in 2021 and 2022
  - Paid users in 2021 and 2022
- Used **z-statistics** with assumed normal distribution
- Drew conclusions about engagement patterns between years

### Task 4: Hypothesis Testing
- Null hypothesis: Q4 2021 engagement ≥ Q4 2022
- Alternative hypothesis: Q4 2022 engagement > Q4 2021
- Conducted two-sample t-tests assuming unequal variances
- Degrees of freedom:
  - Free-plan students: **40,836**
  - Paid-plan students: **8,229**
- Discussed potential business impact of Type I and Type II errors

### Task 5: Regional Engagement Comparison
- Compared **free-plan students in the US vs. India** in 2022
- Null hypothesis: US engagement ≥ India
- Alternative hypothesis: US engagement < India
- Used a two-sample t-test assuming unequal variances
- Degrees of freedom: **11,001**
- Helped guide regional product strategy based on student usage

---

## 🧰 Tools Used

- **Microsoft Excel**: For descriptive stats, confidence intervals, hypothesis testing
- **Basic statistical concepts**: Mean, median, standard deviation, skewness, kurtosis
- **T-tests**: To compare engagement levels across years and countries

---

## 📎 Files To Include

- `data.xlsx` — the original dataset
- `Engagement_Project.xlsx` — each Excel file for the individual tasks

---

