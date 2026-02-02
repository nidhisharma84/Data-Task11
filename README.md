# Task 11: A/B Testing — Hypothesis Testing in Python

## 📌 Objective

The goal of this task is to perform **A/B testing** on an e-commerce marketing dataset to determine whether a new version (Test group) performs better than the old version (Control group) in terms of conversion rate.

This task demonstrates the ability to make **data-driven business decisions** using statistical hypothesis testing.

---

## 🛠 Tools & Technologies Used

* **Google Colab** (Python environment)
* **Python Libraries**:

  * pandas
  * numpy
  * scipy
  * matplotlib

---

## 📁 Dataset Description

**File:** `ab_test_data.csv`

| Column Name | Description                       |
| ----------- | --------------------------------- |
| user_id     | Unique user identifier            |
| group       | control or test group             |
| converted   | 1 = conversion, 0 = no conversion |

The dataset contains **100 users**:

* 50 users in the **control group**
* 50 users in the **test group**

---

## 🧪 A/B Testing Methodology

### 1️⃣ Hypothesis Definition

* **H0 (Null Hypothesis):** Conversion rate of control group = conversion rate of test group
* **H1 (Alternative Hypothesis):** Conversion rate of control group ≠ conversion rate of test group
* **Significance Level (α):** 0.05

---

### 2️⃣ Metric Used

* **Conversion Rate** = Mean of the `converted` column

---

### 3️⃣ Statistical Test Used

* **Chi-Square Test of Independence**

**Reason:**

* Data is categorical (converted: yes/no)
* Two independent groups (control vs test)

---

### 4️⃣ Confidence Interval

A 95% confidence interval was calculated to estimate the range in which the true difference in conversion rates lies.

---

### 5️⃣ Visualization

A bar chart was created to compare conversion rates between the control and test groups.

---

## 📊 Results Summary

| Group   | Conversion Rate |
| ------- | --------------- |
| Control | ~30%            |
| Test    | ~70%            |

* **p-value < 0.05**
* The difference between groups is **statistically significant**

---

## ✅ Final Decision

The null hypothesis is **rejected**.

---

## 💼 Business Recommendation

The **test version performs significantly better** than the control version.

👉 It is recommended to **implement the test version** to improve overall conversion rates and business performance.

---

## 📦 Deliverables

* `task11_abtest.ipynb` → Jupyter Notebook with full analysis
* `ab_test_summary.csv` → Conversion rate summary
* `final_recommendation.txt` → Business decision & recommendation
* `README.md` → Project documentation

---

## 🎯 Key Learnings

* Understanding hypothesis testing
* Choosing the correct statistical test
* Interpreting p-values and confidence intervals
* Translating statistical results into business decisions

**Sneha Singh**
Data Analyst Intern
