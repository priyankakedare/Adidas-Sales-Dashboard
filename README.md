# 📊 Adidas Sales Dashboard – Power BI Project

An interactive and insightful dashboard built using Power BI to analyze Adidas sales performance across products, retailers, regions, and time periods.

---

## 🎯 Objective

To build an interactive and insightful sales dashboard for Adidas using Power BI, allowing users to explore key metrics such as **revenue**, **profit**, **sales trends**, and **regional performance** – all presented with clean visuals and dynamic filters.

---

## 🧠 Tools & Skills Used

- Power BI Desktop  
- DAX (Data Analysis Expressions)  
- Power Query for data cleaning  
- Custom JSON Theme  
- Data Modeling and Relationships  
- UX/UI Dashboard Design Best Practices  

---

## 📁 Dataset Summary

- **Source:** [Kaggle – Adidas US Sales Dataset](https://www.kaggle.com/datasets/whenamancodes/adidas-us-sales-dataset)  
- **Format:** CSV  
- **Rows:** 9,648  
- **Columns:** 14  

### 🔑 Key Columns

- Invoice Date  
- Retailer  
- Region  
- State  
- City  
- Product  
- Units Sold  
- Price per Unit  
- Total Sales  
- Operating Profit  
- Operating Margin  
- Sales Method  

---

## 🧮 Sample DAX Measures

```dax
Total Sales M = FORMAT(SUM('adidas (2)'[Total Sales]) / 1000000, "$#,##0.0M")
Operating Profit M = FORMAT(SUM('adidas (2)'[Operating Profit]) / 1000000, "$#,##0.0M")
Units Sold M = FORMAT(SUM('adidas (2)'[Units Sold]) / 1000000, "0.0M")
Operating Margin % = FORMAT(AVERAGE('adidas (2)'[Operating Margin]), "0.0%")
