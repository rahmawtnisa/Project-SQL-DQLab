# 📘 DQLab SQL Bootcamp – Learning SQL Fundamentals

Welcome to my repository! This repo contains notes and exercises from the **DQLab SQL Bootcamp**, where I learned the fundamentals of SQL for data analysis. The bootcamp focuses on essential SQL concepts and how to use them effectively to gain insights from data.

---

## 🎯 Learning Objectives

- Understand the basics of SQL and relational databases
- Practice writing queries using various SQL clauses and functions
- Build a solid foundation for data analysis using SQL

---

## 🛠️ Tools Used

- **DQLab Query Editor** (official DQLab learning platform)
- **Google Big Query** (for local practice)
- **Jupyter Notebook, Google Colab** (optional, for interactive documentation)
- Sample datasets: transactions, customers, products, and sales Telco Churn Data

---

## 📚 Topics Covered

| Topic                      | Description                                                                      |
|---------------------------|----------------------------------------------------------------------------------|
| `SELECT`                  | Retrieve data from a table                                                       |
| `LIMIT`                   | Limit the number of returned rows                                                |
| `ORDER BY`                | Sort query results by one or more columns                                        |
| `WHERE`                   | Filter data based on specific conditions                                         |
| `CASE WHEN`               | Add conditional logic inside queries (similar to IF statements)                  |
| Aggregation (`SUM`, `AVG`, `COUNT`, `MAX`, `MIN`) | Perform basic statistical calculations on data                    |
| `GROUP BY`                | Group data to perform aggregation on subsets                                     |
| `HAVING`                  | Filter grouped results based on aggregate values                                 |

---

## 💻 Sample Queries

```sql
-- Show top 5 best-selling products by total quantity sold
SELECT product_name, SUM(quantity) AS total_sold
FROM sales
GROUP BY product_name
ORDER BY total_sold DESC
LIMIT 5;
```

```sql
-- Categorize customers based on their total spending
SELECT customer_id,
       CASE 
           WHEN total_spent >= 1000000 THEN 'High Spender'
           WHEN total_spent >= 500000 THEN 'Medium Spender'
           ELSE 'Low Spender'
       END AS spending_category
FROM customer_summary;
```

---

## 📁 Repository Structure

```
.
├── notebooks/               # SQL practice and notes in Jupyter Notebooks
│   └── sql_practice.ipynb
│
├── screenshots/             # Screenshots of query results from DQLab
│   └── select_query_result.png
│
├── dataset/                 # Sample datasets for offline practice (if needed)
│   └── sales_data.csv
│
└── README.md
```

---

## 📝 Personal Notes

This bootcamp helped me better understand how SQL can be used to answer business questions efficiently. Concepts like `GROUP BY` and `CASE WHEN` were especially useful for segmenting and summarizing data.

---

## 📬 Contact

- Name: Rahmawati Annisa Salsadilla  
- Email: rahmawati.salsadila@gmail.com  
- LinkedIn: [Rahmawati Annisa Salsadilla](https://www.linkedin.com/in/rahmawatiannisasalsadilla/)

---

## ✅ Project Status

📅 Last updated: February-March 2025  
🚀 Status: Completed  
