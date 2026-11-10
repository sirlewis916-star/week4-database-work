# SQL Assignment - ClassicModels

## Q1: Top 5 Payments by Date
```sql
USE classicmodels;
SELECT TOP 5 paymentDate, SUM(amount) AS total_amount
FROM payments
GROUP BY paymentDate
ORDER BY paymentDate DESC;
