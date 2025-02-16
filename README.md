# SQL-Query-_-Cumulative-SUM

**🚀 SQL Interview Question: Cumulative Sum / Running Total**  

In SQL interviews, a common question is:  
👉 *How do you calculate the cumulative sum (running total) of salaries in a table?*  

💡 Here’s a simple solution using the **SUM() OVER()** window function:  

```sql
SELECT emp_id, empname, salary,  
       SUM(salary) OVER (ORDER BY emp_id) AS cumulative_sum  
FROM employees;
```

✅ This query calculates the running total of salaries, ordered by `emp_id`.  

📌 *Why is this useful?*  
- Helps in financial reporting 📊  
- Used in trend analysis 📈  
- Common in business intelligence dashboards
  



