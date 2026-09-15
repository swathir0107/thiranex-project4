# 🛍️ Retail Sales Data Analysis Using Python

## 📌 Project Overview

This project focuses on analyzing a real-world retail sales dataset using Python. The objective is to understand customer purchasing behavior, product category performance, sales trends, and relationships between different variables.

The project follows an end-to-end data analysis workflow, starting from data loading and cleaning and continuing through exploratory data analysis, visualization, and business insights.

---

## 🎯 Project Objectives

The main objectives of this project are:

* To understand the structure of the retail sales dataset.
* To clean and prepare the data for analysis.
* To identify missing values and duplicate records.
* To analyze overall sales performance.
* To understand customer purchasing behavior.
* To compare sales across product categories.
* To analyze sales trends over time.
* To study the relationship between age, quantity, price, and total sales.
* To identify important business insights from the data.
* To present findings using clear and meaningful visualizations.

---

## 📂 Dataset

The dataset used in this project is:

**`retail_sales_dataset.csv`**

The dataset contains **1,000 retail transaction records** and the following columns:

| Column             | Description                                       |
| ------------------ | ------------------------------------------------- |
| `Transaction ID`   | Unique identification number for each transaction |
| `Date`             | Date on which the transaction occurred            |
| `Customer ID`      | Unique identification number of the customer      |
| `Gender`           | Gender of the customer                            |
| `Age`              | Age of the customer                               |
| `Product Category` | Category of the purchased product                 |
| `Quantity`         | Number of units purchased                         |
| `Price per Unit`   | Price of one unit of the product                  |
| `Total Amount`     | Total amount spent in the transaction             |

---

## 🛠️ Technologies Used

The following technologies and Python libraries are used:

* **Python**
* **Jupyter Notebook**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**

---

## 🔄 Project Workflow

The project follows the following data analysis workflow:

```text
Dataset
   ↓
Data Loading
   ↓
Data Understanding
   ↓
Data Cleaning
   ↓
Feature Engineering
   ↓
Exploratory Data Analysis
   ↓
Data Visualization
   ↓
Correlation Analysis
   ↓
Outlier Analysis
   ↓
Business Insights
   ↓
Conclusion
```

---

## 🧹 Data Cleaning

The following data-cleaning operations were performed:

1. Loaded the dataset using Pandas.
2. Checked the number of rows and columns.
3. Examined column names and data types.
4. Checked for missing values.
5. Checked for duplicate records.
6. Removed duplicate records where necessary.
7. Converted the `Date` column into the appropriate datetime format.

---

## ⚙️ Feature Engineering

Additional date-related features were created from the `Date` column:

* `Year`
* `Month`
* `Month Name`
* `Day`
* `Day of Week`

These features make it easier to analyze sales patterns across different time periods.

---

## 📊 Exploratory Data Analysis

Several analyses were performed to understand the retail business.

### 1. Overall Sales Analysis

The project calculates:

* Total sales
* Average transaction amount
* Maximum transaction amount
* Minimum transaction amount
* Total quantity sold

### 2. Customer Analysis

Customer behavior is analyzed using:

* Number of unique customers
* Sales by gender
* Number of transactions by gender
* Top customers based on total spending

### 3. Product Category Analysis

Product categories are analyzed based on:

* Total sales
* Quantity sold
* Average price per unit

### 4. Time-Based Sales Analysis

Sales trends are analyzed by:

* Year
* Month
* Day of the week

### 5. Age Analysis

Customer age is analyzed using:

* Age distribution
* Relationship between age and total spending

### 6. Quantity and Price Analysis

The project examines:

* Quantity distribution
* Quantity versus total amount
* Price per unit distribution
* Price per unit versus total amount

---

## 📈 Data Visualizations

The following visualizations are created using Matplotlib and Seaborn:

* Sales by gender
* Number of transactions by gender
* Sales by product category
* Quantity sold by product category
* Average price by product category
* Monthly sales trend
* Sales by day of the week
* Customer age distribution
* Age versus total amount
* Quantity distribution
* Quantity versus total amount
* Price per unit distribution
* Price per unit versus total amount
* Correlation heatmap
* Sales outlier analysis
* Top 10 customers by spending

These visualizations make it easier to identify patterns and trends in the dataset.

---

## 🔥 Correlation Analysis

A correlation matrix is used to examine relationships between numerical variables such as:

* Age
* Quantity
* Price per Unit
* Total Amount

A heatmap is created to visually represent these relationships.

