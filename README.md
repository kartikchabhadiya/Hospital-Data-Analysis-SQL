# Hospital Data Analysis (SQL Project)

This project contains SQL queries for analyzing hospital data.  
It demonstrates how to use **aggregation, grouping, subqueries, ordering, and date functions** to solve real-world healthcare analytics problems.  

---

## 📊 Project Overview
The dataset represents hospital records with columns such as:
- **hospital_name**
- **location**
- **department**
- **doctors_count**
- **patients_count**
- **admission_date**
- **discharge_date**
- **medical_expenses**

Using this dataset, queries were written to answer different business questions related to patients, doctors, departments, and expenses.

---

## ✅ Queries Covered
1. **Total Number of Patients** – Calculate the sum of patients across all hospitals.  
2. **Average Number of Doctors per Hospital** – Find the average number of doctors in each hospital.  
3. **Top 3 Departments with Highest Number of Patients** – Identify departments with maximum patient load.  
4. **Hospital with Maximum Medical Expenses** – Retrieve the hospital that spent the most.  
5. **Daily Average Medical Expenses** – Compute per-day average expenses using date differences.  
6. **Longest Hospital Stay** – Find the patient(s) with the longest stay duration.  
7. **Total Patients Treated per City** – Sum of patients grouped by location.  
8. **Average Length of Stay per Department** – Average days spent in each department.  
9. **Department with Lowest Number of Patients** – Identify least busy department.  
10. **Monthly Medical Expenses Report** – Group expenses by month.  

---

## 🛠️ Technologies Used
- **PostgreSQL** (queries tested)
- **SQL concepts**: `GROUP BY`, `ORDER BY`, `LIMIT`, `SUM()`, `AVG()`, `MIN()`, `MAX()`, `ROUND()`, `TO_DATE()`, `TO_CHAR()`

---

## 🚀 How to Run
1. Create the table:
   ```sql
   CREATE TABLE hospital_data (
     hospital_name    VARCHAR(50) NOT NULL,
     location         VARCHAR(50) NOT NULL,
     department       VARCHAR(50) NOT NULL,
     doctors_count    INTEGER     NOT NULL,
     patients_count   INTEGER     NOT NULL,
     admission_date   VARCHAR(20) NOT NULL,
     discharge_date   VARCHAR(20) NOT NULL,
     medical_expenses NUMERIC(7,2) NOT NULL
   );
