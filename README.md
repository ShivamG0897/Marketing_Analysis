# 📊 Marketing Analysis

## 📝 Problem Scenario
**Marketing mix** is a popular concept used in implementing marketing strategies.  
It revolves around the **four Ps** of marketing:
1. **Product**
2. **Price**
3. **Place**
4. **Promotion**

---

## 🎯 Problem Objective
As a **data scientist**, the goal is to:
- Perform **exploratory data analysis (EDA)**.
- Conduct **hypothesis testing**.
- Gain a better understanding of the various factors contributing to **customer acquisition**.

---

## 📂 Data Description
The dataset includes variables mapped to the 4Ps:

| Category  | Example Variables |
|-----------|------------------|
| **People** | `birth-year`, `education`, `income`, etc. |
| **Product** | Amount spent on `wine`, `fruits`, `gold`, etc. |
| **Place** | Sales channel information: `web purchases`, `store purchases`, etc. |
| **Promotion** | Fields describing campaign results and promotions. |

---

## 🛠 Steps to Perform

### **1. Data Import & Verification**
- Import dataset and inspect variables like `Dt_Customer` and `Income` to ensure correct data types.

### **2. Missing Value Imputation**
- Handle missing `Income` values:
  - Assume customers with similar **education** and **marital status** have the same average yearly income.
  - Clean category labels in `education` and `marital status` before imputation.

### **3. Feature Engineering**
- Create new variables:
  - `Total_Children`
  - `Age`
  - `Total_Spending`  
    *(Hint: Sum purchases through all three sales channels)*

### **4. Outlier Treatment**
- Create **box plots** and **histograms** to visualize distributions.
- Apply outlier treatment where necessary.

### **5. Encoding**
- Use **ordinal encoding** for ordered categorical variables.
- Use **one-hot encoding** for nominal categorical variables.

### **6. Correlation Analysis**
- Create a **heatmap** to show correlation between variables.

---

## 📊 Hypotheses to Test
1. Older people are less tech-savvy and prefer shopping **in-store**.
2. Customers with kids prefer **online shopping** due to time constraints.
3. Other sales channels may **cannibalize** in-store sales.
4. The US performs significantly better than the rest of the world in total purchases.

---

## 📈 Additional Analysis & Visualizations

- **Product Performance**  
  Identify top and least performing products in terms of revenue.

- **Age vs. Campaign Acceptance**  
  Analyze patterns between customer age and last campaign acceptance rate.

- **Geographic Insights**  
  Which country has the highest number of customers accepting the last campaign?

- **Children at Home vs. Spending**  
  Explore the relationship between the number of children and total spending.

- **Customer Complaints**  
  Education background of customers who complained in the last 2 years.

---

## 📦 Technologies Used
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib / Seaborn**
- **Scikit-learn**

---

## 📜 License
This project is open-sourced under the MIT License.