The correlation analysis helps determine whether variables have positive, negative, or weak relationships with each other.

---

## 📦 Outlier Analysis

Box plots are used to identify potential outliers in:

* Age
* Quantity
* Total Amount

Outlier analysis helps understand unusual transactions or customer records that may require further investigation.

---

## 💡 Key Business Questions

The project attempts to answer questions such as:

1. What is the total revenue generated?
2. What is the average transaction value?
3. Which product category generates the highest sales?
4. Which product category has the highest quantity sold?
5. Which gender contributes more to total sales?
6. Which month has the highest sales?
7. Which day of the week generates the highest sales?
8. Which customers spend the most?
9. Is there a relationship between quantity purchased and total amount?
10. Is there a relationship between customer age and spending?
11. How does price per unit affect the total transaction amount?

---

## 📌 Business Insights

The analysis can help a retail business:

* Identify high-performing product categories.
* Understand customer purchasing patterns.
* Identify high-value customers.
* Understand monthly sales trends.
* Determine which days have stronger sales activity.
* Understand the relationship between quantity and spending.
* Develop better marketing and sales strategies.
* Make more informed business decisions using data.

The exact numerical findings are generated directly from the dataset when the analysis notebook is executed.

---

## 📁 Project Structure

```text
Retail-Sales-Data-Analysis/
│
├── retail_sales_dataset.csv
│
├── Retail_Sales_Analysis.ipynb
│
├── README.md
│
└── visualizations/
    │
    ├── sales_by_gender.png
    ├── sales_by_category.png
    ├── monthly_sales_trend.png
    ├── sales_by_day.png
    ├── age_distribution.png
    ├── quantity_distribution.png
    └── correlation_heatmap.png
```

---

## ▶️ How to Run the Project

### Step 1: Install Python

Download and install Python from the official Python website.

### Step 2: Install Required Libraries

Open the terminal or command prompt and run:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Step 3: Open Jupyter Notebook

Run:

```bash
jupyter notebook
```

### Step 4: Open the Project

Open:

```text
Retail_Sales_Analysis.ipynb
```

Make sure the following file is in the same folder:

```text
retail_sales_dataset.csv
```

### Step 5: Run the Notebook

Execute the notebook cells from top to bottom.

---

## 🧪 Example Code

The dataset can be loaded using:

```python
import pandas as pd

df = pd.read_csv("retail_sales_dataset.csv")

df.head()
```

The date column can be converted using:

```python
df['Date'] = pd.to_datetime(df['Date'])
```

Total sales can be calculated using:

```python
total_sales = df['Total Amount'].sum()

print("Total Sales:", total_sales)
```

---

## 📊 Expected Outcome

After completing the project, the analysis provides a better understanding of:

* Retail sales performance
* Customer behavior
* Product category performance
* Sales trends
* Purchasing quantities
* Pricing patterns
* Relationships between numerical variables

The project demonstrates how Python and data science techniques can be applied to a real-world retail business problem.

---

## 🚀 Future Improvements

The project can be extended in the future by adding:

* Sales forecasting
* Customer segmentation
* Machine learning models
* Customer lifetime value analysis
* Recommendation systems
* Interactive dashboards using Power BI or Tableau
* Automated business reports
* Advanced time-series forecasting

---

## 🏁 Conclusion

This project demonstrates an end-to-end approach to retail sales data analysis using Python.

The dataset was first loaded and cleaned, followed by exploratory data analysis and feature engineering. Different statistical techniques and visualizations were then used to understand customer behavior, product performance, and sales trends.

The insights obtained from this analysis can help retail businesses understand their customers, identify successful product categories, recognize high-value customers, and make data-driven decisions.

Overall, this project demonstrates the practical application of **Python, Pandas, NumPy, Matplotlib, and Seaborn** to a real-world data analysis problem.

---

## 👨‍💻 Skills Demonstrated

Through this project, the following skills are demonstrated:

* Python Programming
* Data Cleaning
* Data Preprocessing
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Statistical Analysis
* Data Visualization
* Correlation Analysis
* Outlier Detection
* Business Insight Generation
* Data-driven Decision Making

---

## 📜 License

This project is created for **educational and learning purposes** as part of a real-world data analysis project.

---

## ⭐ Acknowledgement

This project was developed as a practical exercise in applying data science and analytics techniques to a retail dataset.

The project follows an end-to-end data analysis approach covering data preparation, analysis, visualization, and interpretation.
