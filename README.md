# 🏥 Medical Data Analysis using SQL

A SQL project that solves 34 questions on a hospital database using MySQL Workbench.

## 🗄️ Database Schema

Database name: `medical_data`

**patients**
```
patient_id    integer
first_name    text
last_name     text
gender        varchar(1)
birth_date    date
city          text
allergies     text
height        integer
weight        integer
province_id   char(2)
```

**admissions**
```
patient_id       integer
admission_date   date
discharge_date   date
diagnosis        text
doctor_id        integer
```

**doctors**
```
doctor_id   integer
first_name  text
last_name   text
specialty   text
```

**province_names**
```
province_id    char(2)
province_name  text
```
## 🛠️ SQL Concepts Used

- Filtering: WHERE, LIKE, BETWEEN, IN, IS NULL
- Sorting and limiting: ORDER BY, LIMIT, DISTINCT
- Aggregate functions: COUNT, SUM, MAX, MIN
- Grouping: GROUP BY, HAVING
- JOINs across 2 and 3 tables
- CASE statements
- UNION ALL
- String functions: CONCAT, UPPER, LOWER, LENGTH
- Date and math functions: YEAR, DAY, FLOOR, POWER
- UPDATE and ALTER TABLE

## 💻 Tool

MySQL Workbench 

## 📊 Key Findings

- Admissions are spread across all days of the month, with the 4th and 11th having the most (184 each).
- Only 2 patients had 'Epilepsy' with a doctor named 'Lisa' (found by joining 3 tables).
- Patients were grouped by weight into groups of 10 kg to see how weight is distributed.

## 🎯 What I Learned

- Writing SQL queries to answer real-world hospital data questions
- Joining 2 and 3 tables using JOIN
- Summarizing data with GROUP BY, HAVING and aggregate functions
- Creating new columns using CASE and string/date functions
- Cleaning and preparing data using UPDATE and ALTER TABLE
